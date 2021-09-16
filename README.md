[![](https://github.com/scijava/scijava-coding-style/actions/workflows/build-main.yml/badge.svg)](https://github.com/scijava/scijava-coding-style/actions/workflows/build-main.yml)

# scijava-coding-style

This Maven artifact contains Eclipse coding style settings, intended for use with `pom-scijava`.

There is also a `preferences.epf` you can import into the Eclipse IDE via _File > Import_.

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
    <coding-style>imglib2</coding-style>
</properties>
```
