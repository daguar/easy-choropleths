Easy Choropleths
====

An experimental tool to let humans build choropleths (data-shaded maps) without any knowledge of Javascript or GIS.

Try it out here! http://daguar.github.io/easy-choropleths/

### About

The idea and motivation for this is flushed out in my `ideas` repo here: https://github.com/daguar/ideas/issues/2

### How it works

At a basic level, what this app does is pretty simple:

- Pulls data from a Google Spreadsheet (using Tabletop)
- Scales the data by putting each value into a bucket; buckets here are of equal size based on the minimum and maximum values, a "quantize" scale in D3 terms (using D3 and ColorBrewer)
- Maps the data by a color scale based on the scaled values (using Leaflet)

Everything's done in Javascript, so it's a simple static site.

### Running Locally

Right now, easiest way is to `cd` into the root directory and run the python one-liner web server:
`python -m SimpleHTTPServer`

Then load up your browser (preferably Chrome with Dev Console open) to:

http://0.0.0.0:8000/


Copyright Dave Guarino, 2014
