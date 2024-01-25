# Sunday setup

This entire process can be done by 1 person in 10 minutes if there are no outstanding issues.

## Prerequisites

- Phone and earphones

## Procedure

- [Set cameras](#cameras)
- Start presenting the powerpoint
    - Download this Sunday's powerpoint
    - Start presenting the powerpoint
- Open OBS and start streaming
    - Open YouTube and log in (usually already logged in)
    - Click `Go live` on YouTube
    - Set the name of the livestream to `信義會新生堂 x年x月x日`
    - Set the thumbnail of the livestream to a screenshot of the first slide of the powerpoint
    - Start streaming in OBS
    - Send livestream link to Whatsapp
    - Continue to monitor the livestream via your phone and earphones
- (Optional) stream audio check
- Start [Zoom](#zoom)
    - Enter the Zoom room with the given room ID and password (pick from dropdown)
    - Open YouTube and navigate to the livescreen
    - Wait for the host to grant screen-share permissions
    - Screenshare the livestream, taking care to also stream the audio and check the box that says
      to stream in "video mode"

# Cameras

There are pieces of sticky tape on both cameras, but the settings to change are the following:

- Settings -> CTRL for HDMI -> Off
- Settings -> Demo Mode -> Off
- Settings -> Power Save -> Off
- Photos -> Facial Recognition -> Off

These settings will already be mostly set on the camera that doesn't completely reset itself (the
right-most one usually).

Be cautious when touching the cameras in the winter because static electricity may reset the cameras.
Always discharge yourself on a nearby metal object.

## The third frontal camera

The eagle-eyed viewer may notice that there are 3 HDMI cables running into the video mixer, but there are
only 2 cameras at the back. There is a camera on top of the wooden piano in the front. You can control the
angle the camera is pointing with the 3rd remote (the remote with all the batteries on display). You can
also control the magnification of the camera. The remote can control the camera in ideal conditions:

- The camera's IR sensors are facing towards you
- There is clear line-of-sight between the remote's IR emitter and the camera's IR sensors

# Zoom

On the off chance that you also have to control the Zoom meeting. The laptop that we will be using is the
one that is currently stored in the Sunday School cabinet beside the printer (Cathay Pacific lanyard). It
is in the third drawer counting from the top.

1. Laptop
2. Power cable
3. USB to ethernet dongle

The PIN is the same PIN for Cantonese ministry login.

- When users enter the room, be sure to greet them as an usher would

> Existing issue: if the laptop enters a Zoom meeting when the desktop computer livestreams, and when the
> laptop and desktop computers are both on the same switch (i.e. the laptop via the USB to ethernet dongle),
> there's a high chance that the livestream on YouTube's side fails. In such cases, use WiFi for laptop
> connectivity.

In general, use WiFi to connect the laptop to the internet.

# Troubleshooting

I take a page out of commercial aviation: Aviate, Navigate, Communicate. Except we can skip the middle
one. The most important thing is to continue controlling the Powerpoint and on-site audio. There are
usually 2 people assigned to the Sunday post. 1 of them will do the Powerpoint and audio. The other will
be there to support and communicate, suggest ideas.

Remember: <kbd>alt</kbd>+<kbd>tab</kbd> is your friend.

## No internet

You won't be able to do anything. Most likely, the following will happen after the internet disconnects
for more than 1-2 minutes: [YouTube livestream auto-ends](#youtube-livestream-ends-prematurely), Zoom
meeting auto-transfers host to a random other participant. You will be able to troubleshoot when internet
returns.

## Youtube livestream ends prematurely

You will only be able to troubleshoot when internet returns.

1. Go to YouTube and `Go live` again
2. Start streaming in OBS
3. Check that we are sending packets to YouTube by checking stream status on YouTube
4. Send the new stream link in Whatsapp
5. Redo the Zoom procedure

## No video from 3rd frontal camera

1. Check that the frontal camera is powered
2. Press the `sync` button on the HDMI/ethernet bridge
3. Press the `sync` button on the ethernet/HDMI bridge

## Laggy system

This could be caused by pure chance, and is usually diagnosed at the setup phase. The following are some
ways this lag could be mitigated, ordered from least disruptive to most disruptive. Only try them if you
absolutely have to.

1. Reduce the number of PowerPoint files open at once
2. Close the browser
3. Restart OBS
4. Restart the computer

## OBS cannot pick up audio/video

Probably caused by a driver not getting detected. These instructions will disrupt the livestream.

1. Unplug/replug the video mixer USB
2. Restart OBS

The audio comes from a LAN cable, and I have no clue how it works.
