[![](https://travis-ci.org/scijava/scijava-coding-style.svg?branch=master)](https://travis-ci.org/scijava/scijava-coding-style)

# scijava-coding-style

This Maven artifact contains Eclipse coding style settings, intended for use with `pom-scijava`.

## Installation

The parent POM of your project needs to be `pom-scijava` at version 27.0.0 or later.

## Usage

Code formatting for all java files can be done with the following command line:
```bash
$ mvn formatter:format
```
Sorting of java imports is supported as well:
```
$ mvn impsort:sort
```

## Configuration

Three coding styles are supported: `imagej`, `imglib2` and `scifio`.
The default setting is `imagej`.
To change this set the `coding-style` property in you maven pom. For examle:
```
<properties>
    <coding-style>imglib2</coding-style>
</properties>
```
