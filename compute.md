# Compute

### InstancedMesh, node material, compute shaders and psrdnoise
- https://x.com/soju22/status/1856342359954387226
- https://threejs-webgpu-test.netlify.app/
- https://github.com/klevron/test-webgpu
fn rotationXYZ(euler:vec3<f32>) -> mat3x3<f32> {
  let a = cos(euler.x); let b = sin(euler.x);
  let c = cos(euler.y); let d = sin(euler.y);
  let e = cos(euler.z); let f = sin(euler.z);
  let ae = a * e; let af = a * f; let be = b * e; let bf = b * f;
  return mat3x3<f32>(
    vec3<f32>(c * e, af + be * d, bf - ae * d),
    vec3<f32>(-c * f, ae - bf * d, be + af * d),
    vec3<f32>(d, -b * c, a * c)
  );
}
fn compose(pos: vec3<f32>, rmat: mat3x3<f32>, scale: vec3<f32>) -> mat4x4<f32> {
	return mat4x4<f32>(
    rmat[0][0] * scale.x, rmat[0][1] * scale.x, rmat[0][2] * scale.x, 0.,
    rmat[1][0] * scale.y, rmat[1][1] * scale.y, rmat[1][2] * scale.y, 0.,
    rmat[2][0] * scale.z, rmat[2][1] * scale.z, rmat[2][2] * scale.z, 0.,
    pos.x, pos.y, pos.z, 1.
  );
}
fn lookAt(direction: vec3<f32>, up: vec3<f32>) -> mat3x3<f32> {
	var direction_var = direction;
	if (direction_var.x * direction_var.x + direction_var.y * direction_var.y + direction_var.z * direction_var.z == 0.) {
		direction_var.z = 1.;
	}
	direction_var = normalize(direction_var);
	var x: vec3<f32> = cross(up, direction_var);
	if (x.x * x.x + x.y * x.y + x.z * x.z == 0.) {
		if (abs(up.z) == 1.) {
			direction_var.x = direction_var.x + (0.0001);
		} else { 
			direction_var.z = direction_var.z + (0.0001);
		}
		x = cross(up, direction_var);
	}
	x = normalize(x);
	return mat3x3<f32>(x, cross(direction_var, x), direction_var);
}