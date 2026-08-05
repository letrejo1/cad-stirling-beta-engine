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

Se puede apreciar en las imágenes el modelo 3D final. La geometría principal y ubicación de los orificios frontales se especifica mediante un Base Sketch. La pieza también presenta orificios laterales y chaflanes en su perímetro. La estrategia de modelado requiere que los sketchs sean referenciados a los planos principales o planos de trabajo creados por el usuario; también, es necesario que las operaciones de extrusión, corte y orificios sean referenciados a planos y no a dimensiones particulares.

Para entender mejor la secuencia y jerarquía de las operaciones, a continuación se mostrara imágenes del modelo paso a paso.

### STEP 1: Base Sketch

INSERTAR IMAGEN 1

A partir de los planos del motor Stirling, se realiza un Base Sketch en el plano principal XZ con la geometría principal de la pieza, con la finalidad de realizar posteriormente la extrusión, corte y orificios frontales.

### STEP 2: Creación de Workplanes para realizar extrusión frontal y orificios laterales
