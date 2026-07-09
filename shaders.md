# Shaders

### Info / Tips
- https://mini.gmshaders.com/p/gm-shaders-mini-derivatives
- https://mini.gmshaders.com/p/gm-shaders-mini-fractal-texturing-1408552
  - https://x.com/XorDev/status/1911914119831118046
- Mirrored tiling is an easy way to make untileable textures tile
  - https://x.com/XorDev/status/1912237720220676345
  - uv = abs(mod(uv + 1.0, 2.0) - 1.0);
- LOTS OF Lighting, etc code: https://github.com/alienkitty/alien.js/tree/main/examples/three
- https://www.makingsoftware.com/chapters/shaders
- 14 Shader Techniques: https://x.com/XorDev/status/2021357513237495932
- ShaderToys like site: https://fragcoord.xyz/explore
- LOTS OF SHADERS : https://godotshaders.com/shader
- HEX Tiling : https://godotshaders.com/shader/stochastic-hex-tiling-mikkelsens-adaptation/
- https://tsl-docs.vercel.app/

### XOR
- https://mini.gmshaders.com/p/turbulence
  - It's a cheap, effective way to create fluidity without complicated formulas or resolution limitations
- https://mini.gmshaders.com/p/chaos
  - Chaos - Tiling / Layering / Spacing / Rotating
- https://mini.gmshaders.com/p/dot-noise
  - A cheap alternative to 3D simplex noise
- https://mini.gmshaders.com/p/gm-shaders-mini-fractal-texturing-1408552
  - Fractal Texturing to texture at any scale
- https://x.com/XorDev/status/1784054180186927536
  - fwidth outlines
- https://mini.gmshaders.com/p/volumetric
  - Volumetric Raymarching to create Glowing & Lighting Effects
- https://x.com/XorDev/status/2021363563173134628?s=20
  https://x.com/XorDev/status/1981417928302960666
  - This concept can even be used for depth of field effects:
  //Focus ratio should be small like 0.1 or 0.01
  float focus = abs(depth - focal_point) * focal_ratio;
  //Step through when out of focus
  step_dist = max(step_dist - focus, focus);
- Fast 3D pixel sorting: https://shadertoy.com/view/mdfyzl
- Antialiasing with derivatives: https://mini.gmshaders.com/p/antialiasing
- Blocky turbulence: https://x.com/XorDev/status/1975230424982183956
- Easy radial noise with normalized coordinates: snoise2D(normalize(p) * SCALE)

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

### Rigs with Glow
- https://github.com/SahilK-027/TPP-Orbit-Camera-Controller

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
- https://x.com/Tuatara_Games/status/2054969999719268359?s=20

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
- More Code in Comments : https://x.com/XorDev/status/2008979114544509285?s=20

### Phosphor
- https://mini.gmshaders.com/p/decoding-phosphor

### Jello
- https://x.com/alexanderchen/status/1990865914758070622?s=20
- https://aistudio.google.com/apps/bundled/vibecheck?showPreview=true&appParams=vibecheckcollectionBbQMXRGZwqxCirfzokN6&showAssistant=true

### Noise Depth Sphere
- https://x.com/cmzw_/status/1988223201009430657?s=20

### Depth Card
- https://x.com/cmzw_/status/1991161463273087369

### SDF Normals
- https://x.com/cmzw_/status/1988237431691489632
- https://iquilezles.org/articles/normalsSDF/

### infinite game of life
- https://x.com/jcponcemath/status/1992439382910087374
- https://oimo.io/works/life/
- https://github.com/saharan/works/tree/main/life

### Matcap generator
- https://x.com/ycwhk/status/1989585025566986673
- https://codepen.io/ycw/full/gbrMeXJ

### Jump Flood Outlines
- ScreenSpace SDF - https://x.com/nagakagachi/status/1987865976260763796
- https://bgolus.medium.com/the-quest-for-very-wide-outlines-ba82ed442cd9
- https://x.com/garrettkjohnson/status/1988450074318565774
- https://github.com/gkjohnson/three-jumpflood-demo

### 2D Fluid inside Sphere
- https://x.com/TheMirzaBeig/status/1711574005247819899
  - https://www.shadertoy.com/view/Ds3BRN

### Black Hole 
- https://x.com/dangreenheck/status/2008835472534151541
  - RayTracing : https://github.com/dgreenheck/webgpu-black-hole

### Stylized Mario Item Box
- https://x.com/jettelly/status/1982492419120910410

### Lens Flare
- https://github.com/ektogamat/lensflare-threejs-vanilla
- https://github.com/N8python/nektoFlare

### Ascii Render
- https://x.com/__rockbiter/status/1930205628162519526
  - https://www.youtube.com/watch?v=MIZbAO_rNWU&feature=youtu.be

### Painterly
- https://www.youtube.com/watch?v=7RJGttIYNrY

- https://www.reddit.com/r/Unity3D/comments/1tim92d/i_saw_a_painterly_shader_on_tiktok_and_tried_to/
  - https://github.com/tantaneity/painterly-urp

### Bump Color Noisey
- https://x.com/ycwhk/status/1984106944706310556
  - https://codepen.io/ycw/full/VYeGRqB

### Patterns
- Latvian : https://x.com/focru_ino/status/2033016010199199809
  - https://twigl.app/?ol=true&ss=-OnjRJNc7sNVIh-PgR75

### MISC
- Procedural Hex Grid : https://x.com/TheMirzaBeig/status/1731890067264688388
- Drip Shader : https://x.com/XorDev/status/2019209536352268572
- Soap Film : https://x.com/ekimroyrp/status/2021268795772297515
  - https://ekimroyrp.github.io/260208_SoapFilm/

- Flesh Like / Cellular Automata : https://x.com/thespite/status/2028539206612422986
  - https://spite.github.io/genuary-2026/9/
  - https://github.com/spite/genuary-2026/blob/main/9/main.js

- Hex Shield ( Awesome Scene ) : https://x.com/pmndrs/status/2041936585659453666
  - https://pmnd.rs/blog/creating-flow-shield/
  - https://pmndrs.github.io/examples/flow-shield/

- Nebula : https://www.motion-gpu.dev/playground?demo=nebula

- Neon Liquid Fluid / Energy, REALLY COOL : https://x.com/sabosugi/status/2043303971654410636
  - https://codepen.io/sabosugi/full/XJjypjm

- Oil Paint : https://x.com/yutorikoubo/status/2043832918750159035
  - https://x.com/yutorikoubo/status/2043592899078877336
  - https://x.com/yutorikoubo/status/2043619753206636939

- Colored crystal cube : https://github.com/jeantimex/cmy-cube

- Interior Mapping : https://x.com/codedgar_dev/status/2058794218613543284
  - https://github.com/codedgar/three-fenestra
  - https://three-fenestra.codedgar.com/
  - https://github.com/emirhanyener/three-interior-plane
  - https://threetag.com/three-plane-interior/

 - Rainbow God Rays, Like NMS portaling scene
   - https://x.com/sabosugi/status/2063530026361135225
   - https://codepen.io/sabosugi/full/OPbrMKz

 - Amazing Parallax Mapping Effect to raise Tiles / Iterative parallax mapping
   - https://www.reddit.com/r/godot/comments/1u9sbwv/parallax_mapping_rules/
   - https://godotshaders.com/shader/iterative-parallax-mapping/
