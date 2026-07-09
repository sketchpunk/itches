# Inverse Kinematics

### Great Info
- GDC Doom, Amazing lots of IK * Animation syncing ideas : https://www.youtube.com/watch?v=3lO1q8mQrrg
- "Cruse-rule gait" for procedural walking for 4 legs or more : https://www.youtube.com/watch?v=HjmIOKSp7v4&t=35s

### Godot
- https://godotengine.org/article/inverse-kinematics-returns-to-godot-4-6/

- SkeletonModifier3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/skeleton_modifier_3d.h#L37
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/skeleton_modifier_3d.cpp#L391

- LookAtModifier3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/LookAtModifier3D.xml#L2
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/look_at_modifier_3d.cpp
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/look_at_modifier_3d.h

- RetargetModifier3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/RetargetModifier3D.xml#L2
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/retarget_modifier_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/retarget_modifier_3d.cpp

- SpringBoneSimulator3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/SpringBoneSimulator3D.xml#L2
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/spring_bone_simulator_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/spring_bone_simulator_3d.cpp/

- BoneConstraint3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/BoneConstraint3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/bone_constraint_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/bone_constraint_3d.cpp

- AimModifier3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/AimModifier3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/aim_modifier_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/aim_modifier_3d.cpp

- ConvertTransformModifier3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/ConvertTransformModifier3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/convert_transform_modifier_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/convert_transform_modifier_3d.cpp

- CopyTransformModifier3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/CopyTransformModifier3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/copy_transform_modifier_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/copy_transform_modifier_3d.cpp

- IKModifier3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/IKModifier3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/ik_modifier_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/ik_modifier_3d.cpp

- TwoBoneIK3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/TwoBoneIK3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/two_bone_ik_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/two_bone_ik_3d.cpp

- ChainIK3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/ChainIK3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/chain_ik_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/chain_ik_3d.cpp

- SplineIK3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/SplineIK3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/spline_ik_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/spline_ik_3d.cpp

- IterateIK3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/IterateIK3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/iterate_ik_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/iterate_ik_3d.cpp

- FABRIK3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/FABRIK3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/fabr_ik_3d.cpp
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/fabr_ik_3d.h

- CCDIK3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/CCDIK3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/ccd_ik_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/ccd_ik_3d.cpp

- JacobianIK3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/JacobianIK3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/jacobian_ik_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/jacobian_ik_3d.cpp

- BoneTwistDisperser3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/BoneTwistDisperser3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/bone_twist_disperser_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/bone_twist_disperser_3d.cpp

- LimitAngularVelocityModifier3D
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/doc/classes/LimitAngularVelocityModifier3D.xml
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/limit_angular_velocity_modifier_3d.h
  - https://github.com/godotengine/godot/blob/5cb1ec590036fba44cdd8e727136ec6c25f11660/scene/3d/limit_angular_velocity_modifier_3d.cpp



### VRM
- Constraints (has code) - https://github.com/vrm-c/vrm-specification/tree/master/specification/VRMC_node_constraint-1.0
- SpringBone - https://vrm.dev/en/vrm1/springbone/

### UI 
- https://x.com/BurakKaraoglan4/status/1896909191903858903

### Cool IK Demos
- https://x.com/armorattack/status/1820823686879785177
- https://x.com/80Level/status/1821035916212785621
- https://x.com/ChristophSchadl/status/1821063356301644047
- https://x.com/cyanpuppets/status/1859080401790321027  // NICE SKELETON DESIGN
- https://x.com/onirenaud/status/1986367172017594741 SDF Particles with BVH

### CCD
- https://github.com/mrdoob/three.js/blob/dev/examples/jsm/animation/CCDIKSolver.js
- https://web.archive.org/web/20221206080850/https://sites.google.com/site/auraliusproject/ccd-algorithm

- With constraints - https://zalo.github.io/blog/inverse-kinematics/

### Spline IK in Maya
- https://x.com/cal4hike/status/1831325815814099383
- https://github.com/gaki131/maya_bifrost

### Interesting UI of IK
- https://x.com/WuotanStudios/status/1829111552210850145

### FABRIK
- Has hinge & ball constraints : https://github.com/upf-gti/IK-threejs
- Adds pole vector : https://github.com/upf-gti/IK-threejs/pull/3/commits/92796560d8b851cf06704b40fdf4601ecad2e729


### Closed Chained IK - Parallel Kinematrics Solver ( Hexapod )
- https://x.com/garrettkjohnson/status/1595253478707773441
- https://gkjohnson.github.io/closed-chain-ik-js/dist/hexapod.html
- https://github.com/gkjohnson/closed-chain-ik-js/blob/main/src/core/ChainSolver.js
- https://mathweb.ucsd.edu/~sbuss/ResearchWeb/ikmethods/iksurvey.pdf

### Auto Posing
- https://x.com/Cascadeur_soft/status/1823459674949345327


# Cool Demo of procedural spider walking in crazy angles
- https://x.com/keenanwoodall/status/1822031721296167186
- https://x.com/keenanwoodall/status/1822031723535696351
- https://x.com/keenanwoodall/status/1822441835450536085
- https://x.com/keenanwoodall/status/1121793645034631169
- https://x.com/keenanwoodall/status/1121793648364941312

# Interesting Cureling, Might be useful as a solver
- https://x.com/74WTungsteno/status/1819614402502443382


# Bone Springs? -- curves?
- https://x.com/paul_jarvis/status/1815131459344351684
- https://x.com/paul_jarvis/status/1815134869070168385

- https://github.com/akasaki1211/boneDynamicsNode
- https://x.com/akasaki1211/status/1843672590667395209

# Plane IK
- https://x.com/brave_rabbit/status/1836228649760034964
- https://braverabbit.gumroad.com/l/simpleIkSolverNodeGroup
- https://www.youtube.com/watch?v=kmFt4-SkKIo

# Heel Rigging
- https://x.com/GACCHI_3DCG/status/1836374612612891024

# Gaze Animation
- https://x.com/PolygonCherub/status/1837298407251013773
 - Additive angle. A look-at node. I store a WS location and just have the animation BP do a look at. I have all the bones from pelvis to head involved. Each with progressively more alpha to their rotation.
  
# Capsule overlay showing motion matching data
- https://x.com/RyanMuoio/status/1838686486084091908

# Awesome Hand Rig UI
- https://x.com/BlenderHub7/status/1842072481001099654

# Setup subchains in UE with the FBIK Node
- https://x.com/LincolnMargison/status/1853610984427905182
- https://www.youtube.com/watch?v=U0eVLm1attU&feature=youtu.be

### Cool poses
- https://x.com/geodraws_art/status/1837880171782934796

### Mechanical Wing Rig
- https://x.com/DemNikoArt/status/1856461011160600961

### Deformable Mesh
- https://x.com/cloudofoz/status/1870122139606524225
- https://github.com/cloudofoz/godot-deformablemesh


### Spline + Ring IK
- https://www.linkedin.com/posts/arturo-coso-aa814252_maya-rigging-techart-ugcPost-7294991065877467138-IY7o?utm_source=share&utm_medium=member_desktop
- https://arturocoso.gumroad.com/l/SplineWeights

### Mechanical Claw
- https://x.com/DemNikoArt/status/1893716301459124324
- https://www.youtube.com/watch?v=nyC57_HN6B0

### Laplacian Mesh And Animation Deformation
- https://www.youtube.com/watch?v=ZloIm02ZlAg
- https://www.linkedin.com/posts/jeromeeippers_animation-animation3d-numpy-activity-7299853598350278659-chIW?utm_source=share&utm_medium=member_desktop&rcm=ACoAABCBdyUBKZI3Bi-E7poUb5-kzZgKKi5j0RA

### Jiggle Physics in Godot ( Bone Springs )
- https://x.com/gamefromscratch/status/1899131462722470198
- https://gamefromscratch.com/godot-4-4-gets-jiggle-physics/
- https://www.youtube.com/watch?v=ClRH5HruUEQ&t=1s
- https://github.com/godotengine/godot/pull/101409

### Amazing Rig for Eyes
- https://x.com/ransom_vt/status/1899267129075257494

### Procedural hit Reaction
- https://www.youtube.com/watch?v=y_BLLSzCjd4&t=1s
- https://github.com/Vaei/ProcHitReact

### Interesting Arc
- https://x.com/Probiner/status/1912090991697277365
- https://x.com/FreyaHolmer/status/1626354308412317696?s=20

### IK With Quaternion Joint Limits
- http://number-none.com/product/IK%20with%20Quaternion%20Joint%20Limits/index.html

### Constraints
- https://x.com/makeshifted/status/1107917049051799553
- https://zalo.github.io/blog/constraints/

### Procedural Animation
- https://80.lv/articles/tutorial-procedural-spider-animation-in-unreal-engine-5/
- Climbing : https://x.com/DigitalOpus/status/1389266692782448646
- Walk Cycle : https://x.com/leedoppo/status/1389540103459123201

### Spring Bones
- https://en.wikipedia.org/wiki/Harmonic_oscillator#Damped_harmonic_oscillator
- https://codesandbox.io/p/sandbox/rough-fire-vpkg44?file=%2Fsrc%2FApp.js%3A4%2C29-4%2C42
- https://www.jsdelivr.com/package/npm/wiggle?tab=files&path=src
- https://github.com/skevy/wobble
- https://github.com/pavelbabenko/react-native-awesome-gallery/blob/5ab264db201379a3b6aa2e7b65c8018dc46b05bd/src/utils/withDecaySpring.ts#L82
- https://github.com/IAFahim/foundation/blob/fa9038b755d92f2c31ee8352107365bd23a30ceb/Assets/Heart/Modules/Component/Spring/SpringFloat.cs#L75

### Triangle Solver
- https://x.com/FreyaHolmer/status/1394406626229198858
- https://acegikmo.com/trianglesolver/

### Physical Walker using gait planner foot placement
The control is further shown to generalize across a variety of walking-related skills, including picking up objects placed at any height, lifting and walking with heavy crates, pushing and pulling crates, stepping over obstacles, ducking under obstacles, and climbing steps.
- https://x.com/DigitalOpus/status/1443621981375504397
- https://www.cs.ubc.ca/~van/papers/2010-TOG-gbwc/index.html
- https://www.youtube.com/watch?v=lOxeyyooDmw
- https://code.google.com/archive/p/cartwheel-3d/

### Foot Sliding Solutions
- https://x.com/sixthorns/status/1445096290174525441

### Auto Weight Painting
- https://x.com/scottpetrovic/status/1934283169294942463
- https://mesh2motion.org/news
- https://github.com/scottpetrovic/mesh2motion-app/

### Loop Animations
- https://x.com/anorangeduck/status/1572263286590279681
- https://theorangeduck.com/page/creating-looping-animations-motion-capture
- https://theorangeduck.com/media/uploads/Looping/looping.html

### Muscles
- https://x.com/80Level/status/1970450575612617092

### Face Rig
- https://x.com/sttuuuufffff/status/1964172439073570954

### Spline, CCD, Fabrik, Jacobian Godot
- https://github.com/godotengine/godot/pull/110120

### Jacobian
- https://www.youtube.com/watch?v=2_cdDGwnl80

### Spring Bone VRM
- https://github.com/vrm-c/vrm-specification/pull/496

### Rig Physics
- https://x.com/Cartesian_C/status/1960389845429215393

### Measuring Animations Speed
- https://x.com/meby_central/status/2008125473579221446

### Robotics
- https://www.linkedin.com/posts/ilir-aliu_17-faster-inverse-kinematics-in-pure-python-ugcPost-7422698105923395585-DjZh?utm_source=social_share_send&utm_medium=member_desktop_web&rcm=ACoAABCBdyUBKZI3Bi-E7poUb5-kzZgKKi5j0RA
  - https://github.com/chungmin99/pyroki
  - https://pyroki-toolkit.github.io/

- Mech arm Rig : https://www.youtube.com/watch?v=SCz1tmOVmFw

### MISC
- Procdural Turn : https://www.linkedin.com/posts/muhammad-kashif-ali-250487154_techanimstudios-unrealengine5-gamedev-activity-7420100618427707392-N6pH?utm_source=share&utm_medium=member_desktop&rcm=ACoAABCBdyUBKZI3Bi-E7poUb5-kzZgKKi5j0RA
- Procdural Avoidance : https://www.linkedin.com/posts/muhammad-kashif-ali-250487154_techanimstudio-unrealengine-gamedev-activity-7395025821750673408-SISM?utm_source=share&utm_medium=member_desktop&rcm=ACoAABCBdyUBKZI3Bi-E7poUb5-kzZgKKi5j0RA

- IK Run Cycle Path : https://x.com/HekiTen10/status/2025445284072087978?s=20
  - https://x.com/HekiTen10/status/2025921403070066858

- Stable Twist in IK Spline : https://dyncgi.wordpress.com/2026/02/23/en-ik-spline-twist-stable-without-flipping/

- AI to retarget Mixamo Animations : https://x.com/saori_xbt/status/2029623210812023175

- Cool looking tongue rig : https://x.com/jettelly/status/2032366052605378847

- Amazing Ragdoll Effect : https://x.com/Cartesian_C/status/1960389845429215393

- MMD IK : https://github.com/AmyangXYZ/reze-engine/blob/master/engine/src/ik-solver.ts

- IK Foot, Sliding fix, Grounded, locomotion ( Free unity plugin )
  - https://arkhipovdesign.itch.io/footwerk
  - https://jettelly.com/blog/footwerk-a-foot-placement-plugin-made-to-reduce-foot-sliding
  - https://www.youtube.com/watch?v=3SrBm_zbdLI

- Decomposed FABRIK : https://helpful-pudding-de25bb.netlify.app/
  - https://x.com/kiaran_ritchie/status/2069455535129367032?s=20

- Procedural Spider : https://github.com/majidmanzarpour/threejs-procedural-spider
