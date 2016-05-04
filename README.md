# planviz

Planning Network Visualization

As this is a pre-release version **planviz**. You can clone
it (and the required libraries) to build it locally.

<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"  id="bigplan" viewBox="0 0 305 290" style="top:0px;left:0px;" width="470.12068965517244" height="447" data-reactid=".2">
<style type="text/css">
<![CDATA[
/* Copyright (c) 2016 Dynamic Object Language Labs Inc.

   This software is licensed under the terms of the
   Apache License, Version 2.0 which can be found in
   the file LICENSE at the root of this distribution.
*/

svg, g, rect, circle, text, symbol, use {
    pointer-events: all;
}

.plain {
    fill: none;
    stroke: black;
    stroke-width: 1px;
}

#arrowhead {
    fill: #444;
}

#arrowlight {
    fill: lightblue;
}

#arrow {
    /* fill: #555; */
    fill: rgba(100,100,100,0.9);
}

#arrow-long {
    /* fill: #888; */
    fill: rgba(150,150,150,0.9);
}

#arrow-very-long {
    /* fill: #ccc; */
    fill: rgba(200,200,200,0.9);
}

#choicehem > circle {
    fill: blue;
}

.outline {
    fill: none;
    stroke: green;
    stroke-width: 1px;
}

.planview {
    fill: rgba(0,0,255,0.2);
    stroke: none;
}


.activity-normal, .null-activity-normal, .parallel-edge-normal {
    fill: none;
    stroke: #444;
    stroke-width: 3.0px;
}

.choice-edge-normal {
    fill: none;
    stroke: #888;
    stroke-width: 3.0px;
}

.target-unselected {
    fill: none;
}

.node .target-unselected {
    stroke: none;
}

.node .target-selected {
    opacity: 0.67;
    fill: yellow;
}

.node:hover .target-selected, .node:hover .target-unselected {
                                  opacity: 0.67;
                                  fill: Fuchsia;
                              }

.edge .target {
    fill-opacity: 0.67;
    opacity: 0.67;
    stroke-width: 8px;
}

.edge .target-unselected {
    fill-opacity: 0.67;
    opacity: 0.67;
    stroke: none;
    stroke-width: 8px;
}

.edge .target-selected {
    fill-opacity: 0.67;
    opacity: 0.67;
    stroke: yellow;
    stroke-width: 8px;
}

.edge:hover .target-selected, .edge:hover .target-unselected {
                                  stroke: Fuchsia;
                                  stroke-width: 8px;
                              }

.activity-active, .null-activity-active, .activity-started, .null-activity-started, .choice-edge-active, .parallel-edge-active, .choice-edge-started, .parallel-edge-started {
    fill: none;
    stroke: blue;
    stroke-width: 3.0px;
}

.activity-finished, .null-activity-finished, .choice-edge-finished, .parallel-edge-finished {
    fill: none;
    stroke: #00ff00;
    stroke-width: 3.0px;
}

.activity-negotiation, .null-activity-negotiation, .activity-start, .null-activity-start, .choice-edge-negotiation, .parallel-edge-negotiation  {
    fill: none;
    stroke: orange;
    stroke-width: 3.0px;
}

.activity-best, .null-activity-best, .choice-edge-best, .parallel-edge-best {
    fill: none;
    stroke: magenta;
    stroke-width: 3.0px;
}

.activity-impossible, .null-activity-impossible, .choice-edge-impossible, .parallel-edge-impossible  {
    fill: none;
    stroke: grey;
    stroke-width: 3.0px;
}

.activity-failed, .null-activity-failed, .choice-edge-failed, .parallel-edge-failed  {
    fill: none;
    stroke: red;
    stroke-width: 3.0px;
}


.edge-vedge {
    fill: none;
    stroke: yellow;
    stroke-width: 3.0px;
}

.virtual-normal {
    fill: none;
    stroke: #eee;
    stroke-width: 3.0px;
}

.temporal-constraint-normal {
    fill: none;
    stroke-dasharray: 2 2;
    stroke: rgba(100,100,100,0.5);
    stroke-width: 3.0px;
}

.temporal-constraint-normal-long {
    fill: none;
    stroke-dasharray: 3 3;
    stroke: rgba(150,150,150,0.5);
    stroke-width: 3.0px;
}

.temporal-constraint-normal-very-long {
    fill: none;
    stroke-dasharray: 4 4;
    stroke: rgba(200,200,200,0.5);
    stroke-width: 1px;
}

.parallel-normal, .choice-normal, .state-normal {
    /* fill: #0099cc; */
    fill: white;
    stroke: #006699;
    stroke-width: 3px;
}

.parallel-best, .choice-best, .state-best {
    fill: magenta;
    stroke: #006699;
    stroke-width: 3px;
}

.parallel-impossible, .choice-impossible, .state-impossible {
    fill: silver;
    stroke: #006699;
    stroke-width: 3px;
}

.parallel-reached, .choice-reached, .state-reached {
    fill: #00ff00;
    stroke: #006699;
    stroke-width: 3px;
}

.parallel-failed, .choice-failed, .state-failed {
    fill: #ff0000;
    stroke: #006699;
    stroke-width: 3px;
}

/* typically :started is not used for TPN nodes */
.parallel-started, .choice-started, .state-started {
    fill: blue;
    stroke: #006699;
    stroke-width: 3px;
}

.hem-normal {
    fill: white;
    stroke: Chocolate;
    stroke-width: 3.0px;
}

.hem-reached {
    fill: #00ff00;
    stroke: Chocolate;
    stroke-width: 3.0px;
}

.hem-best {
    fill: magenta;
    stroke: Chocolate;
    stroke-width: 3.0px;
}

.hem-impossible {
    fill: silver;
    stroke: Chocolate;
    stroke-width: 3.0px;
}

.hem-reached {
    fill: #00ff00;
    stroke: Chocolate;
    stroke-width: 3.0px;
}

.hem-failed {
    fill: red;
    stroke: Chocolate;
    stroke-width: 3.0px;
}

.hem-started {
    /* fill: #0099cc; */
    fill: blue;
    stroke: Chocolate;
    stroke-width: 3.0px;
}

.active, .started {
    fill: blue;
    stroke: #006699;
    stroke-width: 4px;
}

.best {
    fill: magenta;
    stroke: #006699;
    stroke-width: 4px;
}

.negotiation, .start  {
    fill: orange;
    stroke: #006699;
    stroke-width: 4px;
}

.impossible {
    fill: grey;
    stroke: #006699;
    stroke-width: 4px;
}

.failed {
    fill: red;
    stroke: #006699;
    stroke-width: 4px;
}

.state-virtual-normal {
    fill: #eee;
    stroke: lightgray;
    stroke-width: 4px;
}

.normal-probability {
    fill: #0099cc;
    stroke: #006699;
    stroke-width: 4px;
}

.active-probability, .started-probability {
    fill: blue;
    stroke: #006699;
    stroke-width: 4px;
}

.reached-probability {
    fill: #00ff00;
    stroke: #006699;
    stroke-width: 4px;
}

.best-probability {
    fill: magenta;
    stroke: #006699;
    stroke-width: 4px;
}

.negotiation-probability, .start-probability  {
    fill: orange;
    stroke: #006699;
    stroke-width: 4px;
}

.impossible-probability {
    fill: grey;
    stroke: #006699;
    stroke-width: 4px;
}

.failed-probability {
    fill: red;
    stroke: #006699;
    stroke-width: 4px;
}

.parallel {
    stroke: black;
    stroke-width: 3px;
}

.choice {
    fill: none;
    stroke: black;
    /* stroke-width: 1.5px; */
    stroke-width: 3px;
}

.unchoice {
    fill: none;
    stroke: #555;
    stroke-width: 2.2px;
}

text {
    font-size: 9px;
    font-family: Roboto Condensed, Liberation Sans Narrow, Nimbus Sans Condensed,  Helvetica Narrow, Helvetica, Verdana, Arial, sans-serif;
    pointer-events: none;
    text-shadow: 0.16em 0.16em 0.10em white, -0.16em -0.16em 0.10em white, -0.16em 0.16em 0.10em white, 0.16em -0.16em 0.10em white;
}

text.node-label {
    font-size: 7px;
    fill: DarkSlateGrey;
}

.show, .node:hover .node-tooltip, .edge:hover .edge-tooltip {
                                      fill-opacity: 1.0;
                                      opacity: 1.0;
                                  }

.hide {
    opacity: 0.0;
    fill-opacity: 0.0;
}

.node {
}

.edge {
}

.node-tooltip, .edge-tooltip {
    transition: opacity 0.5s ease;
}
.node-tooltip rect, .edge-tooltip rect {
    fill: Cornsilk;
    stroke: Chocolate;
    stroke-width: 1.0px;
}

]]>
</style>
<defs data-reactid=".2.0">
<g id="state" data-reactid=".2.0.0">
<circle r="10" class="node" data-reactid=".2.0.0.0">
</circle>
</g>
<g id="parallel" data-reactid=".2.0.1">
<circle r="10" class="node" data-reactid=".2.0.1.0">
</circle>
<path d="M-5 -7L-5 7M5 7L5 -7" class="parallel" data-reactid=".2.0.1.1">
</path>
</g>
<g id="choice" data-reactid=".2.0.2">
<circle r="10" class="node" data-reactid=".2.0.2.0">
</circle>
<circle r="5" class="choice" data-reactid=".2.0.2.1">
</circle>
</g>
<g id="unchoice" data-reactid=".2.0.3">
<circle r="10" class="node" data-reactid=".2.0.3.0">
</circle>
<path d="M-4.719484489288494 2.7247956403269757L-4.719484489288494 -2.7247956403269757L0 -5.4495912806539515L4.719484489288494 -2.7247956403269757L4.719484489288494 2.7247956403269757L0 5.4495912806539515Z" class="unchoice" data-reactid=".2.0.3.1">
</path>
</g>
<g id="hem" data-reactid=".2.0.4">
<rect x="-40" y="-20" rx="3" ry="3" width="80" height="40" class="hem" data-reactid=".2.0.4.0">
</rect>
</g>
<g id="markers" data-reactid=".2.0.5">
<marker id="arrowhead" orient="auto" markerHeight="4" markerWidth="4" refY="0" refX="17" viewBox="0 -5 10 10">
<path d="M0,-5L10,0L0,5">
</path>
</marker>

<marker id="choicehem" orient="auto" markerHeight="5" markerWidth="5" refY="0" refX="-70" viewBox="-5 -5 10 10">
<circle r="5">
</circle>
</marker>

<marker id="arrowhem" orient="auto" markerHeight="5" markerWidth="5" refY="0" refX="5" viewBox="0 -5 10 10">
<path d="M0,-5L10,0L0,5">
</path>
</marker>

<marker id="arrowlight" orient="auto" markerHeight="4" markerWidth="4" refY="0" refX="19" viewBox="0 -5 10 10">
<path d="M0,-5L10,0L0,5">
</path>
</marker>

<marker id="arrow" orient="auto" markerHeight="3" markerWidth="3" refY="-2" refX="22" viewBox="0 -5 10 10">
<path d="M0,-5L10,-1L1,5">
</path>
</marker>

<marker id="arrow-long" orient="auto" markerHeight="3.5" markerWidth="3.5" refY="-0.5" refX="20" viewBox="0 -5 10 10">
<path d="M0,-5L10,0L0,5">
</path>
</marker>

<marker id="arrow-very-long" orient="auto" markerHeight="8" markerWidth="8" refY="0" refX="24" viewBox="0 -5 10 10">
<path d="M0,-5L10,0L0,5">
</path>
</marker>

</g>
</defs>
<g id="planviz" data-reactid=".2.1">
<g data-reactid=".2.1.$=2rmq-net-24567">
<g data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567">
<g class="edge" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24565">
<path marker-end="url(#arrowhead)" d="M25 105L75 130" class="null-activity-finished" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24565.2">
</path>
<g class="edge-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24565.3:0">
<rect x="10" y="90.5" rx="3" ry="3" width="80" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24565.3:0.0">
</rect>
<text x="14" y="100.5" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24565.3:0.1">
act-24565 finished</text>
</g>
</g>
<g class="edge" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24559">
<path d="M75 130L180 130" class="target-unselected" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24559.0">
</path>
<path marker-end="url(#arrowhead)" d="M75 130L180 130" class="activity-active" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24559.1">
</path>
<g class="edge-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24559.2:0">
<rect x="91.5" y="135" rx="3" ry="3" width="72" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24559.2:0.0">
</rect>
<text x="95.5" y="145" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24559.2:0.1">
act-24559 active</text>
</g>
</g>
<g class="edge" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24566">
<path marker-end="url(#arrowhead)" d="M180 130L230 105" class="null-activity-normal" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24566.2">
</path>
<g class="edge-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24566.3:0">
<rect x="169" y="90.5" rx="3" ry="3" width="72" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24566.3:0.0">
</rect>
<text x="173" y="100.5" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24566.3:0.1">
act-24566 normal</text>
</g>
</g>
<g class="edge" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24563">
<path marker-end="url(#arrowhead)" d="M25 105L75 80" class="null-activity-normal" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24563.2">
</path>
<g class="edge-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24563.3:0">
<rect x="14" y="65.5" rx="3" ry="3" width="72" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24563.3:0.0">
</rect>
<text x="18" y="75.5" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24563.3:0.1">
act-24563 normal</text>
</g>
</g>
<g class="edge" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24556">
<path d="M75 80L180 80" class="target-unselected" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24556.0">
</path>
<path marker-end="url(#arrowhead)" d="M75 80L180 80" class="activity-normal" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24556.1">
</path>
<g class="edge-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24556.2:0">
<rect x="91.5" y="85" rx="3" ry="3" width="72" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24556.2:0.0">
</rect>
<text x="95.5" y="95" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24556.2:0.1">
act-24556 normal</text>
</g>
</g>
<g class="edge" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2cnstr-24554">
<path marker-end="url(#arrow)" d="M75 80A78.75 78.75 0 0,1 180 80" class="temporal-constraint-normal" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2cnstr-24554.2">
</path>
<g class="edge-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2cnstr-24554.3:0">
<rect x="87.5" y="32.94678440936948" rx="3" ry="3" width="80" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2cnstr-24554.3:0.0">
</rect>
<text x="91.5" y="42.94678440936948" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2cnstr-24554.3:0.1">
cnstr-24554 normal</text>
</g>
</g>
<g class="edge" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24564">
<path marker-end="url(#arrowhead)" d="M180 80L230 105" class="null-activity-normal" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24564.2">
</path>
<g class="edge-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24564.3:0">
<rect x="169" y="65.5" rx="3" ry="3" width="72" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24564.3:0.0">
</rect>
<text x="173" y="75.5" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24564.3:0.1">
act-24564 normal</text>
</g>
</g>
<g class="node" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24561">
<circle cx="25" cy="105" r="16" class="target-unselected" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24561.0">
</circle>
<use x="25" y="105" xlink:href="#choice" class="choice-reached" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24561.1">
</use>
<g class="node-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24561.2">
<rect x="-15" y="80" rx="3" ry="3" width="80" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24561.2.0">
</rect>
<text x="-11" y="90" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24561.2.1">
node-24561 reached</text>
</g>
</g>
<g class="node" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24560">
<circle cx="75" cy="130" r="16" class="target-unselected" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24560.0">
</circle>
<use x="75" y="130" xlink:href="#state" class="state-reached" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24560.1">
</use>
<g class="node-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24560.2">
<rect x="35" y="105" rx="3" ry="3" width="80" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24560.2.0">
</rect>
<text x="39" y="115" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24560.2.1">
node-24560 reached</text>
</g>
</g>
<g class="node" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24558">
<circle cx="180" cy="130" r="16" class="target-unselected" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24558.0">
</circle>
<use x="180" y="130" xlink:href="#state" class="state-normal" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24558.1">
</use>
<g class="node-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24558.2">
<rect x="142" y="105" rx="3" ry="3" width="76" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24558.2.0">
</rect>
<text x="146" y="115" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24558.2.1">
node-24558 normal</text>
</g>
</g>
<g class="node" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24562">
<circle cx="230" cy="105" r="16" class="target-unselected" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24562.0">
</circle>
<use x="230" y="105" xlink:href="#choice" class="choice-normal" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24562.1">
</use>
<g class="node-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24562.2">
<rect x="192" y="80" rx="3" ry="3" width="76" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24562.2.0">
</rect>
<text x="196" y="90" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24562.2.1">
node-24562 normal</text>
</g>
</g>
<g class="node" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24557">
<circle cx="75" cy="80" r="16" class="target-unselected" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24557.0">
</circle>
<use x="75" y="80" xlink:href="#state" class="state-normal" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24557.1">
</use>
<g class="node-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24557.2">
<rect x="37" y="55" rx="3" ry="3" width="76" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24557.2.0">
</rect>
<text x="41" y="65" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24557.2.1">
node-24557 normal</text>
</g>
</g>
<g class="node" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24555">
<circle cx="180" cy="80" r="16" class="target-unselected" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24555.0">
</circle>
<use x="180" y="80" xlink:href="#state" class="state-normal" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24555.1">
</use>
<g class="node-tooltip hide" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24555.2">
<rect x="142" y="55" rx="3" ry="3" width="76" height="15" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24555.2.0">
</rect>
<text x="146" y="65" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2node-24555.2.1">
node-24555 normal</text>
</g>
</g>
<text text-anchor="middle" x="45" y="112.5" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24565-label">
</text>
<text text-anchor="middle" x="122.5" y="125" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24559-label">
plant$unbounded</text>
<text text-anchor="middle" x="200" y="112.5" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24566-label">
</text>
<text text-anchor="middle" x="45" y="87.5" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24563-label">
</text>
<text text-anchor="middle" x="122.5" y="75" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24556-label">
plant$bounded</text>
<text text-anchor="middle" x="122.5" y="54.94678440936948" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2cnstr-24554-label">
 [1 5]</text>
<text text-anchor="middle" x="200" y="87.5" data-reactid=".2.1.$=2rmq-net-24567.$=2rmq-net-24567=2net-24567.$=2rmq-net-24567=2act-24564-label">
</text>
</g>
</g>
</g>
</svg>

Check out the [CHANGELOG](CHANGELOG.md)

## News

The [DOLL](http://dollabs.com/) team (including
[Paul Robertson](https://twitter.com/DrPaulRobertson),
[Dan Cerys](https://twitter.com/dcerys),
[Prakash Manghwani](https://twitter.com/manghwani), and
[Tom Marble](https://twitter.com/tmarble)) recently demoed
PLANVIZ in the talk **Model based programming in PAMELA** at
[Clojure/west](http://clojurewest.org/speakers#tmarble).
Check out the [ClojureTV](https://youtu.be/WLovW6hlYHM) video
and the [slides](https://github.com/dollabs/pamela/blob/master/doc/slides/ClojureWestHelloPamela.pdf).

For more details visit the [PAMELA project page](http://dollabs.com/projects/pamela).

## Documentation

The **planviz** application is part of the [PAMELA](https://github.com/dollabs/pamela) suite of tools.

## Building

Here are the steps to build **planviz** locally:

1. Install [RabbitMQ](https://www.rabbitmq.com/) Server
 * For Debian GNU/Linux systems simply do

   `# apt-get install rabbitmq-server`

1. Install [boot](https://github.com/dollabs/plan-schema#building).
   Please note the steps to install **boot.properties** and **profile.boot**
   to your `~/.boot/` directory (so that the cider deftask is available).

   ````
   $ boot --version
   #http://boot-clj.com
   #Wed Apr 13 13:18:30 CDT 2016
   BOOT_CLOJURE_NAME=org.clojure/clojure
   BOOT_CLOJURE_VERSION=1.8.0
   BOOT_VERSION=2.5.5
   $
   ````

2. Clone and install [plan-schema](https://github.com/dollabs/plan-schema)

   ````
   $ mkdir -p ~/src/github/dollabs
   $ cd ~/src/github/dollabs
   $ git clone https://github.com/dollabs/plan-schema
   $ cd plan-schema
   $ boot local
   ````

3. Clone and install [webtasks](https://github.com/dollabs/webtasks)

   ````
   $ cd ..
   $ git clone https://github.com/dollabs/webtasks
   $ cd webtasks
   $ boot local
   ````

4. Clone and install [webkeys](https://github.com/dollabs/webkeys)

   ````
   $ cd ..
   $ git clone https://github.com/dollabs/webkeys
   $ cd webkeys
   $ boot local
   ````

5. Clone and build **planviz** (_NOTE:_ you may see various warnings
like `WARNING: Use of undeclared Var planviz.components/x21694 at line 42`
that do not prevent building)

   ````
   $ cd ..
   $ git clone https://github.com/dollabs/planviz
   $ cd planviz
   $ boot build-jar
   ````

6. Run the demo
  * *NOTE* this config uses the example plans from **plan-schema**
  * For convenience you may add the [planviz/bin](bin) directory to your `PATH`
(or simply refer to the startup script as `./bin/planviz`).
  * Note that the single argument to `planviz FOO` refers to a configuration file
    with details in `config/FOO.edn`.

   ````
   $ planviz demo
   ````

7. After you see `PLANVIZ server ready` you can open a (or several) browser windows to [http://localhost:8080](http://localhost:8080)

   ````
   $ open http://localhost:8080
   ````

## Commands (*a la* IRC)

* `/who` see which clients are connected
* `/whoami` see the host and port of your browser connection (remote id)
* `/msg user ...` private message for user
* `/nick firefox` set nickname for this connection
* `/list` list available plans
* `/show v1.tpn` show a specific plan
* `/next` view the next plan
* `/prev` view the previous plan
* `/manual` manual mode (do not respond to other user updates)
* `/auto` automatic mode (highlight relevent selections from others)
* `/export` export current plan as SVG
* `/?` help
* `free format text` broadcast message

## Key bindings

* **z** or **=**  (zoom-in)
* **x** or **-** (zoom-out)
* **ArrowRight** (pan-right)
* **ArrowLeft** (pan-left)
* **ArrowUp** (pan-up)
* **ArrowDown** (pan-down)
* **A-ArrowRight** or **C-ArrowRight** (next-plan) *use Alt- or Control- key*
* **A-ArrowLeft** or **C-ArrowLeft** (prev-plan)
* **1** (reset) *zoom out to 100%*
* **p** (list-plans)

## Development status and Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details on
how to make a contribution.

*NOTE* The tests are (obviously) incomplete!


## Copyright and license

Copyright © 2016 Dynamic Object Language Labs Inc.

Licensed under the [Apache License 2.0](http://opensource.org/licenses/Apache-2.0) [LICENSE](LICENSE)
