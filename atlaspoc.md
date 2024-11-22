# Atlas Proofs of Concept

## Markmap
[Markmap](https://github.com/markmap/markmap) (MIT License) is a typescript mindmap renderer leveraging YAML-like markup for structure, resulting in very simple human-readable backmatter.  Tolerant of raw markdown, with intelligent parsing of headers and bullets while ignoring tables and base text, along with support for CSS, and allows for initial fold status at the node level.  Markmap does not render unstructured datasets or hierarchies deeper than six.

The backend is logically separated from the renderer, so markmap co-exist and interoperate with alternative renderers such as [drawio](https://github.com/jgraph/drawio) (Apache License) to address canvas-style and deep structure use cases.   The same data set can be leveraged in multiple structures, so user could define their own hierarchies or canvases, save and switch between them without impacting the state and content of the objects, even if the views leverage different renderers.

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
#### Structure Navigation and Object Editing
![nav](image-4.png)

#### Structure Inventory
![inventory](image-5.png)