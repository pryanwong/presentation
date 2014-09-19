---
title       : Canadian Federal Civil Service Employees by Region
subtitle    : View by Year
author      : Sean Ferenci, P.Eng.
job         : Developing Data Products Student
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Canadians Want to Know

1. Where Federal Jobs are located
2. How many jobs are in the National Capital Region
3. They want to be able to see job shifts over time

--- .class #id 

## What My App Does

1. It lets users view federal employment numbers by province
2. They can change the year through a simple selection box
3. Users can seperate the national capital region from Ontario and Quebec data

--- .class #id

## A Typical Chart

<!-- BarChart generated in R 3.1.1 by googleVis 0.5.5 package -->
<!-- Thu Sep 18 22:04:20 2014 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataBarChartID287c10cd5df3 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "NL",
4605 
],
[
 "PE",
3119 
],
[
 "NS",
10598 
],
[
 "NB",
7899 
],
[
 "QC",
56465 
],
[
 "ON",
118270 
],
[
 "MB",
10326 
],
[
 "SK",
5957 
],
[
 "AB",
14447 
],
[
 "BC",
22801 
],
[
 "YT",
363 
],
[
 "NT",
487 
],
[
 "NU",
285 
],
[
 "Abroad",
1516 
] 
];
data.addColumn('string','Province');
data.addColumn('number','Employees');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartBarChartID287c10cd5df3() {
var data = gvisDataBarChartID287c10cd5df3();
var options = {};
options["allowHtml"] = true;
options["isStacked"] = false;
options["orientation"] = "horizontal";
options["hAxis"] = {title:'Province or Territory',format:'####'};
options["vAxis"] = {title: 'Employees'};
options["legend"] = {position: 'none'};
options["width"] =   1000;
options["height"] =    500;
options["title"] = "Federal Employees by Province for  2014 ";

    var chart = new google.visualization.BarChart(
    document.getElementById('BarChartID287c10cd5df3')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "corechart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartBarChartID287c10cd5df3);
})();
function displayChartBarChartID287c10cd5df3() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartBarChartID287c10cd5df3"></script>
 
<!-- divChart -->
  
<div id="BarChartID287c10cd5df3" 
  style="width: 1000; height: 500;">
</div>

--- .class #id 

## About the Chart

1. Data was taken from the Open Government site of the Canadian Government
2. Easy to read and Understand
3. Google bar chart implementation with HTML5 makes it easy for users to get precise figures by hovering over areas of interest


--- .class #id




