# modelos
Modelos 3D GLTF

```
	var modelMatrix = Cesium.Transforms.eastNorthUpToFixedFrame(
		Cesium.Cartesian3.fromDegrees(-48.62898254394531, -24.02804946899414, 500.0));
		
	var model = scene.primitives.add(Cesium.Model.fromGltf({
		url : '/models/ah-64_helicopter/scene.gltf',
		modelMatrix : modelMatrix,
		scale : 20.0
	}));	
	
	Cesium.when( model.readyPromise ).then( function( model ) {
		model.activeAnimations.addAll({
			loop : Cesium.ModelAnimationLoop.REPEAT
		});
	});
  
```
