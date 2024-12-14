# Documentation

Introduction 
Element five switches between 2 scences,

The scene does not contain much simply a few object of various colours that are created textured and coloured
the camera is placed in the center an can arc rotate around it

clicking the buttons displays the scene whilst keeping the menu buttons on screen 

I tried to add a skybox to it but was having trouble with referenceing the assets from within the scecific scene

Create Ground from createStartScene.ts

```Javascript
Js
 function createGround(scene: Scene) {
    let ground = MeshBuilder.CreateGround(
      "ground",
      { width: 6, height: 6 },
      scene,
      
    );
    var groundMaterial = new StandardMaterial("groundMaterial", scene);
    groundMaterial.backFaceCulling = false;
    ground.material = groundMaterial;
    groundMaterial.diffuseColor = new Color3(0.1, 1, 0.5);
    return ground;
  }
```
this code creates the mesh gives it a material and sets its colour to a light green

the Texture for the cylinder stopped working in the build but can be seen in the Bablylon proj repository