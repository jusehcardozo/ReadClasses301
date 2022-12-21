Jose Cardozo 
12/21/2022

https://wiki.freeradius.org/guide/Concepts


RADIUS Concepts
How things work in RADIUS
The client sends the server a RADIUS authentication request. You don't decide what's in the request, the client does. The server doesn't decide what's in the request, the client does. The client is 100% responsible for everything in the request.

Picking an Auth-Type - authorize {}
The radius server looks at the request and says:

Hmmm... can I deal with this request?

The answer to that depends on what authentication types you have enabled in the server, what the server can look up in a database, and what is in the request.

The server will then start querying the modules in the authorize section:

Unix module, can you handle this one?

Pap module, can you handle this one?

Mschap module, can you handle this one?

At some point, one of the modules will say:

Yes, I see something in the request I recognize. I can do something!

Authenticating a user - authenticate {}
At the end of authorize, the server will check if anything set the Auth-Type.

If nothing did, it immediately rejects the request.

Lets suppose that the client sends a request with a User-Password attribute, and pap is enabled, the pap module will then have set Auth-Type = pap.

So in authenticate, the server will call the pap module again:

I see a User-Password, which is what the user entered. That's nice, but I need to compare it with something. Ah! Another module added the "known good" password for this user in authorize!

So it then compares the local "known good" password to the password as entered by the user. This is how authentication works.

The "known good" password comes from another module. The pap module just does PAP authentication, and nothing more. The benefit of this approach is that the "known good" password can come from the 'users' file, SQL, LDAP, /etc/passwd, external program, etc. i.e. pretty much anything.

Insufficient information
But WAIT! What if the client sends a MSCHAP request? What does the radius server say then?

Well that's a fine kettle of fish! That client has really really tied my hands on this one!

In this case, the mschap module looks at the request, and finds the MS-CHAP attributes. It sets the Auth-Type to itself (mschap). A database module (such as LDAP, above) gets the "known good" password, and adds it to the request. The mschap module is then run for authentication. It looks for either a clear text password or nt-hash (why? look at the protocol table). If one of those hasn't been added by a datastore, the mschap module says:

Sorry, I can't authenticate the user, because I don't have the information I need to validate MSCHAP.
