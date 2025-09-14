# smw-physics-for-godot
Super Mario World's movement values converted from hexadecimal subpixels/frame to Godot's pixels/second.
Used the default PhysicsModifier.asm for the original values.

```
var base_jump_spd	= (11*16^1) *3.75
var base_spin_spd	= ((11*16^1) + (6*16^0)) *3.75
var jump_incr		= ((2*16^2) + (8*16^1)) *3.75
var spin_incr		= ((2*16^2) + (5*16^1)) *3.75

var max_fall		= (4*16^1) *3.75

var accel_fall_noAB	= (6*16^0) /256 *225
var accel_fall_AB	= (3*16^0) /256 *225

var max_walk		= ((1*16^1) + (4*16^0)) *3.75
var max_run		    = ((2*16^1) + (4*16^0)) *3.75
var max_sprint		= (3*16^1) *3.75

var accel_walk		= (((1*16^2) + (8*16^1)) /256 *225
var accel_run		= ((1*16^2) + (8*16^1)) /256 *225

var decel_still		= ((15*16^3) + (15*16^2)) /256 *225
var decel_walk		= ((15*16^3) + (13*16^2) + (8*16^1)) /256 *225
var decel_run		= ((15*16^3) + (11*16^2)) /256 *225

var timer_sprint	= (7*16^1) /60

var climb_spd		= (1*16^1) *3.75
var climbjump_spd	= (11*16^1) *3.75
```
