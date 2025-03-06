# Procedural Generation

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

### Planet Gen 
- https://dgreenheck.github.io/threejs-procedural-planets/
- https://x.com/dangreenheck/status/1854255756050121005
- Awesome Blender Procedural Planet : https://x.com/cmzw_/status/1865769276122231263

### Fracture Mesh ( intresting insights )
- https://youtu.be/O8brssfgtWc?si=rDoeJKucr6fmWtPQ

### Procedural Rock face terrain 
- https://x.com/bjornornorn/status/1861740021956436206
- https://x.com/bjornornorn/status/1861740563868913871
- https://x.com/bjornornorn/status/1861873026700132587
The rocks are based on a hexagonal grid and tiling 3d rock shapes (sorts of like voxels, but irregular). The 3d shapes are drawn with chamfers or cracks depending on what other rocks they connect to.

The rocks are hexagonal prisms with randomized heights. Vertices are added where they meet prisms in neighbouring columns. That base shape is then altered in various ways.

I’m creating the meshes this way directly. I decide how tall each rock is, then I use info about neighbouring heights to determine where to place vertices.


### Cool blender node to create terrain and clouds
- https://x.com/cmzw_/status/1867603773910323248

### Punch Out Model Synthesis / Breakout Model Synthesis - WFC Like Algo
- https://x.com/boris_brave/status/1866166898309648516
- https://zzyzek.github.io/PunchOutModelSynthesisPaper/
- https://github.com/zzyzek/PunchOutModelSynthesis