# [[Concept design]]

When embarking on a concept design, designers need to decide which aspects of the product must be considered, and which tools will be used to make a start.

Usually, this is based off considerations of previous designs.

Given a few previous designs, it is usually possible to construct some basic design rules that will allow a designer to make outline predictions,  thus the use of [[statistically based tools in concept design]].

## Quantities characterised in Concept design

The designs produced during concept design can be characterised by relatively few quantities.

A typical aircraft design may be summarised by less than 100 numbers at this stage.

> [!NOTE]
> The "aim is to obtain the information required in order to decide whether the concept will be technically feasible and possess satisfactory economic possibilities" - Torenbeek

In the modern day UAV design process, the merging of the [[Concept design]] and [[Preliminary design]] eliminates [[difficulties due to conflict between economic and engineering perspectives]] to a large extent. However - it requires a greater effort to set up and develop.

> [!NOTE] Possibility of automating the decision making process
> This decision-making process is still normally carried out manually. However, it is starting to change with the development of multiobjective optimization, game theory, and search methods in decision making.

# [[Preliminary design]]

Once the economic decision is made to proceed, the **preliminary design (or full concept / development definition**) stage begins.

Traditionally, different aspects o the design will be considered by dedicated teams

- eg. aerodynamics, structures control systems, costing, etc.
- eg. fuselage, wing, tail, propulsion

> [!NOTE] IPTs (Integrated project teams)
> Such teams are formed specifically for the product, and grow in size progressively throughout this stage.
>
> It is supported by specialist divisions who are charged with providing technical input across a range of project teams.

## Tools used in the preliminary design stage

> [!NOTE] FEA (finite element analysis)
> Designers considering structures will conduct detailed stress analysis using this tool.

> [!NOTE] CFD methods (Computational fluid dynamics)
> Those considering wings will consider predictions of the airflow through extensive use of CFD methods.

Noteworthily, computational tools tend to have no _direct_ impact on the geometry of the design being produced. They are used for analysis.

It is left to the designer to make decisions on how to change the design as a result of these outputs.

# [[Detail Design]]

Once the [[Preliminary design]] is complete, detail/production/embodiment design begins.

This stage focuses on design verification. This may involved prototype manufacture and testing.

Issues such as robustness, reliability, safety and maintainability will be major concerns.

At this stage, little work is automated/parametized. Detailing **CAD representations** with all the information needed for manufacturing remains an intensely manual task.

## CAD systems

The effort required to convert full geometries into descriptions capable of being analyzed by [[CFD]] or [[FEA]] codes is often so great, that such analyses are carried out less often than desirable.

In most small-scale UAV programs, this means full stress analysis is rarely carried out, with reliance being placed on prototype testing.

# Manufacturing Design

Once a detailed design is completed, manufacturing begins.
A complete description of the final product isn't enough to answer:

- if the desired material properties will mandate a certain manufacturing process
- If special geometric properties are required
- if special tooling is required
  Thus the need for manufacturing design.
