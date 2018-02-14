# Prime Mover (Coming soon at PrimeMover.io) 

Bash script(s) to facilitate migration of WordPress sites into and out of servers managed by GridPane, ServerPilot, RunCloud, and (possibly) others. 

Copyright 2018 - K. Patrick Gallagher

# CAUTION!!!

This is all very VERY aplha right now. Use at your own risk.

This is basically a highly neutered version of the MigrateSafely migration tool we use internally at GridPane.com

So all kinds of things might be completely broken. Please feel free to help out.

Best of luck! Drop me a line at patrick at gridpane dot com

# INSTALL

This documentation is coming soon. 

Basically: 

1.) Download primemover.sh

2.) Run "chmod +x primemover.sh"

3.) Run "mv primemover.sh /usr/local/bin/primemover"

Done.

# BIG PICTURE

In order for this to work (for ServerPilot and RunCloud) you need to have already created SSH keys on both your source server and your destination server. You need to have also already added these keys between your source and destination server.

This all automatigically works if you're using GridPane because we kick all of the asses.

Currently - version Nothing Dot Zero Zero Zero One - February 14th, 2018, this will only work to migrate sites out of EasyEngine, ServerPilot, RunCloud, and SOME CPanel nodes and push this sites IN to GridPane managed servers.

But coming very soon - end of the week probably - I'll reintegrate all of my original code for moving things between ServerPilot nodes and from ServerPilot to already provisioned sites at RunCloud. And, obviously, all the various back and forth versions of that. 

I probably won't build a version of this that will migrate sites out of GridPane and into these other control panels. 

I'm not going to poke any of my daughters in the eye, either. Because I like them too. 

I'll leave it to the community to knock out that simple chunk of code. It's actually already there, if you know what you're looking for. 

# USAGE

primemover $SOURCEURL (or ALL) $DESTIP $SOURCETOKEN $DESTTOKEN

Lots and lots of improvements coming very soon.

Building new sites on ServerPilot is super simple because their API is well done. Building sites on RunCloud currently can't be automated. You'll need to manually build them first.

The syntax for that (moving a site to RC) will be "primemover $SOURCEURL (ALL) $DESTIP $DESTPATH" (This ins't implemented yet)

# MORE DOCUMENTATION COMING SOON!!!
