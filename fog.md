# Fog

### Fake Volumetric fog
- https://x.com/3eyes_iii/status/1846089734444974178
- https://x.com/thefrontendcat/status/1846940102213120266 Radius fog
- https://www.artstation.com/blogs/lisavettas/1A1W/fake-volumetric-fog-tricks-for-ue4
- https://stackoverflow.com/questions/21549456/how-to-implement-a-ground-fog-glsl-shader
- https://stackoverflow.com/questions/45783444/glsl-spotlight-projection-volume
- https://shahriyarshahrabi.medium.com/interactive-volumetric-fog-with-fluid-dynamics-and-arbitrary-boundaries-f82fdee86397
- !!!! https://stackoverflow.com/questions/21549456/how-to-implement-a-ground-fog-glsl-shader  
- https://www.terathon.com/lengyel/Lengyel-UnifiedFog.pdf
- !!!! https://www.youtube.com/watch?v=k1zGz55EqfU

### Volumetric Fog
- https://github.com/godotengine/godot/blob/970be7afdc111ccc7459d7ef3560de70e6d08c80/servers/rendering/renderer_rd/shaders/environment/volumetric_fog.glsl#L201-L206
- https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@14.0/manual/fog-volume-shader.html


https://x.com/iced_coffee_dev/status/1864688637520036203
This one is the same fog equation I sent you a while back, the crytek one. Then all I did was calculate an AABB intersection, use that to figure out the depth of the fog. Make sure to take a min between that and the scene's depth. Then I took a couple noise samples along that vector, starting at the AABB's near intersection, and fed that into the fog equation.

https://x.com/iced_coffee_dev/status/1846926132731408744
- https://advances.realtimerendering.com/s2006/Chapter6-Real-time%20Atmospheric%20Effects%20in%20Games.pdf
float ComputeVolumetricFog( in float3 worldPos, in float3 cameraToWorldPos) { 
    // NOTE: cVolFogHeightDensityAtViewer = exp( -cHeightFalloff * vfViewPos.z ); 
    float fogInt = length( cameraToWorldPos ) * 
    cVolFogHeightDensityAtViewer; 
    const float cSlopeThreshold = 0.01;

    if( abs( cameraToWorldPos.z ) > cSlopeThreshold ){ 
        float t = cHeightFalloff * cameraToWorldPos.z; 
        fogInt *= ( 1.0 - exp( -t ) ) / t; 
    }

    return exp( -cGlobalDensity * fogInt ); 
}