## .NET MVC Web API with Angular JS Bootstrapping Template

Visual Studio 2012 project to easily bootstrap AngularJS application into a .NET WEB API project.

Project contains basic framework in one easy project structure to easily create working AngularJS prototypes.

Utilises Bootstrap CSS and AngularJS via CDN, but also include in /SPA/vendor directory if required to work offline.

This project structure should only used be used for quickly prototyping .NET MVC WEB API applications in a demo or test environment.

### File Structure

The basic structure is generated using the Web API Empty Controller template in Visual Studio 2012

#### App_Data

.NET folder used to add data files. Accessible via 

```
HostingEnvironment.MapPath("@/App_Data/")
```

### App_Start

.NET MVC Web API configuration files that run on start up. 

### Controllers

.NET MVC Web API Controllers

### Models

POCO classes used to map data and to be returned to the UI.

### Services

Any service classes used to access data.

### SPA

Single page application file structure. Entry point index.html. 

``` 
app.module.js
```

AngularJS module definition file 

```
app.constants.js
```

AngularJS constants file - contains Web API uri that can be passed into AngularJS factories or sevices


Sub directories as follows:

#### controllers

AngularJS controllers

### css

All css should be added to the site.css file which is referenced in the index.html file.

### directives

AngularJS directives

### services

AngularJS services or factories

### views

Html views - this project assume only 1 view is required which is passed in via a ng-include directive in the index.html file.
For more complex scenarios would need to utilise ui-router and add to a config section of the root of the SPA directory.

## Utilities
Any additional CS classes should be added to this directory.
