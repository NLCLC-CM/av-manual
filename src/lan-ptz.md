# LAN PTZ Architecture

# Background

The current livestreaming requirement started during the COVID pandemic in 2020. We were graced with
2 camcorders (and an old PTZ with 3x zoom), and we have run with them since. 5 years have passed, and
along with that, a large amount of wear and tear on the already ~17 year old equipment. In fact, one of
the camcorders is currently unusable due to an autofocus malfunction.

These camcorders were presented as temporary solutions to a temporary problem. Now that they are an
integrated solution into our hybrid worship service, it is time to upgrade.

# Current approved solution

We have proposed (and Council has approved) the following purchases:

- 2 x PTZ cameras with 30x zoom
- 1 x PTZ camera controller
- 1 x Power-over-Ethernet (PoE) switch
- Various cables and extenders to connect everything

# Connecting everything together

- All cameras will be connected to the PoE switch for power and control
- Camera outputs are routed into the ATEM mini video multiplexer (muxer) for a seamless upgrade experience
- The controller is connected to the PoE switch to control the camera
- Computers on the church office network are also able to control the cameras
- IP addresses for connected devices are set statically such that reconfiguration isn't necessary

# PTZ cameras

They are mainly controlled by the physical PTZ controller. Though they can also be controlled by a remote
or any computer on the church office network. To control them via IP address, you can use the remote in
conjunction with the screen to display what the camera is outputting.

- Press `Menu`
- Go to `Network settings`
- See the IP address of the camera

You can also use the controller to view the IP address of the camera, if the IP address of the camera
hasn't changed. You can verify that the IP address of the camera hasn't changed by trying to use the
joystick to control the camera in question.

# PTZ controller

Instructions may not be completely accurate because I'm going off of memory.

## Typical usage

There are 3 methods of controlling the camera. By descending order of typicality:

1. The physical controller
2. The remote control (which has nothing to do with the controller)
3. The camera's web interface (which also has nothing to do with the controller)

Below are the two ways of controlling the camera. Note that both these ways can be achieved with any of
the above 3 methods.

**Joystick.** Play around with the joystick to get a feel of how to use it. Zooming in/out is done by
twisting the joystick itself, or by using the slider on the bottom-left of the controller.

**Presets.** When you have a camera configuration you like and would like to save it to the camera, press
the `PRESET` button on the controller, followed by the slot number you would like to set it to (1-255),
then press `ENTER`. Note that each ministry has [their own set of slot
numbers](./sunday.md#ptz-controller) that only they can edit, so don't go overwriting their presets. To
call a certain preset, press `CALL`, followed by the slot number you would like to call (1-255), then
press `ENTER`. The camera will snap to the pre-defined position.

## Adding a new camera

You can use either the physical controller or the online interface to do this. To use the physical
controller:

1. Press `SETUP`
2. Go to `Add Network...`, which should be the first option
3. Fill in the fields accordingly

To use the online interface

1. Go to the IP address displayed on the physical controller
2. Log in with `admin` credentials
3. Go to `Discover` to discover a camera
4. If the camera is connected to the same network, it should show the camera on the list

## Unable to control the camera

- Check that you are on the correct camera number
- If the display says that a timeout has occurred, this means that the camera's IP address has changed,
  and you have to edit the camera settings
