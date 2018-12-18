# godot-touch-joystick
A touchscreen joystick for use in godot 3

## Functions and Signals
The Joystick contains 3 signals
_joystick_pressed is emited when the joystick is touched
_joystick_released is emitted when the user releases the joystick
_joystick_axis_change is emitted when the axis value is changed the new axis value is also supplied

to get the current joystick axis value use the getStickPosition() method it will return a Vector2() ranging between (-1,-1) and (1,1)

if the circular pad is within the adjustable dead_zone it will defualt to returning (0,0)

## Adjustable Properties
circle_pad_radius sets the radius of the circle pad itself
dead_zone a circular area in the center of the joystcik in which input is ignored
outer_ring_radius sets the size of the space in which the circle pad can move
touch_screen_only can be set to block the joystick from displaying on devices that do not have a touchscreen or support emulation of one
