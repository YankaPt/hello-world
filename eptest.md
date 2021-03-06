# linterhub: engine output

| Metadata     |                                         |
| ------------ |-----------------------------------------|
| EP           | ep-lh-0018                              |
| Version      | 1                                       |
| Title        | linterhub: engine output         	    |
| Authors      | YankaPt              			    |
| Status       | Draft                                   |
## Abstract
This document describes the structure of engine output.

## Proposal
The output of each engine should is an array. Each item of array is described by:
- `path` - The path relative to the analysis root
- `messages` - List of messages in the path

## Messages
Messages is an array. Each item is a `message`. `message` is a JSON Schema object with the following properties:

| Property    | Type     | Required | Description |
| -           | :-:      | :-:      | -           |
| message          | string   | +        | The short description of the message |
| description      | string   | -        | The explanatory text of the message  |
| severity     | string      | +        | The severity of the message: “verbose”, “hint”, “information”, “warning” or “error” |
| line        | integer    | +        | The line where the message is located|
| lineEnd         | integer   | -        | The end line where the message is located (the same as line by default)|
| column          | integer   | -        | The column where the message is located |
| columnEnd          | integer   | -        | The end column where the message is located |
| ruleId          | string   | -        | The id of the rule that produced the message |
| ruleName          | string   | -        | The name of the rule that produced the message |
| ruleNs          | string   | -        | The namespace of the rule that produced the message |

