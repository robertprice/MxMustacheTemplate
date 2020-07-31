# MxMustacheTemplate

## Overview

This Mendix module provides an implementation of the [Mustache](https://mustache.github.io/) templating system for Mendix applications. 

## How to use the module

### Installing

The module can be installed directly from the App Store. Please assign the User security role to all roles that need to use this module.

### A Simple Example.

The Java Action FillTemplateJSON in the USE_ME folder takes a template String and JSON String returning a String with the resuling populated template. In this case, pass empty to the Partial template strings input.

![A simple example microflow calling FillTemplateJSON](assets/simplemicroflow.png "How to call FillTemplateJSON")

The data being passed looks like this

![JSON String data](assets/vJSONString.png)

The template string looks like this

![Template String](assets/vTemplateString.png)

The data is passed to FillTemplateJSON like this

![Calling FillTemplateJSON](assets/FillTemplateJSON.png)

This will return the following String

    <h1>Colors</h1>

    <li><strong>red</strong></li>
    <li>red</li>
    <li>green</li>
    <li>blue</li>

## Bugs

There are no known bugs.

## Contributing

This module can be found on GitHub at [https://github.com/robertprice/MxMustacheTemplate](https://github.com/robertprice/MxMustacheTemplate).

Dependencies are managed using Maven.

The module is based on the Java implementation and also uses GSON internally to map JSON to a Java Hashmap.

### Unit Testing

There are Unit Tests in the UnitTesting directory. These return a boolean that is true if the test passed, or false if not. This means there is loose coupling to the UnitTesting module and tests are only run if this is available. Please only commit if all tests pass.

To run the unit tests install the Unit Testing and Object Handling modules from the Mendix App Store.

## See Also

* [Mustache Language Specification](https://mustache.github.io/mustache.5.html)
* [Mustache Java](https://github.com/spullara/mustache.java)
* [Google GSON](https://github.com/google/gson)

## Author

Robert Price - [robertprice.co.uk](https://www.robertprice.co.uk)