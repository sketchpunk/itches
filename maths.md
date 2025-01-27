# Maths

### Collections of math examples
- https://www.geogebra.org/u/daniel+mentrard

### Math as Code
- https://github.com/Experience-Monks/math-as-code

### Inigo Quilez
- https://x.com/iquilezles/status/1815189030826602876 useful functions
- https://iquilezles.org/articles/functions/

### Derivatives
- https://medium.com/@akella/love-derivatives-and-loops-f4a0da6e2458 REALLY Cool grid animatiion

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

### UV to Vec3
- https://x.com/SoundSafari_io/status/1800686190468661630

### Pythagorean Theorem - Spherical Version
- cos(a) = cos(b) cos(c)
- https://x.com/74WTungsteno/status/1850538184255353272
- https://x.com/74WTungsteno/status/1850417403936625120
- https://x.com/74WTungsteno/status/1850296586057703697
- sin(α) = sin(a) / sin(c)
cos(α) = tan(b) / tan(c)
tan(α) = tan(a) / sin(b)
- Spherical Cosine Rule
cos(a) = cos(b)cos(c) + sin(b)sin(c)cos(α)


### Laplace Transform - Interesting damping curve equations in tweet
- https://x.com/Knowledgehub_67/status/1850978810818359303
- (( sin( tx ) ) / x ) * dx === pi / 2


### 3D Coil
- https://x.com/Knowledgehub_67/status/1850976177093017826
- e^ia = cos( a ) + i * sin( a )

### Monotone Cubic Interpolation of Quaternions
- https://x.com/anorangeduck/status/1843978305093132467
- https://x.com/anorangeduck/status/1853963107351064701
- https://theorangeduck.com/page/cubic-interpolation-quaternions#overshoot
- https://jbrd.github.io/2020/12/27/monotone-cubic-interpolation.html

### Cool Fire Pattern
- https://x.com/Pixelated_Donut/status/1856500971083575647
- https://x.com/Pixelated_Donut/status/1856339794487550371

### Geometric Spiral with Variable Angles
- https://www.tungsteno.io/post/exa-spiral_complex_geometric_sum

### Schwarz Transformations
- https://x.com/74WTungsteno/status/1861651399332806671
- https://www.tungsteno.io/post/app-schwarz_transformations/

### Möbius Transformations
- https://www.tungsteno.io/post/app-mobius_transformations/

### Bitangent Circle
- Exterior Point - https://www.tungsteno.io/post/app-circles_exterior_point_bitangent_circle
- Interior Point - https://www.tungsteno.io/post/app-circles_interior_point_bitangent_circle

### Circle Polar Line Reciprocity
- https://x.com/74WTungsteno/status/1866845634365379005
- https://www.tungsteno.io/post/app-circle_polar_recip

### Hilbert Curve
- https://github.com/mrdoob/three.js/blob/master/examples/webgl_lines_colors.html

### Projective Transformation of 4 point plane
- https://x.com/74WTungsteno/status/1863342529673855204

### Primatives
- https://mathigon.org/course/circles/spheres-cones-cylinders#sphere-volume

### Different Sine Shapes from polygon side count
- https://1ucasvb.tumblr.com/post/42906053623/in-a-previous-post-i-showed-how-to-geometrically
- https://1ucasvb.tumblr.com/post/42881722643/the-familiar-trigonometric-functions-can-be
- https://x.com/mathladyhazel/status/1867439854751297992
- PPn(x) = sec((2/n)·arcsin(sin((n/2)·x)))   // N is side count
- Psinn(x) = PPn(x)·sin(x)
- Pcosn(x) = PPn(x)·cos(x)

### Snap Vector to 45 Degree Angle
- https://x.com/iquilezles/status/1878967410272965053

### Circle from 3 Points
- https://x.com/iquilezles/status/1875802416089886751
- // Any three (non colinear) points define a circle
// { .xy=center, .z=radius }
vec3 getCircle( vec2 a, vec2 b, vec2 c )
{
    vec2 ba = b-a, cb = c-b, ac = a-c;
    float de = ba.x*cb.y-ba.y*cb.x; // zero if colinear
    vec2 ce = 0.5*(a+b+vec2(ba.y,-ba.x)*dot(ac,cb)/de);
    return vec3( ce, length(a-ce) );
}

### Rotor and Motor
- https://x.com/ENDESGA/status/1848252943553929291
- https://endesga.xyz/
- https://endesga.xyz/?page=vector
- https://endesga.xyz/?page=rotor
- https://endesga.xyz/?page=motor
- https://endesga.xyz/?page=projection

### Non-Uniform Scaling - on Normals
- https://x.com/lisyarus/status/1867287966881640472
- https://www.reedbeta.com/blog/normals-inverse-transpose-part-1/
- sx = s.y*s.z, sy = s.x*s.z, sz = s.x*s.y

- https://x.com/iquilezles/status/1866219178409316362
- https://x.com/iquilezles/status/1866586811864322554
- shadertoy.com/view/3s33zj

- https://github.com/graphitemaster/normals_revisited
Included here is some sample C code for calculating the cofactor of a 4x4 matrix which can be used instead of transpose(inverse(M))
float minor(const float m[16], int r0, int r1, int r2, int c0, int c1, int c2) {
  return m[4*r0+c0] * (m[4*r1+c1] * m[4*r2+c2] - m[4*r2+c1] * m[4*r1+c2]) -
         m[4*r0+c1] * (m[4*r1+c0] * m[4*r2+c2] - m[4*r2+c0] * m[4*r1+c2]) +
         m[4*r0+c2] * (m[4*r1+c0] * m[4*r2+c1] - m[4*r2+c0] * m[4*r1+c1]);
}
void cofactor(const float src[16], float dst[16]) {
  dst[ 0] =  minor(src, 1, 2, 3, 1, 2, 3);
  dst[ 1] = -minor(src, 1, 2, 3, 0, 2, 3);
  dst[ 2] =  minor(src, 1, 2, 3, 0, 1, 3);
  dst[ 3] = -minor(src, 1, 2, 3, 0, 1, 2);
  dst[ 4] = -minor(src, 0, 2, 3, 1, 2, 3);
  dst[ 5] =  minor(src, 0, 2, 3, 0, 2, 3);
  dst[ 6] = -minor(src, 0, 2, 3, 0, 1, 3);
  dst[ 7] =  minor(src, 0, 2, 3, 0, 1, 2);
  dst[ 8] =  minor(src, 0, 1, 3, 1, 2, 3);
  dst[ 9] = -minor(src, 0, 1, 3, 0, 2, 3);
  dst[10] =  minor(src, 0, 1, 3, 0, 1, 3);
  dst[11] = -minor(src, 0, 1, 3, 0, 1, 2);
  dst[12] = -minor(src, 0, 1, 2, 1, 2, 3);
  dst[13] =  minor(src, 0, 1, 2, 0, 2, 3);
  dst[14] = -minor(src, 0, 1, 2, 0, 1, 3);
  dst[15] =  minor(src, 0, 1, 2, 0, 1, 2);
}




### Four Bar Linkage
- https://dynref.engr.illinois.edu/aml.html
- https://www.youtube.com/watch?v=EBqrDj-Wkiw
- https://www.youtube.com/watch?v=mCoCeuhi1v8
- https://www.desmos.com/calculator/egmi3wr0o7
- https://github.com/goessner/mec2
- https://github.com/fjovine/FourBarLinkage
- https://github.com/dillonhuff/fourbar
- https://github.com/hrldcpr/linkages?files=1
- https://github.com/dillonhuff/linkage_solver
- https://github.com/Rod-Persky/Simple-Four-Bar
- https://github.com/RCmags/FourBarSimulation
- https://testbook.com/mechanical-engineering/four-bar-linkage-mechanism-and-analysis
- https://www.chegg.com/homework-help/questions-and-answers/introduction-four-bar-linkages-used-variety-common-mechanisms-windshield-wipers-many-cars--q43023507
- https://github.com/MaybeRex/FourBar
- https://codepen.io/chrdiede/pen/WNWwwqj
- https://cooperrc.github.io/engineering-dynamics/module_02/project.html
- https://www.geogebra.org/m/BueCG9ch
- https://www.softintegration.com/chhtml/toolkit/mechanism/fourbar/synth3pos.html
- https://en.wikipedia.org/wiki/Slider-crank_linkage
- https://en.wikipedia.org/wiki/Four-bar_linkage


### Polyline Convex?
    isConvex: function(resolver) {
        if (!this.isClosed() || this.isDegenerate()) return null;

        var nodes = utilArrayUniq(resolver.childNodes(this));
        var coords = nodes.map(function(n) { return n.loc; });
        var curr = 0;
        var prev = 0;

        for (var i = 0; i < coords.length; i++) {
            var o = coords[(i+1) % coords.length];
            var a = coords[i];
            var b = coords[(i+2) % coords.length];
            var res = vecCross(a, b, o);

            curr = (res > 0) ? 1 : (res < 0) ? -1 : 0;
            if (curr === 0) {
                continue;
            } else if (prev && curr !== prev) {
                return false;
            }
            prev = curr;
        }
        return true;
    },

    /** Returns the 2D cross product of OA and OB vectors
 * @param a A
 * @param b B
 * @param origin If not passed, defaults to [0,0]
 * @returns magnitude of Z vector - A positive value, if OAB makes a counter-clockwise turn,
 * negative for clockwise turn, and zero if the points are collinear.
 * @example
 * vecCross([2, 0], [0, 2]);   // returns 4
 */
export function vecCross(a: Vec2, b: Vec2, origin?: Vec2): number {
  origin = origin || [0, 0];
  const p = vecSubtract(a, origin);
  const q = vecSubtract(b, origin);
  return p[0] * q[1] - p[1] * q[0];
}
