D'Anconia
=========

D'Anconia is my independent study project for Fall 2013. It is intended to be a web application with which one can build graph-based macroeconomic models of an equity's performance, and then use these models to predict the equity's value in specific scenarios.

### Example Workflow
Max wants to make money trading ExxonMobil (XOM). He researches the oil industry and related industries significantly before he creates a causal model of the macroeconomic effects which influence the stock's price.

In D'Anconia's *Model Builder* tab, Max drags out each macroeconomic effect onto an empty directed graph template, connects the nodes and assigns edge weights according to his perceived model.

Then in the *Events* tab, Max can drag out various macroeconomic events, set their parameters, and immediately see their effect on XOM according to his model. This tab is the primary focus of the project: a laboratory to quickly test different ideas about the future, given a subjective (but ideally well-researched) causal model of the stock's drivers.

### Model Builder Tab
  - Two panes:  Model graph and Events list
  - Drag events in Events list to graph; they transform into nodes
  - Click and drag to create edges between nodes
  - Click edges to set edge weights

### Events tab
  - Three panes:  Chosen events, Events list, and Outcomes
  - Can include multiple models to show multiple price outcomes
  - Click an outcome -> links to corresponding model in *Model Builder* tab

### My Models tab
  - A simple list of all the user's models
  - Click one -> links to corresponding model in *Model Builder* tab
  - This necessitates a login system, and a method of serializing each graph sensibly to generate persistent URLs to graphs

### Technologies
  - d3.js - JavaScript library to render nodes and edges of each graph
  - Bootstrap - frontend framework which makes overall layout painless
  - Ember.js - web framework for convenient templating and DOM updating
  - Node.js/Django - backend frameworks (I'll pick one.)
