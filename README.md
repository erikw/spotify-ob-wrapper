Spotify Openbox Wrapper
======================

This project provides support for notifications to Spotify. I designed this
script for OpenBox, but it might be usable under different WM's anyway.

The script uses the Spotify-DBus-interface to control the client.

Many thanks to [Stuart Colville](http://muffinresearch.co.uk/archives/2011/03/23/linux-spotify-track-notifier-with-added-d-bus-love/) for 
this excellent idea and the great script he created, and to [Abhijeet Rastogi](http://blog.abhijeetr.com/2012/01/spotify-song-change-notifications-with.html)
for the modifications to use Spotify's own album art. I used part of the
code from [John Reese](https://github.com/jreese/spotify-gnome) to make
this script launch the actual Spotify client.

Requirements
============
 - python2
 - python2-notify
 - python2-gobject
 - libnotify

Installation
============
Verify the installation directory of Spotify
    
    $ which spotify    
    /usr/bin/spotify

If Spotify was installed in a different directory you'll need to
change `SPOTIFY_BIN` to the directory of your installation.    
    
Copy `src/spotify` to `/usr/local/bin/spotify` or another directory
that is precedent over the location of your Spotify binary.

    sudo cp bin/spotify /usr/local/bin && sudo chmod 755 /usr/local/bin/spotify    
    
Launching Spotify should now result in launching the wrapper first, which
will launch the official client after binding to the keys and DBus-interface.    
    
Binding to your media keys is not yet possible, but this section will follow
soon.

Details
=======
spotify-ob-wrapper v0.2    
by Bas Dalenoord, mijn.me.uk    
Copyright (c) 2012 All rights reserved    
    
This project is licensed under the BSD license. See the LICENSE file for 
details.    

Please report any bugs/issues through GitHub.
