# Maths

### Math as Code
- https://github.com/Experience-Monks/math-as-code

### Inigo Quilez
- https://x.com/iquilezles/status/1815189030826602876 useful functions

### Chromatric aberration
- https://x.com/XorDev/status/1831738521935360079
- col.rgb += dFdx( col.rgb ) * vec3( 3,0,-3 )

### Exponential density - SDF kind of fake bloom ?
- https://x.com/Pete_Nichols_fx/status/1831952014399697085

### Dot Product, Cross Product, Quaternions, and Matrix Rotation
- https://x.com/ushadersbible/status/1826850118152110343

### Compute Shader Structure
- https://x.com/FreyaHolmer/status/1826718390574350550

### Repeat Binary Patterns
- https://x.com/FreyaHolmer/status/1823312779152966087
```
with pattern p of stride s, the repeated uint is:
p*( 4294967295 / ((1<<s)-1) )

for example!
p: 1101 (13)
s: 4 (bits of stride)
= 11011101110111011101110111011101 (3722304989)
```

### SmoothClamp
- smoothstep(min, max, x) * (max - min) + min
- https://x.com/jakubtomsu_/status/1822939696009204128

### Pringles - hyperbolic paraboloid
- https://x.com/PhysInHistory/status/1820511027370352667
- z = ( x^2 / a^2 ) - ( y^2 / b^2 )

### Meters per Pixel in shader
- https://x.com/FreyaHolmer/status/1820157167682388210
- m / px = ( 2 * clip_w_coord ) / ( camera_width_in_px * proj_matrix )


### Eerp
- https://x.com/FreyaHolmer/status/1813629237187817600
- a * Exp( T * Log( b/a ) )

### Different way to do Abs with scalling
- https://x.com/XorDev/status/1808261880009445856
- abs( x ) : max( x*a, -x*b )

### spherize UV
- https://x.com/bruno_simon/status/1801637441645789683

## UV to Vec3
- https://x.com/SoundSafari_io/status/1800686190468661630