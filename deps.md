# Deps
Package dependencies
## Structure

### package
The definition of required package, later it should be converted to linterhub package reference

|Key|Type|Required|Description|
|-|:-:|:-:|-|
|manager|[ /Collectionmanager](./collection.md#/definitions/manager)|+|The package manager name|
|package|string|+|The package name in a format accepted by package manager|
|version|string|-|The package version in a format accepted by package manager, if not specified the latest version is assumed|
|target|boolean|-|The flag indicating whether the package is the target itself|
## Example
```
```