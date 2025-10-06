# Shaders

### Info / Tips
- https://mini.gmshaders.com/p/gm-shaders-mini-derivatives
- https://mini.gmshaders.com/p/gm-shaders-mini-fractal-texturing-1408552
  - https://x.com/XorDev/status/1911914119831118046
- Mirrored tiling is an easy way to make untileable textures tile
  - https://x.com/XorDev/status/1912237720220676345
  - uv = abs(mod(uv + 1.0, 2.0) - 1.0);
- LOTS OF Lighting, etc code: https://github.com/alienkitty/alien.js/tree/main/examples/three

### Collections 
- https://sketches.isaacmason.com/sketch/intro
- https://github.com/brunosimon/three.js-tsl-sandbox
- https://github.com/gdquest-demos/godot-shaders
- https://github.com/paper-design/shaders
  - https://x.com/sdothaney/status/1882113262092976634
- https://shadergpt.14islands.com/explore
- https://www.xordev.com/arsenal
- https://threejsresources.com/tool/cosmic-texture-browser

### Crazy Curvey Grid - Escher grid visualizer
- https://x.com/unconed/status/1833618881799131352
- https://gitlab.com/unconed/use.gpu/-/blob/master/packages/app/src/pages/shader/droste.tsx
- https://usegpu.live/demo/shader/droste

### Toon Gem
- https://x.com/AcarcaneCG/status/1894942321109786674
- https://www.youtube.com/watch?v=mQPFjzAgGQo

### MaterialX
- GLSL Bits : https://github.com/AcademySoftwareFoundation/MaterialX/tree/main/libraries/pbrlib/genglsl

### UV Scale & Rotation
- https://x.com/Tuatara_Games/status/1905318904244867140

### Turbulence ( Liquid or Fire Effects )
- https://mini.gmshaders.com/p/turbulence
- https://x.com/XorDev/status/1901753484233343116
- Ink: https://shadertoy.com/view/WclSWn
- Flames: https://shadertoy.com/view/wffXDr
- Basic Code : https://x.com/XorDev/status/1902739410568810908

### Coordinate
- UV on Resolution : https://x.com/XorDev/status/1958578168115163319

### Blur with Gamma Correct Lights
- https://x.com/XorDev/status/1882941821388792027
- https://www.shadertoy.com/view/XXyBRR

### Simple toon Shader
- https://www.linkedin.com/posts/mirzabeig_gamedev-vfx-realtimevfx-activity-7283091088498683905-d1Io?utm_source=social_share_sheet&utm_medium=member_desktop_web

### Car Paint Blender
- https://x.com/thomas__marcos/status/1885353626224263443

### Stripe Pattern
- https://x.com/Zxyowo/status/1894721102187757775

### Crystaline Effect
- https://x.com/VoXeloStudio/status/1902973442632327506
- https://codepen.io/VoXelo/full/RNwMgJY

### Awesome nebulus cloud
- https://www.shadertoy.com/view/MsVXWW

### Dissolve
- https://x.com/CantBeFaraz/status/1678007542817882112
- https://codesandbox.io/p/sandbox/green-resonance-5fgz3d

### Screen Blending Addtitive without overexposure
- https://x.com/XorDev/status/1912255691483664654
- col.rgb = col.rgb + TINT - col.rgb * TINT;
- col.rgb = 1.0 - sqrt((1.0-col.rgb) * (1.0-TINT));
- https://x.com/XorDev/status/1781339718610821426
- A + B  or A + B - A * B;
- https://www.shadertoy.com/view/4c3SRH
- screen2(a,b) = a+b - sqrt(a*b) // sum - geometric mean
- ( screen2(a,a) = a, while screen(a,a) = 2a-a**2 )

### Wrinkle Shader
- https://bbbn19.gumroad.com/l/xxroj

### Real-ish flame
- https://x.com/cmzw_/status/1912515524078247958
- https://x.com/cmzw_/status/1912538189010739688

### Depth of Field
- https://x.com/turanszkij/status/1404746068651294720

### UV Distortion
- https://x.com/Tuatara_Games/status/1961126642568630404

### Mood Phase Shader
- https://x.com/flogelz/status/1476285518396669954

### Noise to make lots of eyes
- https://x.com/iced_coffee_dev/status/1580217793756426240

### Spiral
- https://x.com/cmzw_/status/1716776953959854203

### Pixel Water
- https://x.com/cmzw_/status/1721843939941183692

### Custom Toon Shader
- https://x.com/erbukev/status/1971611963328520605
- https://www.moddb.com/tutorials/tf2-shading-in-ut3

### Height Blend Textures
- https://passivestar.xyz/posts/simple-height-blend-shader/

### TSL Vignette
- https://x.com/thenoumenon/status/1967962195989250052/photo/1

### Turbulence
- https://mini.gmshaders.com/p/turbulence

### Phosphor
- https://mini.gmshaders.com/p/decoding-phosphor