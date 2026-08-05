# 3D CAD MODELING OF A BETA STIRLING ENGINE

_____________________________________________________________________________________________________________________________________________

## INTRODUCTION

Hello, nice to meet you all. In the following repository, I’m sharing a 3D CAD model of a Beta-type Stirling engine. It’s a small personal project motivated by my desire to explore some parametric design methodologies—and as a hobby.

Years ago, for my college thesis project, I developed a proposal for a test bench and sensor selection for a Stirling engine. Although that project never came to fruition, it taught me a lot and sparked a lasting interest in these topics.

I used the construction drawings from the book "Stirling Hot Air Engines" by Roy Darlington and Keith Strong as a reference. Some parts, such as the piston connecting rod and crank mechanisms, were modified in the model to prevent interference with both the inner walls of the cylinders and the housing.

3D CAD modeling is a skill in the field of engineering that not only allows us to visualize, communicate, and explore concepts, but also to replicate and bring to life drawings of parts, components, assemblies, and machines. Even though technological advances have replaced many of these devices, they continue to amaze both young and experienced engineers due to their apparent simplicity, as well as the coordination required for the design of their mechanisms, manufacturing, and assembly—a process that evokes an artistic one.

In an era where the focus and new developments center on electric motors and batteries, the Stirling engine seems like a thing of the past—a machine that harnesses heat from an external source to expand a gas, move pistons, and generate rotational work. However, as demonstrated by companies such as Saab (incorporating Stirling engines into military submarines https://www.saab.com/products/oceanic), Hyliion (generating electricity for data centers using linear engines based on the Stirling thermodynamic cycle https://www.hyliion.com/karno-technology/) and Stirling Ultracold (cryogenic refrigeration for the pharmaceutical and biotechnology sectors, based on the free-piston reverse Stirling cycle https://www.stirlingultracold.com), have succeeded—through their vision, intuition, creativity, strategy, and business models—in understanding market needs, keeping alive, even today, the innovative spirit of Reverend Robert Stirling when he designed and patented his first engine around 1816.

The parts were modeled in Autodesk Inventor version 2021, following certain guidelines of a methodology called “Resilient Modeling Strategy” or “Resilient CAD Modeling,” which aims to create robust digital models that are easy to edit, with a feature tree organized according to a hierarchy and sequence of actions. I would like to thank industry experts such as Richard Gebhard (Assembly Technology Inc.) and Rafael Testai (SolidWorks Content Creator), who taught the most important aspects of this method through videos and webinars.


_____________________________________________________________________________________________________________________________________________

## SOME ASPECTS RELATED TO THE MODELING STRATEGY

The process begins with constructive or wireframe sketches, which allow material to be added using extrusion, revolution, or sweep operations, followed by operations to remove material through cuts and holes; pattern and mirror operations are then applied, culminating in chamfers and fillets. This approach prevents errors caused by mismatches between sketches, geometry, and the modeling sequence. 

Take for example the next part, a Balanced Crank:

INSERTAR IMAGEN 1 y 2

The final 3D model can be seen in the images. The main geometry, as well as the location of the front holes, is specified using a Base Sketch. The part also features side holes and chamfers along its perimeter. The modeling strategy requires that sketches be referenced to the main planes or user-defined working planes; furthermore, extrusion, cut, and hole operations must be referenced to sketches and planes, rather than to specific dimensions.

To better understand the sequence and hierarchy of the operations, images and a step-by-step explanation of the modeling process are provided below.


### STEP 1. Base Sketch creation:

INSERTAR IMAGEN 1

A Base Sketch is created in the main XZ plane using the Stirling engine drawings (Darlington, Strong) as a reference. This sketch defines the part’s main geometry, from which material is added using extrusion operations. It also allows you to define sections of the part that will later be cut away or where holes will be added.


### STEP 2. Workplanes:

INSERTAR IMAGEN 6 Y 7

Workplanes are created with dimensions that define the depth or length of extrusion, cutting, and hole operations (front and lateral holes). These workplanes are referenced to the main XY, XZ, and YZ planes.


### STEP 3. Creating sketches for side holes:

INSERTAR IMAGEN 8 Y 9

Sketches for side holes must be referenced to workplanes. See the feature tree image, where they are identified with easy-to-recognize names.


### STEP 4. Extrusion:

INSERTAR 10 Y 11

The main geometry is extruded from the Base Sketch and the BaseExtrusion_Plane. It is important to note that the thickness of the extrusion is controlled by the workplane and not by a specific number or parameter in the Extrude panel; if you want to change the thickness, you must edit the workplane.


### STEP 5. Middle cut:

INSERTAR 12 13 Y 14

A cut is made through the center of the part using the Base Sketch and BaseExtrusion_Plane.


###  STEP 6. Holes:

INSERTAR 15 16 y 17

Holes are created based on the previous sketches and workplanes. When the command is executed, the diameter and thread type (if applicable) are specified. Similarly, the dimensions associated with the created holes are indicated in the feature tree.


### STEP 7. Chamfers:

INSERTAR 18 Y 19

Finally, aesthetic or detail elements, such as chamfers, are added. In my experience, this type of feature tends to cause a lot of problems if it isn't properly referenced, which is why the modeling strategy specifies that it should be done as the final step.


