

# Introducing Atlas
Copyright Notice

© 2024 Paul Galjan. All rights reserved. This project and its contents, including any designs, specifications, and associated materials, are protected by copyright law. Unauthorized use, reproduction, or distribution of this document or any part of its contents is prohibited without the express written permission of Paul Galjan.

Legal Use and Restrictions

This document is intended solely for personal use and may not be shared, reproduced, or modified without prior written consent. Violators may be subject to legal action.

## Overview & Use Cases
Atlas is a conceptual structure visualization and annotation platform featuring a modular interactive renderer that allows the user to create or calculate multiple structured or unstructured views of their data.  These views can be shared with others, and the same data may be represented in different views while maintaining consistency.

The front-end is paired with a simple, flexible and scalable multi-user key/value store for user annotation of the data, along with subsequent reporting.

<table border="0">
 <tr>
    <td> 
    <img src="./img/image-4.png" alt="project planner use case"> 
    </td>
    <td>
    
- **Strategy teams** can quickly generate, iterate, assess, and compare business plan and proposal assets.  

- **Analysts** can construct reports across structures for comparative and historical analysis.  

- **Generative AI Consumers** can structure GenAI output for human curation, research, and annotation

- **Instructors** can distribute syllabus and other assets, and gather assets from learners. 

- **Learners** can leverage it for structured notetaking aligning to a syllabus or learning plan.  

- Buy-side **planners** can collect and report on assets from vendors, suppliers and distributors.  

- **UX designers** can quickly re-imagine  legacy records user experiences, using the Atlas backend to integrate and enrich data from multiple sources.  

- **Consultants** can create flexible, semi-structured data sets and no-code UIs for comparative analysis.</td>
 </tr>
</table>


## Proof of concept<!-- markmap: foldAll -->
The PoC is built on, but not dependent on, [Markmap](https://github.com/markmap/markmap) (MIT License), a typescript mindmap renderer leveraging YAML-like markup for structure, resulting in simple. human-readable backmatter.  It is tolerant of raw markdown, with intelligent parsing of headers and bullets while ignoring tables and base text, along with support for CSS, and allows for initial fold status at the node level, so it's an ideal candidate for initial exploration of the concept.  Markmap does not render unstructured datasets.

The backend is logically separated from the renderer, maintaining UUIDs and annotated, so markmap can and will co-exist and interoperate with alternative renderers such as [drawio](https://github.com/jgraph/drawio) (Apache License) or [mermaid](https://github.com/mermaid-js/mermaid) (MIT License) to address canvas-style, tree-style, workflow, state diagram, ganntt, C4, and deep structure use cases.   The same data set can be leveraged in multiple structures, so user could define their own hierarchies or canvases, save and switch between them without impacting the state and content of the objects.

### Markmap
<table border="0">
 <tr>
    <td> 
    <img src="./img/image-3.png" alt="markmap frontmatter"> 
    </td>
    <td>
    <img src="./img/image-2.png" alt="markmap backmatter"> 
 </tr>
</table>

### Simulations
All simulations have randomized excel-generated guids, which are more or less reliable for test purposes but clearly not RFC9562 compliant.

#### **Bicycle Project Test**: Semi-functional project quoting demo with sample backend data and simulated iconography

<table border="0">
 <tr>
    <td> 
<iframe
  src="./bicycleDemo_WBS.html"
  style="width:800px; height:400px;"
></iframe>
    </td>
    <td>
<iframe
  src="./054c5638-61a8-7530-789c-aeb3b73e746d.html"
  style="width:600px; height:400px;"
></iframe>
 </tr>
</table>




#### Other structures
-  [**Space System**](./spacedemo.html):  System of System structure for [MIL-STD-811F Appendix J Space System](https://quicksearch.dla.mil/qsDocDetails.aspx?ident_number=36026) with over 400 elements

- [**Product breakdown**](./computerpbs.html): PBS for a typical laptop computer 

- [**Human Body**](./humanbody.html):  Taxonomy for human anatomy
  
- [**Web Design**](./webDesign_WBS.html):  Typical web design work breakdown structure

- [**Human brain**](./humanbrain.html): Taxonomy of the human brain

- [**Sensor Package**](./autonomousVehicle.html):  Notional sensing and control package for autonomous systems

- [**Curriculum**](./ancientHistory_Curr.html):  Syllabus for a freshman-level ancient history course

- [**Languages**](./humanlanguages.html): Human Language Taxonomy


- [**Learning Path**](./learningPath.html): Example learning path


### Mock Data Set
Mock data for these and a variety of structures are provided in the atlas [wbs generator](./AtlasWBSGenerator.xlsx)

- **uatDataSet**:  User acceptance data - the platform is expected to calculate the numerically accurate structure for each named dataset, along with an [RFC9562](https://datatracker.ietf.org/doc/html/rfc9562)-compliant **version 4** UUID for each record, populating the results into an appropriate persistent data store to generate backmatter and allow the user to enrich the data.

- **wbs2markmap**: Allows users to create their own numerically accurate structures with guids, customize the base url and iconography.

- **markmap2wbs**:   Converts hash-annotated markmap into a numerically accurate structure with guids.

### In Context

#### [Structure Display, Attributes, Summary nav](./img/image-4.png)

![nav](./img/image-4.png)

#### [Resource Attributes, Summary](./img/image-6.png)

![nav](./img/image-6.png) 

#### [Structure Inventory](./img/image-5.png)

![nav](./img/image-5.png) 

#### [Learning Path use case](./img/image-7.png) 

![nav](./img/image-7.png)

#### [Structure-level attributes](./img/image-8.png)

![alt text](./img/image-8.png)

#### [Export](./img/image-9.png)

![alt text](./img/image-11.png)
![alt text](./img/image-12.png)

#### [Cross-structure reporting](./img/image-10.png)

![alt text](./img/image-10.png)