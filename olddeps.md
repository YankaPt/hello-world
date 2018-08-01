# Olddeps
This schema describes the engine dependencies
## Structure
The engine dependencies

|Key|Type|Required|Description|
|-|:-:|:-:|-|
|id|string|-|The engine id|
|name|string|+|The engine name|
|dependencies|[dependencies](#dependencies)[]|+|The engine dependencies|
### requirement
The engine dependencies

|Key|Type|Required|Description|
|-|:-:|:-:|-|
|manager|[Manager](#/definitions/manager)|+|The manager for dependency|
|package|string|+|The package name|
|version|string|-|The package version|
|engine|boolean|-|The flag indicating whether it's engine itself|
## Example
```
```