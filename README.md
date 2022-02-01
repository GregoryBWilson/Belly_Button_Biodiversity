The data is structured as an object that contains three keys at the top level: `metadata`, `names`, and `samples`. Each of these keys is associated with an array that contains 153 elements.

data.names

```
function init() {
  // Grab a reference to the dropdown select element
  var selector = d3.select("#selDataset");

  // Use the list of sample names to populate the select options
  d3.json("samples.json").then((data) => {
    var sampleNames = data.names;
```

data.metadata

```
function buildMetadata(sample) {
  d3.json("samples.json").then((data) => {
    var metadata = data.metadata;
```



```
function buildCharts(sample) {
  // 2. Use d3.json to load and retrieve the samples.json file 
  d3.json("samples.json").then((data) => {
  	var samples = data.samples;
```



OTU stands for Operational Taxonomic Unit

Uncaught (in promise) TypeError: data.map is not a function

forEach is the same error
