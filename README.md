# ProcessingLite

This mini-project aims to recreate some basic processing functions in Unity3D, using a single drag and drop file.

This is made for Unity3D version 2020.2 or newer but is largely untested (It uses C# v8 stuff).


## Useage
1. Download the ProcessingLite.cs file.
2. Drag and drop the ProcessingLite.cs file into your unity project.
3. Change inherence from the class MonoBehaviour to ProcessingLite.  
   (You will still have all MonoBehaviour functionality).
4. Use the supported commands in Start or Update.

> *Please note that origin will be placed at the bottom left corner (In Processing, it's in the top left corner).*


## Supported Commands
All these commands might not have full support (Example: rounded corners on rectangles). The base version of these commands should work.

[Processing documentation](https://processing.org/reference/)

#### Environment
- Height
- Width

#### Shape
- Attributes
  - StrokeWeight()
- Vertex
  - BeginShape()
  - EndShape()
  - Vertex()
- 2D primitives
  - Circle()
  - Ellipse()
  - Line()
  - Point()
  - Quad()
  - Rect()
  - Square()
  - Triangle()

#### Color
- Background()
- Fill()
- NoFill()  
- NoStroke()
- Stroke()


## Features covered by Unity
Some features from Processing will not be ported over since the already exist in Unity.

- Data
- Input
- Transform
- Math and Constants
- PVector


## Test Code
In Unity, create a class called `Test`.
Change the inheritance from MonoBehaviour to ProcessingLite.GP21
Run the program. If you see the word _Hi_, then it's working.

```CS
using UnityEngine;

public class Test : ProcessingLite.GP21
{
	void Start()
	{
    Line(4, 7, 4, 3);
    Line(4, 5, 6, 5);
    Line(6, 7, 6, 3);
    Line(8, 5.5f, 8, 3);
    Line(8, 7, 8, 6.8f);
  }
}
```

## Contributions
- [Wowbagger84](https://github.com/wowbagger84)
- [millennIumAMbiguity](https://github.com/millennIumAMbiguity)


## References
- [Processing](https://processing.org/)
