# Sequence Types


### 1. Created a Polygon Class in polygon module:

    - where initializer takes in:
            - number of edges/vertices
            - circumradius

      - that can provide these properties:

            - edges
            - vertices
            - interior angle
            - edge length
            - apothem
            - area
            - perimeter

      - that has these functionalities:

            - a proper __repr__ function

            - implements equality (==) based on # vertices and circumradius (__eq__)

            - implements > based on number of vertices only (__gt__)

### 2. Implemented a Custom Polygon sequence type in polygon_sequence module:

    - where initializer takes in:
  
        - number of vertices for largest polygon in the sequence
        - common circumradius for all polygons

    - that can provide these properties:

        - max efficiency polygon: returns the Polygon with the highest area: perimeter ratio

    - that has these functionalities:

        - functions as a sequence type (__getitem__)
        - supports the len() function (__len__)
        - has a proper representation (__repr__)


The classes are called and tested in the notebook uploaded.




## Strictly convex polygon 

A regular strictly convex polygon is a polygon that has the following characteristics:

- all interior angles are less than 180
- all sides have equal length
 

For a regular strictly convex polygon with:

- n edges (=n vertices) and 
- R circumradius
---
- interiorAngle
  - = (n−2)⋅180/n

- edgeLength,s
  - =2⋅R⋅sin(π/n)

- apothem,a
  - =R⋅cos(π/n)

- area
  - =12⋅n⋅s⋅a

- perimeter
  - =n⋅s