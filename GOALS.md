Web Threading Model Goals
=========================

### tl;dr
We want to empower web authors to create rich, custom effects without sacrificing [performance](https://docs.google.com/document/d/1bYMyE6NdiAupuwl7pWQfB-vOZBPSsXCv57hljLDMV8E/edit).

### preliminaries
In the best of all possible worlds, every operation on the web would be fast. Style, layout, painting, rastering, JS, etc. would all complete well within the frame budget and there would be no need for threaded solutions or the complexity that comes with them. This ideal is not as crazy as it sounds. Certainly, each of these operations can have unbounded execution time, but if we were able to decompose these operations, we might be able to introduce some bounds. And even in the absense of bounds, we can make these operations awfully fast (eg, GPU rasterization). Before getting into goals for threaded solutions to performance issues on the web, it's worth remembering that they're not the only solutions, and perhaps not even the best.

### tough cases
One way to measure the quality of a solution, is to judge its performance on a set of difficult test pages. TODO: create some tests and upload.

### must have's
- Must be possible to coordinate effects with input.
- TODO: more?

### nice to have's
TODO: fill this in
