# Procedural Generation

### Node Systems
- https://github.com/protongraph/protongraph

### WFC Island Generator with triangle tiles
- https://github.com/Pierre-Terdiman/WFC_Explorer
- https://x.com/PierreTerdiman/status/1935047242135519607

### General Dual Grid Examples
- https://x.com/bjornornorn/status/1855971006482968714

### Surface Nets and Trilinear Mapping
- https://bonsairobo.medium.com/smooth-voxel-mapping-a-technical-deep-dive-on-real-time-surface-nets-and-texturing-ef06d0f8ca14

### Soda Can
- https://x.com/PavelBoytchev/status/1808130140859232716
- https://boytchev.github.io/3d-assets/online/drink-can.html

### Step terrain
- https://x.com/ULuIQ12/status/1815787696519868852
- https://x.com/ULuIQ12/status/1814350230478901607
- https://github.com/ULuIQ12/webgpu-isoline-geometry

### City Gen
- https://x.com/gnomeslair/status/1809611392028406149
- https://zero.re/worldsmith/roadnet/

### Spline Meshes
- https://x.com/_staggart_/status/1833494496178540558
- https://pastebin.com/u/Staggart/1/gRKibMc1

### Planet Gen
- https://x.com/flobit_dev/status/1835782921812169075
- https://github.com/flo-bit/flo-bit.github.io
- https://github.com/flo-bit/tiny-planets/

### Mesh Line
- https://x.com/makio64/status/1963160279795065084
  - https://meshline.makio.io/
  - https://github.com/Makio64/makio-meshline

### Surface Nets
- https://bonsairobo.medium.com/smooth-voxel-mapping-a-technical-deep-dive-on-real-time-surface-nets-and-texturing-ef06d0f8ca14
- https://x.com/teamldm/status/1896211283718111287

- SDFs to Mesh. Small Code: https://github.com/bonsairobo/fast-surface-nets-rs

- Terrain Gen : https://github.com/EthanHermsey/Nature 

### Turn quad into circle, cone or cylinder
- https://x.com/TheMirzaBeig/status/1828047197738344724
```
float theta = uv.x * 2PI; 

float x = radius * cos(theta); 
float z = radius * sin(theta); 

float radialDistance = 1.0 - (uv.y * pinch);

x *= radialDistance;
z *= radialDistance;

return float3(x, position.y * height, z);
```

### Dual Grids
- https://github.com/pablogila/TileMapDual_godot_node/

### Curved Worlds
- https://www.youtube.com/watch?v=f8O-AmYkLRQ
- https://assetstore.unity.com/packages/vfx/shaders/curved-world-173251?aid=1101l96nj&pubref=rev_curvedworlds
- https://youtu.be/GOYwMPZHaUo?si=L8BGdoRVUE2GJQSk

### Octahedral impostors / hemispherical
- https://x.com/OskSta/status/1849427564034498642
- https://docs.google.com/document/d/17zSUKMpe8sVPJ3fy2lI7T0ct3tTMCKfekgtdx8UFBbU/edit?tab=t.0#heading=h.bsht5cb6u0ur
- https://madarapremawardana.medium.com/the-only-imposter-who-come-in-handy-octahedral-imposters-e2b002379a98
- https://shaderbits.com/blog/octahedral-impostors
- https://gamedev.stackexchange.com/questions/169508/octahedral-impostors-octahedral-mapping

- https://x.com/BrianBreiholz/status/1905759745706758198
- https://github.com/Ctrlmonster/three-octahedral-impostor/

### Planet Gen 
- https://dgreenheck.github.io/threejs-procedural-planets/
- https://x.com/dangreenheck/status/1854255756050121005
- Awesome Blender Procedural Planet : https://x.com/cmzw_/status/1865769276122231263

### Procedural Trees
- https://www.eztree.dev/
- https://github.com/dgreenheck/ez-tree

### Fracture Mesh ( intresting insights )
- https://youtu.be/O8brssfgtWc?si=rDoeJKucr6fmWtPQ

### Procedural Rock face terrain 
- https://x.com/bjornornorn/status/1861740021956436206
- https://x.com/bjornornorn/status/1861740563868913871
- https://x.com/bjornornorn/status/1861873026700132587
- https://x.com/bjornornorn/status/1771468544879788313
The rocks are based on a hexagonal grid and tiling 3d rock shapes (sorts of like voxels, but irregular). The 3d shapes are drawn with chamfers or cracks depending on what other rocks they connect to.

The rocks are hexagonal prisms with randomized heights. Vertices are added where they meet prisms in neighbouring columns. That base shape is then altered in various ways.

Horizontally I have a hexagonal grid. Per hexagon I store a list of where ground begins and ends.
This is combined with a tiling 3d "rock structure", which encodes what shape rocks have. The rock structure looks a bit like a 3d-voronoi diagram. I combine the two by traversing the hexagonal height information and cutting rocks to the appropriate height and if neighbouring columns have similar heights, I merge them to form grass.

I’m creating the meshes this way directly. I decide how tall each rock is, then I use info about neighbouring heights to determine where to place vertices.

The terrain itself here is on a fixed hexagonal grid. I’m editing the terrain with some tools to shape it, to add rock and to smoothen it. On top of this a mesh/grid is updated to align with the heighfield slope/curvature. This will be used for buildings/structures.

- Texture Details : https://x.com/bjornornorn/status/2042322126263185501

- Adapting Grid over terrain : https://x.com/bjornornorn/status/1799070308705636702?s=20
  - https://x.com/bjornornorn/status/1798991352136671422?s=20 
  - https://x.com/bjornornorn/status/1798344289677889964
  - https://x.com/bjornornorn/status/1781379998047158333
  - https://x.com/bjornornorn/status/1536414013176832001?s=20

- Island & Cave Gen : https://x.com/bjornornorn/status/1581277292097310720
  - https://x.com/bjornornorn/status/1570120470002896901 
  - https://x.com/bjornornorn/status/1530135558793707520?s=20
  - https://x.com/bjornornorn/status/1525092887008100352?s=20
  - https://x.com/bjornornorn/status/1525092918297612293?s=20

### Cool blender node to create terrain and clouds
- https://x.com/cmzw_/status/1867603773910323248

### Punch Out Model Synthesis / Breakout Model Synthesis - WFC Like Algo
- https://x.com/boris_brave/status/1866166898309648516
- https://zzyzek.github.io/PunchOutModelSynthesisPaper/
- https://github.com/zzyzek/PunchOutModelSynthesis

### Irregular Grids with a Grid
- https://x.com/jakubtomsu_/status/1902122605961695548
- https://x.com/jakubtomsu_/status/1902406237091766590

### Minecraft / Voxels
- https://www.youtube.com/watch?v=tsOTCn0nROI
- https://github.com/dgreenheck/minecraft-threejs-clone

### Model Synthesis / Wave function collapse WFC
- https://www.boristhebrave.com/2021/10/26/model-synthesis-and-modifying-in-blocks/
- https://www.boristhebrave.com/2020/04/13/wave-function-collapse-explained/

### Marching Cubes / Squares
- asymptotic decider : https://x.com/boris_brave/status/1478042985719861255
  - https://www.boristhebrave.com/2022/01/03/resolving-ambiguities-in-marching-squares/

- https://lo-th.github.io/root/isosurface/
  - https://github.com/lo-th/root/tree/gh-pages/isosurface
  - Native Surface Nets, Matching Tetraheda, Marching Cubes

### Maze Generator
- https://x.com/CasualEffects/status/957520581527855104
  - https://github.com/morgan3d/misc/blob/master/jsmaze/maze.js
  - VERY AWSOME https://morgan3d.github.io/misc/jsmaze/index.html

### Island
- https://x.com/bjornornorn/status/1581277292097310720

### Cave Generator
- https://www.boristhebrave.com/2023/11/19/how-does-cave-glade-generator-work/

### Hex Rocks
- https://80.lv/articles/building-a-columnar-rock-tool-with-houdini-unreal-engine

### Scrolling Cracked floor
- https://x.com/ycwhk/status/1987661595389067700
- https://codepen.io/ycw/full/PwNYqxE

### Lizard Walk
- https://x.com/jettelly/status/1986494144110600663

### Floor Plan
- https://github.com/OndrejNepozitek/Edgar-DotNet

### Geometry Nodes
- https://x.com/repalash/status/2036874338302124463
  - https://threepipe.org/examples/

### Volumetric lines
- Cubes & Spheres : https://web.archive.org/web/20150930205745/http://sebastien.hillaire.free.fr/index.php?option=com_content&view=article&id=54&Itemid=56
- https://web.archive.org/web/20111202022753/http://sebastien.hillaire.free.fr/index.php?option=com_content&view=article&id=57&Itemid=74
- https://sebh.github.io/projects/

### MISC
- City : https://x.com/thespite/status/2025276497263481026
  - https://spite.github.io/genuary-2026/8/
  - https://github.com/spite/genuary-2026/blob/main/8/main.js
- GPU Runtime Placement : https://www.youtube.com/watch?v=ToCozpl1sYY

- Road Data Structures : https://x.com/SandboxSpirit/status/2033975809443041773
  - https://sandboxspirit.com/blog/data-structures-of-roads

- Cave System ( SDF Lerp & Marching Squares ) : https://x.com/Nodragem/status/2034613234406236561

- Lightening Bolts VFX ( cracks, sparks, flash )
  - https://x.com/SahilK027/status/2037143354530738380
  - https://github.com/SahilK-027/Lightning-VFX
  - https://lightning-vfx.vercel.app/

- Island VERY CUTE + AWESOME : https://omma.build/community/tg5ezx5k4dxt

- City Cellular Automata : https://x.com/daturascore/status/2041165443084300353
  - https://github.com/Daturascore/genovae
  - https://objkt.com/tokens/KT1MR2NMrKmyoA6CLFN9LDGkMeHBfyb4jMRx/4?ref=tz1KuuVzzXCrBrZ3tPbWGTs9Aj54NR1Vn5dC

- Line Mesh / MeshLine : https://github.com/Makio64/makio-meshline
  - https://meshline-demo.makio.io/examples/laser-heist

- Gen Rock with Splines & special Stochastic Triplanar
  - https://x.com/Toyojiro3619/status/2063492948684390498?s=20

- Infinite Terrain, Grass & Sky : https://github.com/brunosimon/infinite-world

- Water, Terrain, Sky, Clouds, Atmosphere: https://x.com/scottstts/status/2068732637536010439
  - https://github.com/scottstts/Threejs-Awesome-Graphics-Agent-Skills

- Planet Generator : https://x.com/SkyeSharkie/status/2073455891194806689
  - https://github.com/SkyeShark/SeedThree 

- Awesome Building Generator : https://x.com/chirovisuals/status/2074135400138830228?s=20
  - https://github.com/achrefelouafi/BuildingGeneratorThreeJS
