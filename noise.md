# Noise

### Libraries
- https://github.com/keijiro/NoiseShader
- https://github.com/stegu/webgl-noise

### Value erosion
- https://x.com/Tuatara_Games/status/1859658039172923439
- en = saturate( ( sat(n)-sat(erosionAmt) ) / ( softnessAmt=0.5) )

### Equirectangular textures
- https://x.com/PavelBoytchev/status/1799750298598269282
- https://x.com/SoundSafari_io/status/1799823934080385208
- https://boytchev.github.io/texture-generator/
- https://boytchev.github.io/tsl-textures/
- https://boytchev.github.io/tsl-textures/online/rust.html
- https://x.com/PavelBoytchev/status/1799828767428546827
- https://x.com/PavelBoytchev/status/1804585068138258457
- https://boytchev.github.io/tsl-textures/online/gas-giant.html
- https://x.com/junkiyoshi/status/1818971508091519102
- https://x.com/PavelBoytchev/status/1797322139239874924  ( Planet )

### Normal Map
- https://x.com/PavelBoytchev/status/1804585068138258457
- https://boytchev.github.io/tsl-textures/examples/example-normal-map.html

### Wood
- https://x.com/PavelBoytchev/status/1813922290813509737
- https://boytchev.github.io/tsl-textures/examples/example-wooden-toys.html

### Cube voronoi pattern
- https://x.com/etiennejcb/status/1848760136145436784
- https://x.com/TinySodaCans/status/1849019439964115451
- https://mathstodon.xyz/@bleuje/113346828157692078
- https://github.com/Bleuje/processing-animations-code/tree/main/code/moorevoronoi
- Moves using moore curve
- uses "accurate sdf"
- replacement technique on Moore curve + design with voronoi cells around points with a shader
- https://iquilezles.org/articles/voronoilines/
For the voronoi cells edges/contours, here is an excerpt from my shader code (where col is the brightness):
float v = 0.4*min(abs(minDist-4),abs(minDist-10));
float col = smoothstep(0.7,0.3,v);
And that minDist is found with an algo from 
@iquilezles

### Zebra
- https://junkiyoshi.com/openframeworks20241104/
- https://github.com/junkiyoshi/Insta20241104
- https://x.com/junkiyoshi/status/1853397536356335643

### Sin SNoise 2D
- https://x.com/DrkFX/status/1859341955500585425
- https://x.com/Renard_VRC/status/1859219331218862183
- o+=sin(snoise2D(FC.xy/r*5.)*64.);

### Neural Noise
- https://x.com/uuuuuulala/status/1796164993039094061
- https://x.com/zozuar/status/1625182758745128981/
- https://codepen.io/ksenia-k/full/vYwgrWv

### Layering and Blending Noise
- https://github.com/hippowombat/FastNoiseLayeringPlugin
- https://github.com/Rockam/FastNoise-UE4-Wrapper
- https://github.com/Auburn/FastNoiseLite
- https://x.com/hippowombat/status/1864030770345459932
- Inspired by @NoMansSky 's GDC talk on noise layering
- https://www.youtube.com/watch?si=rDy-bBiZexrUGoEa&v=C9RyEiEzMiU&feature=youtu.be