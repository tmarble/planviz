# Change Log

All notable changes to this project will be documented in this file. This change log follows the conventions of [keepachangelog.com](http://keepachangelog.com/).

### [Unreleased]

Added
- *TBD*
Changed
- Show between labels on activities (in parens)
- Show sequence-labels on nodes and activities (if present)
- Fixed edge/plant-id to be edge/plantid
- ui.cljs now calculates label width using the same algorithm as tplan.cljs
- Added `/export` function to save a plan as an SVG file

### [0.8.2] - 2016-04-27

Changed
* Significant performance improvements
  * Optimized component queries (to be minimal)
  * Specified precise, minimal queries where full denormalization was unnecessary
  * Decomposed long running functions into several asynchronous tasks
  * Various ClojureScript performance improvements
* Fixed plan loading to pre-load corresponding TPN (when available)
* Added a hide/show tooltips function
* Reorganized actions.cljs function order
* Updated dependencies
* Removed vestiges of non graphic rendering support

### [0.8.1] - 2016-04-12

Changed
* Initial publication on github

### 0.1.0

Added
*  Initial version

[0.8.1]: https://github.com/dollabs/planviz/compare/0.1.0...0.8.1
[0.8.2]: https://github.com/dollabs/planviz/compare/0.8.1...0.8.2
[Unreleased]: https://github.com/dollabs/planviz/compare/0.8.2...HEAD