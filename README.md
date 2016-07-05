# quindar-lineplot
Line plot directive to display spacecraft vehicle's sensors, temperature, battery, etc.  Idea inspired by angular-flot.

## Required Modules
Once you download the quindar-lineplot folder, you need to run buildme.sh in the example folder to install required modules. 

## How to Run the Demo
Go to the example folder and run server.js to open the local host port: 
  
    node server.js

## How to Integrate the Stand Alone Version to Quindar
1. Copy all files except index.html to appropriate Quindar folders.
1. Modify the Quindar index.html to add necessary source links.
1. Totally remove dependencies in app-lineplot.js by removing [] from the module definition line, 
  1. e.g., var app = angular.module('app')
1. Add 'app' as a dependency to angular-lineplot.js.
1. Comment out scopes from angular-lineplot.js.
1. Add controller: 'lineplotCtr', to angular-lineplot.js.
1. Modify widgetDefinitions and $scope.dashboard so that line plot widgets are available. 
