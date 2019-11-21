
# Simple Setup instructions

Hopefully this is a good take on the simplest approach to cutting the cord.

## Expectations:
This is the minimum to have a decent (in my opinion) setup where you can manage your own library of media. DO NOT expect to play 4k content.

## Steps

For this you can get an old computer, or a new raspberry Pi.

Depending on how much media you expect to have, you may want to buy an external drive with enough storage.

```
+--------------+                 +------------+
! Media Server ! <-------------> !  Smart TV  !
+--------------+                 +------------+
```

In this setup, you only need a computer with enough computer processing power and enough storage for your media.

As much as I want to keep things simple, there's knowledge that needs to be shared/known which influences how simple this simple setup can be.

In simple terms, video and audio media are stored in a encoded manner, that means it's stored in a certain way that needs to be compatible with the player you want to use (e.g. your Smart TV).

If the format (encoding) is not understood by the player, then the server needs to do what's called "transcoding", e.g. convert the media from one format to another that the player understands.

For a smooth playback experience, your Media Server needs to be able to transcode the media at least in real time, (ideally faster, as it's doing other things, like transferring data over the network, reading data from disk, etc).

For the simple setup, you can use an old/unused spare computer (try to use at least an Intel i5, with 8GB of RAM). But people have success with Raspberry PIs as well.

You don't need a lot of processing power if the video/audio formats you have can be played directly by your Smart TV (or player). When that happens we say it's a "Direct Play" (as there's no re-encoding happening).

If you want to use Linux for your Media Server, you can follow these instructions:
https://wiki.archlinux.org/index.php/plex

For Ubuntu and other distros the instructions should be similar.

What you're doing is basically:
1) Install "Plex Media Server" package for your distro
2) Enable and Start the service
3) Take note of your Server IP, and note the port is 32400 (default)
4) Configure a reverse proxy to it, if you want to access your player remotely. *


* In this case, "remotely" (loosely) means you're gonna be using the web player to consume media. If you're consuming media using your phone and the Plex app, the you need a Plex Pass.


