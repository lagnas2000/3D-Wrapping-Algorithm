# 3D-Wrapping-Algorithm
This project is 3D wrapping algoritm for Unity3D. 

This algorithm does not originated by gift wrapping. Make a 3-dimension convex hull that contain all given points.


Algorithm
---------

- Make a new two list, openPoints and closePoints.
  - openPoints is list for outer point or maybe outerpoint.
  - closePoints is list for inner point.

- Make a first tetrahedron.

- The tetrahedron`s triangles` vertices make clockwise by tetrahedron`s center.
  - If point inner tetrahedron, all triangles of tetrahedron is clockwise.
  So, at least one triangle detected counterclockwise by outer point.
  
- Merging tetrahedron with outer points.



Details
-------

- Make a first tetrahedron. 

1. Select 3 points of all points randomly. Called them A, B, C.
2. Pick other point
3. Check the point same plane with ABC or not. 
4. If same plane, go to 2.
5. If not same plane, make a first tetrahedron.

- Validate tetrahedron`s polygon`s vertices make clockwise.

1. 
