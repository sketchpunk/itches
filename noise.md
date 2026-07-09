# Noise

### Libraries
- https://github.com/keijiro/NoiseShader
- https://github.com/stegu/webgl-noise
- Tilable Noise : https://github.com/Bubblebird-Studio/NoiseGenerator
- https://github.com/JimmyCushnie/Noisy-Nodes/tree/master/NoiseShader/HLSL

### Tutorials
- https://x.com/iced_coffee_dev/status/2061520875799670933

hash( vec2 p ){
    vec2 M1  = vec2( 3.1251, 17.8737 );
    float M2 = 43758.545312l
    return fract( sin( dot(p,M1)*M2 ) );
}

fbm( coord, octaves, persistance, lacunarity ){
    let amp   = 0.5;
    let total = 0.0;
    let pos   = coord;

    for( i=0; i < octaves; ++i ){
        n = noise( pos );
        total += n * amp;
        amp *= persistence
        pos *= lacunarity;
    }

    return total;
}

### Value erosion
- https://x.com/Tuatara_Games/status/1859658039172923439
- en = saturate( ( sat(n)-sat(erosionAmt) ) / ( softnessAmt=0.5) )

### Dot Noise
- https://x.com/XorDev/status/1964083694924140735
  - https://mini.gmshaders.com/p/dot-noise

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

### Voronoi Projection
- https://x.com/FrnkNlsn/status/1999091833864171721

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

### Interleaved Gradient Noise
- https://x.com/XorDev/status/1907524122151731254
- https://blog.demofox.org/2022/01/01/interleaved-gradient-noise-a-different-kind-of-low-discrepancy-sequence/
- Dithering with IGN
vec2 p=ceil(FC.xy*.1);o+=step(fract(52.9829189*fract(.06711056*p.x+.00583715*p.y)),p.y/r.y/.1);

### Shard Noise - For smokey , foggy 
- https://x.com/ENDESGA/status/1726402993938104493
- https://www.shadertoy.com/view/dlKyWw

### Multi Sin Noise
- https://x.com/XorDev/status/1731771853394292774

### Curl Noise
- https://glsl-curl-noise.vercel.app/
  - https://github.com/SahilK-027/glsl-curl-noise

- How to use it : https://www.linkedin.com/pulse/curl-noise-explorations-illugen-nicholas-seavert-svjve/?trackingId=buqesvXxiL19iBy8H5BYeA%3D%3D

### Various Noise in TSL
- https://threejsroadmap.com/blog/10-noise-functions-for-threejs-tsl-shaders
  - White, Value, Perlin, Simplex, Worley, FBM, Ridged, Wood/Marble, Curl, Domain Warping

### Misc
- Angular noise??? : https://x.com/cmzw_/status/1984240000477876540
- Electric Voronoi : https://0x7444ff-voronoi-electric-pattern.vercel.app/
  - https://github.com/SahilK-027/0x7444ff/tree/main/voronoi-electric-pattern
- Organic? : https://abstract-pattern-sk027.vercel.app/
  - https://github.com/SahilK-027/0x7444ff/tree/main/abstract-pattern
  - https://0x7444ff-organic-pattern.vercel.app/
    - https://github.com/SahilK-027/0x7444ff/tree/main/organic-pattern
- Topology? : https://0x7444ff-perlin-noise-advanced-abstract-pattern.vercel.app/
  - https://github.com/SahilK-027/0x7444ff/tree/main/perlin-noise-advanced-abstract-pattern
- Spectral Flow : https://0x7444ff-spectral-flow.vercel.app/
  - https://github.com/SahilK-027/0x7444ff/tree/main/spectral-flow
- Diamond Patterns : https://godotshaders.com/shader/animated-diamond-pattern/
- Cyclic noise : https://x.com/stormoid/status/2044475887920320555?s=20
  - https://www.shadertoy.com/view/fcjXzh

- Voronoi-diagram for optimal Gaussian Quantization (Lloyd-Max-GQ) : https://x.com/thomasahle/status/2049531010157629773

- Rainbow Noise: https://x.com/delaigrodela/status/2061030569190822337?s=20
