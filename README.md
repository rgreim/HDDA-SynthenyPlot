# ScatterPlot
This repository includes a way to visualize genom data as scatterplot to find synteny parts.

## Good to know
The project is a perfomance for M-BS2-S4B SS2015 at the Justus-Liebig-University Giessen. For the overview [this nice example](http://bl.ocks.org/mbostock/3213173) was used and modified. Brushing is not implemented because d3.brush and d3.zoom both trigger on drag. The links where to look for the genome/gen are hardcoded. The search pattern is individual. The length is calculated from start and end position. This could be a problem when you use circular genomes.

### Requirements
Datafile as JSON. See the example in the files folder. Javascript libraries [D3.js](http://d3js.org) and [underscore.js](http://underscorejs.org).
 
### Usage
In the overview click on the plot you want to see in detail. In the single view you can zoom in and out. Also it is possible to mark the dots by clicking and get them into a table. A rightclick on the dots makes it possible to click on the links to the genes and genomes.
 
### The data
The file "data_sets/Arabidopsis/Arabidopsis.Release5.matchList" from [DAGchainer: Computing Chains of Syntenic Genes in Complete Genomes](http://dagchainer.sourceforge.net/) was used to fill our own JSON file. Thanks a lot!

### What is missing
You cannot save the marked data/ the table or the SVG itself.

### Bugs
The click to open the single plot only works if not clicked on dots. If drawing a frame (class=frame) only a click on the frame opens a new window.

## Licence
The MIT License (MIT)

Copyright (c) 2015 Sabine Hurka, Jens Schauer, Mark-Robin Greim

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
