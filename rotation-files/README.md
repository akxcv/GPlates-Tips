# Rotation files

## Use GRot

In all GPlates tutorials I found people suggested using `.rot` files, which is a rotation file format compatible with [PLATES](https://ig.utexas.edu/marine-and-tectonics/plates-project/), however, GPlates has its own, more convenient, `.grot` format.

GRot's pros:
- Allows comments spanning an entire line
- Allows a newline at the end of file
- Doesn't require each line to end in `!`

See [`rotation.grot`](https://github.com/akxcv/GPlates-Tips/blob/main/rotation-files/rotation.grot) for an example.
