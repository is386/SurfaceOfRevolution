# Surface of Revolution

This is a program that takes in control points for a Catmull-Rom spline and generates Surface of Revolution.

![](https://github.com/is386/SurfaceOfRevolution/blob/main/result.png?raw=true)

## Usage

`./CG_hw4 [-h] [-f F] [-u U] [-t T] [-F] [-S] [-C]`

```
optional arguments:
  -h, --help  show this help message and exit
  -f F        3D control points file
  -u U        Number of point samples of u
  -t T        Theta value
  -F          Toggle flat-shaded
  -S          Toggle smooth-shaded
  -C          Toggle caps
```

## Dependencies

- `python 3.9+`

### Python Dependencies

- `numpy`

## Features:

My program takes in args `-f`, `-u`, `-t`, `-F`, `-S` and `-C`. They are optional and there are default values set. It parses the given file for the given control points. Next, it will compute the Catmull-Rom spline using the given `num_u` parameter. The program then computes the Surface of Revolution using `num_t`. It then defines the triangles, caps, and computes the surface normal if specified. Finally, the program will print out the necessary points and data in the inventor format.
