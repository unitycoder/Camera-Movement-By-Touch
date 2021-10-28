# Camera-Movement-By-Touch

## Table of contents
* Description
* Parameters
* Features

## Description
Scripts: 
* PanPinchCameraMovement.cs  
* TapOnGameObject.cs

#### Used for the camera movement in 2D space that is attached to any gameObject.
#### Used for detecting tap on gameObjects with a Collider attached. [COLLIDER MUST BE ATTACHED TO GAMEOBJECT]

## Parameters
---
PanPinchCameraMovement.cs 
* Camera To Move --> Camera component of the object that you want to move 

* X inferior limit --> the minim x value for the camera position [camera position is the center of the view]

* X superior limit --> the maximum x value for the camera position

* Y inferior limit 

* Y superior limit

* Minimum ortho size --> the minim ortho size of the camera that has the "Projection" in Orthographic mode

* Maximum ortho size --> the maximum ortho size

* Interpolation step for inertia [0.2 recommended]

---
TapOnGameObject.cs
* Sensitivity --> the sensitivity of Touch.deltaPosition to consider it in the Moved phase


## Features

* Panning with one finger in any direction with finger remaining always under the touched object [also know as pixel perfect panning]

* Panning has inertia
    
* Pinching with two or more fingers with zooming target in the middle point of the two fingers

* Visual feedback for achieving minimum ortho 

* Supports panning during the pinching operation

* WorldSpace limits and orthographic limits

* Ignores any UI elements during touch operation
    
* Static bool MovingCamera with tolerance to know when camera is moving by touch

* Gizmo drawing in UNITY EDITOR to know the limits of the camera 

* Detects tap on GameObjects for opening screens or panels [UI canvas]