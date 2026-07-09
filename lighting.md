# Lightning

### Joyce newer Metal Toon Shader
- https://x.com/minionsart/status/1829904147690209784
- https://www.youtube.com/watch?v=ttVEvYQ7X5A&feature=youtu.be

### Nice looking Sketchy Toon Energy Shader
- https://x.com/TheMirzaBeig/status/1829095710198747323
- https://x.com/KasperArnklit/status/1828546764397494353

### Nice lighting with fresnel
- https://x.com/HarryAlisavakis/status/1828069724082553245

### Ambient Occlusion
- https://x.com/XorDev/status/1821024532511019480
- https://x.com/XorDev/status/1820886173839159381
- https://x.com/XorDev/status/1821051533598785581

### NPR Shaders
- https://typhomnt.github.io/post/blender_npr/

### Global illumination
- Radiance Cascades https://x.com/yaazarai/status/1818903149975159173
  - https://github.com/Yaazarai/GMShaders-Radiance-Cascades

- bilateral blur, runs better on IPAD or low devices
  - https://x.com/Ademola_4life/status/2002826156819816701
  - https://p25pd9.csb.app/
  - https://gist.github.com/ademola-lou/8fcd19bf081ff9cafd31f6ce1781c59d
  - https://codesandbox.io/p/sandbox/p25pd9?file=%2Findex.html%3A26%2C20

### Quantized lights
- https://x.com/TheMirzaBeig/status/1818539915728072789
```
RdotV (specular), quantized before applying light colour.
round(dot(norm, lightDir) * x) / x;
round(dot(reflect(-lightDir, norm), viewDir) * x) / x;
(x = resolution, or steps)
```

### Sub Surface Scatering - Flesh
- https://x.com/3dflashlo/status/1724478698429067483
- https://lo-th.github.io/three.lab/examples/#webgl_materials_sss
- https://github.com/lo-th/three.lab/blob/main/examples/webgl_materials_sss.html

### GTAO, Screenspace AO
- https://cdrinmatane.github.io/posts/ssaovb-code/
- https://x.com/Cody_J_Bennett/status/1815338863243538585
- https://x.com/Cody_J_Bennett/status/1815370071365034426

### SAO
- https://lo-th.github.io/root/sao/
  - https://github.com/lo-th/root/tree/gh-pages/sao

### Cluster Lighting
- https://x.com/shawn03261/status/1792924248790499430
- https://uinosoft.github.io/t3d.js/examples/#renderer_clustered_lighting

### PBR
- https://www.youtube.com/watch?v=IjwL_pTAxWw
- Clear Coat : https://www.youtube.com/watch?v=KONdF3WEXa0

### Cheaper PBR
- https://community.arm.com/cfs-file/__key/communityserver-blogs-components-weblogfiles/00-00-00-20-66/siggraph2015_2D00_mmg_2D00_renaldas_2D00_slides.pdf

### Gamma Correction
- https://x.com/XorDev/status/1882941307683045593
- https://mini.gmshaders.com/p/gamma
- https://x.com/XorDev/status/1882938478834671837

### Polyhedral Lights
- https://bastian.urbach.one/rtswplusd/
- https://x.com/BastianUrbach/status/1420292802982907907

### Light Cookie with Cloud & Tree Shadows
- https://x.com/minionsart/status/1715019567041233319
- https://www.patreon.com/posts/animated-light-38047499
- https://www.patreon.com/posts/animated-light-88618240

### Fresnel
- https://x.com/OtanoStudio/status/1737980462910333406
- https://fresnel-shader-material.vercel.app/
- https://github.com/OtanoStudio/Fresnel-Shader-Material

### Fake Glow material into FakeVolumetricMaterial
- https://github.com/ektogamat/fake-glow-material-r3f
- https://x.com/Andersonmancini/status/1756041166259134726

### Reflective Shadow Maps Global Illumination
- https://github.com/ademola-lou/RSMGI
- https://x.com/Ademola_4life/status/1932222317737689452?t=8OMf2nMG2z8W2QWLHCs4MQ&s=03
- Has a 3mb sponza level & a grid textured level

### Fast GGX-Based convolution for glossy reflection probs
- https://x.com/guitio2002/status/1960758324275613898

### Lighting with Sparks, Rim, Reflections, Stencil and Parallax
- https://x.com/bobacupcake/status/1986931909717286933
- https://bobacupcake.com/shader-basics

### Area Lights
- Rect, Tube, Sphere : https://alextardif.com/arealights.html

### PBR
- https://gnikoloff.github.io/webgl-pbr-dojo/
  - https://github.com/gnikoloff/webgl-pbr-dojo

### Screen Space SS
- https://x.com/Ademola_4life/status/2003554430428545232
  - https://7hj567.csb.app/
  - https://codesandbox.io/p/sandbox/7hj567

### Radiance Cascades (SPWI)
- https://x.com/Cody_J_Bennett/status/2025156053323690276
- https://martinfullerblog.wordpress.com/2023/01/13/min-max-buffer-precision-improvement/
- https://x.com/Cody_J_Bennett/status/2024626414947865002
- https://jcgt.org/published/0003/02/01/paper.pdf
- https://pbr-book.org/4ed/Geometry_and_Transformations/Spherical_Geometry#x3-Equal-AreaMapping

### Misc
- Global Illumination : https://jason.today/gi
- Radiance Cascades : https://jason.today/rc
- https://lisyarus.github.io/blog/posts/a-silly-diffuse-shading-model.html
- Toon : https://lo-th.github.io/root/toon/
  - https://github.com/lo-th/root/tree/gh-pages/toon
- Fake Glass : https://x.com/Youssef_Afella/status/2020632755399213068
  - https://github.com/Youssef-Afella/UnityURP-FakeRealGlass
- Spherical Gaussians - https://x.com/bjornornorn/status/2021599470622814281
  - https://x.com/bjornornorn/status/2021599473479078323
  - https://www.shadertoy.com/view/WX3fRB
- Surface Stable Fractal Dithering : https://www.youtube.com/watch?v=HPqGaIMVuLs
  - https://github.com/runevision/Dither3D
- Real-Time Dynamic Environment Maps / Holy Donut Technique
  - https://dev.to/peter3riding/real-time-dynamic-environment-maps-in-threejs-the-holy-donut-technique-explained-2796
- Subsurface Scattering : https://github.com/N8python/subsurfaceScatteringMat

- NICE - Callisto Protocol Light Model : https://godotshaders.com/shader/proxima-ggx-the-callisto-protocol-light-model/

- NICE - UCBC’s Stylized Light : https://godotshaders.com/shader/ucbcs-stylized-light-using-a-mask/

- GGX Light Model - https://godotshaders.com/shader/circle-mask/

- Translucent Glassy Jelly Plasticy
  - https://github.com/pmndrs/drei/blob/master/src/core/MeshTransmissionMaterial.tsx
  - https://x.com/0xca0a/status/1611390751488737282

- Specular Models : https://x.com/ushadersbible/status/2043948669083263213\
  - Phong, Binn-Phong, Ashikhmin–Shirley, GGX

- Awesome Comic book Shader : https://www.youtube.com/watch?v=Ctx1TP0XDUM

- LUT : https://x.com/andreeliasdev/status/2053906095857398158
  - Look Up Table
  - Day/Night Systems: Changing the overall color palette smoothly as time passes.
  - Cinematic Effects: Applying a specific movie-like color grade.
  - Atmosphere: Enhancing scenes with, for example, a cold blue tint for snowy areas or a warm, saturated look for sunny, tropical environments

- Khronos PBR Neutral Tonemapper : https://dev.epicgames.com/community/learning/tutorials/pYEM/unreal-engine-using-khronos-pbr-neutral-as-a-custom-replace-tonemapper-in-ue5

- volumetrics using ray-extensions and Holographic Radiance Cascades: https://github.com/Yaazarai/Volumetric-HRC

- iterative parallax mapping ( cheaper to parallax occlusion mappng )
  - https://www.reddit.com/r/godot/comments/1twtuqd/iterative_parallax_mapping_cheaper_alternative_to/ 
  - https://godotshaders.com/shader/iterative-parallax-mapping/

- Depth, Shader, Reconstruction - https://www.cyanilux.com/tutorials/depth/#orthographic-scene-depth
