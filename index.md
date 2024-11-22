# Welcome to Atlas
Copyright Notice

© 2024 Paul Galjan. All rights reserved. This project and its contents, including any designs, specifications, and associated materials, are protected by copyright law. Unauthorized use, reproduction, or distribution of this document or any part of its contents is prohibited without the express written permission of Paul Galjan.

Legal Use and Restrictions

This document is intended solely for personal use and may not be shared, reproduced, or modified without prior written consent. Violators may be subject to legal action.

## Overview
Atlas is a concept for a scalable multi-user platform for structured planning and reporting featuring frictionless onboarding and granular access control for teams of any size and composition.  

Using a streamlined interface to organize elements and resources, planning teams can use the platform to quickly generate, iterate, assess, and compare business plan and proposal assets.  Analysts can construct reports across structures for comparative and historical analysis.  Instructors can leverage it for syllabus and asset distribution as well as student assignment collection, with a robust backend for snapshotting and timestamping. Student can leverage it for structured notetaking aligning to a syllabus or learning plan.  Buy-side planners can leverage Atlas to collect assets from vendors, suppliers and distributors.  UI developers can leverage the platform to transform the user experience for existing content management or records user interfaces.


## Proof of concept
[Markmap](https://github.com/markmap/markmap) (MIT License) is a typescript mindmap renderer leveraging YAML-like markup for structure, resulting in very simple human-readable backmatter.  Tolerant of raw markdown, with intelligent parsing of headers and bullets while ignoring tables and base text, along with support for CSS, and allows for initial fold status at the node level.  Markmap does not render unstructured datasets or hierarchies deeper than six.

The backend is logically separated from the renderer, so markmap can and will co-exist and interoperate with alternative renderers such as [drawio](https://github.com/jgraph/drawio) (Apache License) to address canvas-style and deep structure use cases.   The same data set can be leveraged in multiple structures, so user could define their own hierarchies or canvases, save and switch between them without impacting the state and content of the objects, even if the views leverage different renderers.

### Example markup
#### Example Frontmatter
![frontmatter](image-3.png)

#### Example backmatter
![backmatter](image-2.png)

### Output
All simulations have excel-generated guids.

- Bicycle Project Test: Semi-functional demo for project quoting.  Has sample backend data and simulated iconography
  - [WBS](https://cloudmappr.github.io/atlas/bicycleDemo_WBS)
  - [Mindmap](https://cloudmappr.github.io/atlas/bicycleDemo_MM)
- Space System:  System of System structure for MIL-STD-811F Appendix J Space System with over 400 elements
  - [WBS](https://cloudmappr.github.io/atlas/spaceSystem_WBS)
  - [Mindmap](https://cloudmappr.github.io/atlas/spaceSystem_MM)
- Web Design:  Typical web design work breakdown structure
  - [WBS](https://cloudmappr.github.io/atlas/webDesign_WBS)
  - [Mindmap](https://cloudmappr.github.io/atlas/webDesign_MM)
- Curriculum:  Syllabus for a freshman-level ancient history course
  - [Mindmap](https://cloudmappr.github.io/atlas/ancientHistory_Curr)
- Learning Path: 
  - [Mindmap](https://cloudmappr.github.io/atlas/learningPath)
  
### In Context
#### Structure Display, Attributes, Summary
![nav](image-4.png)

#### Resource Attributes, Summary
![resource attributes](image-6.png)

#### Structure Inventory
![inventory](image-5.png)

#### Learning Path use case
![alt text](image-7.png)