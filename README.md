## Introduction

This module is an add-on to the [islandora_rest](https://github.com/discoverygarden/islandora_rest) module.
It allows for additional information to be returned.

## Current paths

`islandora/rest/v1/object/<PID>/derivatives`

This will return the derivative map for the object specified by `<PID>` in JSON.

`islandora/rest/v1/object/<PID>/full_info`

This will return the normal full object info returned by the `islandora_rest` modules
along with the derivative map in a JSON array.
```$JSON
{ 
   "object_info" : <normal object info JSON>,
   "derivative_info" : <derivative map for object> }
```

