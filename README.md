Spotify Openbox Wrapper
======================

This project provides support for notifications and control through
your keyboard media keys for Spotify when you are using Openbox.

The script uses the Spotify-DBus-interface to control the client.

Many thanks to [John Reese](https://github.com/jreese/spotify-gnome) for 
this excellent idea and the great script he created.

Requirements
============
 - python2
 - python2-notify
 - OpenBox

Installation
============
Installation of the script isn't yet particularly useful but if you'd
like to install it anyways, follow instructions below.

Verify the installation directory of Spotify
    
    `$ which spotify    
    /usr/bin/spotify`

If Spotify was installed in a different directory you'll need to
change `spotify_bin` to the directory of your installation.    
    
Copy `src/spotify` to `/usr/local/bin/spotify` or another directory
that is precedent over the location of your Spotify binary.

    `sudo cp bin/spotify /usr/local/bin && sudo chmod 755 /usr/local/bin/spotify`    
    
Launching Spotify should now result in launching the wrapper first, which
will launch the official client after binding to the keys and DBus-interface.    
    
Binding to your media keys is not yet possible, but this section will follow
soon.

Details
=======
spotify-ob-wrapper v0.1    
by Bas Dalenoord, mijn.me.uk    
Copyright (c) 2012 All rights reserved    
    
This project is licensed under the BSD license. See the LICENSE file for 
details.    

Please report any bugs/issues through GitHub.
