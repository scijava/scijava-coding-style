[![](https://travis-ci.org/scijava/scijava-coding-style.svg?branch=master)](https://travis-ci.org/scijava/scijava-coding-style)

# scijava-coding-style

This Maven artifact contains Eclipse coding style settings, intended for use with `pom-scijava`.

## Installation

The parent POM of your project needs to be `pom-scijava` at version 28.0.0 or later.

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

Two coding styles are supported: `scijava` and `imglib2`.
The default setting is `scijava`.
To change this, set the `coding-style` property in your Maven POM. For example:
```
<properties>
    <scijava.coding-style>imglib2</scijava.coding-style>
</properties>
```
