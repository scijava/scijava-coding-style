# scijava-coding-style

This  maven artifact contains Exclipse coding styles settings, that are intended to be used with `pom-scijava`.

## Installation
**PLEASE NOTE: This PR needs to be merged first: https://github.com/scijava/pom-scijava/pull/85**

The parent pom of your project needs to be `pom-scijava`.

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
