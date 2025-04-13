# Salad Naming Convention
aka SNC, is an organization between executor developers to provide a unified scripting API for our scripters.

## Why?
Over the years scripting has gotten more and more complex to support multiple executors. This is because of the many unique naming conventions various executors use.

Consider the following scenario. You want to know if a function belongs to the executor or not. In order for this code to be cross compatiable with all executors code like this is needed:
```lua
local is_executor_closure = is_salad_closure or is_essence_closure or is_ronix_closure --[[ew]] or is_awp_closure or is_wave_closure
```
This is reality for scripters who want cross compatibilty in their scripts. Scripters shouldn't have to do such laborous work just to attain cross compatability. The SNC seeks to solve this problem using naming conventions everyone agrees upon and follows.

One variant of a script should naturally work on all script executors which have their environment properly fitted to the SNC. 

## How?
The SNC provides standards for naming conventions as well as API functionality. The standard is written in markdown on this GitHub. Edits or additions are done through pull requests. Edits and additions are manually approved by the SNC council and discussed by everyone.

## Supporting SNC
As a product owner, your support of SNC by following the API will result in a far smoother experience for scripters, as they are able to work on scripts that they can confidently say will work on **most** products.

## Checking your environment

You can run the SNC environment checking script to see how well your executor environment supports the SNC standard. Find the script [here.](SNCCheckEnv.lua) The script determines what is missing, and writes the results to file under workspace.

## Contributing
Go [here](CONTRIBUTING.md) for a guide on contributing.