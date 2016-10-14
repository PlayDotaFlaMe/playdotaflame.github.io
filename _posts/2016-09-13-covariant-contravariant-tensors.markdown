---
layout: post
title:  "Covariant & Contravariant Tensors"
date:   2016-09-13 
categories: Tensors
---


<div id="main">
  Test
</div>

<style>

#arow {
  stroke-width: 1;
}

.arrow {
  stroke-width: 5;
  stroke: #000;
}

.arrow:hover {
 stroke: red; 
}

</style>

<script src="//d3js.org/d3.v4.min.js"></script>

<script>

var width = 900;
var height = 500;

var originX = 450;
var originY = 250;

svg = d3.select("#main").append("svg")
      .attr("width", width)
      .attr("height", height);

defs = svg.append("defs");

defs.append("marker")
    .attr("id", "arrow")
    .attr("viewBox", "0 0 10 10")
    .attr("refX", 0)
    .attr("refY", 5)
    .attr("markerWidth", 4)
    .attr("markerHeight", 4)
    .attr("orient", "auto")
  .append("path")
    .attr("d", "M 0 5 V 10 L 10 5 L 0 0")
    .attr("class", "arrowHead");

svg.append("line")
  .attr("class", "arrow")
  .attr("marker-end", "url(#arrow)")
  .attr("x1", originX)
  .attr("y1", originY)
  .attr("x2", originX + 150)
  .attr("y2", originY + 50);

</script>
