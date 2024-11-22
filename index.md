---
markmap: 
  colorFreezeLevel: 2
  maxWidth: 300
  initialExpandLevel: 2
  embedAssets: true
---
# Introducing Atlas
Copyright Notice

© 2024 Paul Galjan. All rights reserved. This project and its contents, including any designs, specifications, and associated materials, are protected by copyright law. Unauthorized use, reproduction, or distribution of this document or any part of its contents is prohibited without the express written permission of Paul Galjan.

Legal Use and Restrictions

This document is intended solely for personal use and may not be shared, reproduced, or modified without prior written consent. Violators may be subject to legal action.

## Overview
Atlas is a conceptual structure visualization and annotation platform featuring a modular interactive renderer that allows the user to choose and create multuple structured or unstructured views of their data.  The front-end is paired with a simple, flexible and scalable multi-user key/value store for user annotation of the data, along with subsequent reporting.

<iframe
  src="https://cloudmappr.github.io/atlas/atlasintro.html"
  style="width:100%; height:300px;"
></iframe>

### Use cases

#### **strategy teams** can use the platform to quickly generate, iterate, assess, and compare business plan and proposal assets.  
#### **Analysts** can construct reports across structures for comparative and historical analysis.  
#### **Instructors** can leverage it for syllabus and asset distribution as well as student assignment collection, with a robust backend for snapshotting and timestamping. 
#### **Students** can leverage it for structured notetaking aligning to a syllabus or learning plan.  
#### Buy-side **planners** can leverage Atlas to collect assets from vendors, suppliers and distributors.  
#### **UX designers** can leverage the platform to overhaul the user experience for legacy records interfaces interfaces, and it the Atlas backend to integrate and enrich data from multiple sources.  
#### **Consultants** can leverage Atlas to create flexible, semi-structured data sets for comparative analysis.


## Proof of concept
The PoC is built on, but not dependent on, [Markmap](https://github.com/markmap/markmap) (MIT License), a typescript mindmap renderer leveraging YAML-like markup for structure, resulting in simple. human-readable backmatter.  It is tolerant of raw markdown, with intelligent parsing of headers and bullets while ignoring tables and base text, along with support for CSS, and allows for initial fold status at the node level, so it's an ideal candidate for initial exploration of the concept.  Markmap does not render unstructured datasets or hierarchies deeper than six.

The backend is logically separated from the renderer, maintaining UUIDs and annotated, so markmap can and will co-exist and interoperate with alternative renderers such as [drawio](https://github.com/jgraph/drawio) (Apache License) or [mermaid](https://github.com/mermaid-js/mermaid) (MIT License) to address canvas-style, tree-style, workflow, state diagram, ganntt, C4, and deep structure use cases.   The same data set can be leveraged in multiple structures, so user could define their own hierarchies or canvases, save and switch between them without impacting the state and content of the objects, even if the views leverage different renderers.

### Markmap
#### Example Frontmatter
![frontmatter](image-3.png)

#### Example backmatter
![backmatter](image-2.png)

### Output
All simulations have excel-generated guids, which are reliable for test purposes but not RFC9562 compliant.

#### **Bicycle Project Test**: Semi-functional demo for project quoting.  Has sample backend data and simulated iconography

##### [WBS](https://cloudmappr.github.io/atlas/bicycleDemo_WBS)

##### [Mindmap](https://cloudmappr.github.io/atlas/bicycleDemo_MM)

#### **Space System**:  System of System structure for MIL-STD-811F Appendix J Space System with over 400 elements

##### [WBS](https://cloudmappr.github.io/atlas/spaceSystem_WBS)

##### [Mindmap](https://cloudmappr.github.io/atlas/spaceSystem_MM)

#### **Web Design**:  Typical web design work breakdown structure

##### [WBS](https://cloudmappr.github.io/atlas/webDesign_WBS)

##### [Mindmap](https://cloudmappr.github.io/atlas/webDesign_MM)

#### **Curriculum**:  Syllabus for a freshman-level ancient history course

##### [Mindmap](https://cloudmappr.github.io/atlas/ancientHistory_Curr)

#### Learning Path: 
##### [Mindmap](https://cloudmappr.github.io/atlas/learningPath)

#### [Mock Data Set](https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fcloudmappr.github.io%2Fatlas%2Ftemplate.xlsx&wdOrigin=BROWSELINK)
Mock data for these and a variety of structures are provided in the atlas 

#####  **uatDataSet**:  User acceptance data - the platform is expected to calculate the numerically accurate structure for each named dataset, along with an [RFC9562](https://datatracker.ietf.org/doc/html/rfc9562)-compliant UUID for each record, populating the results into an appropriate persistent data store to generate backmatter and allow the user to enrich the data.

#####  **wbs2markmap**: Allows users to create their own numerically accurate structures with guids, customize the base url and iconography.

#####  **markmap2wbs**:   Converts hash-annotated markmap into a numerically accurate structure with guids.

### In Context
#### [Structure Display, Attributes, Summary nav](image-4.png)
![nav](image-4.png)
#### [Resource Attributes, Summary](image-6.png)
![nav](image-6.png) 
#### [Structure Inventory](image-5.png)
![nav](image-5.png) 
#### [Learning Path use case](image-7.png) 
![nav](image-7.png)