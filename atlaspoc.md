# Atlas Proofs of Concept

## Markmap
[Markmap](https://github.com/markmap/markmap) is a typescript mindmap renderer available under MIT license, leveraging YAML-like markup for structure, resulting in very simple backmatter.  Tolerant of raw markdown, with intelligent parsing of headers and bullets while ignoring tables and base text.  It's possible to contribute code back to markmap to will render these elements in the hierarchy.

Markmap does not render unstructured datasets, however it will co-exist and interoperate with alternative renderers such as [drawio](https://github.com/jgraph/drawio) (Apache License) in order to address canvas-style use cases.   Additionally, the same data set can be levered in multiple structures, so user could define their own hierarchies or canvases, save and switch between them, without impacting the state and content of the objects.

### Example markup
#### Example Frontmatter
![frontmatter](image-3.png)

#### Example backmatter
![backmatter](image-2.png)

### Output
All simulations have guids; only Bicycle Simulator has sample backend data

- Bicycle Project Test: Semi-functional demo for project quoting
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
  - [Mindmap](https://cloudmappr.github.io/atlas/learningPath.html)
  
### In Context
#### Structure Navigation and Object Editing
![nav](image-4.png)

#### Structure Inventory
![inventory](image-5.png)