---
title: Command Line
---

##Overview

Interaction with PredictionIO is done through the command line interface. It follows the format of: 

```pio <command> [options] <args>...```

You can run ```pio help``` to see a list of all available commands and ```pio help <command>``` to see details of the command.

PredictionIO commands can be separated into the following three categories. 

##General Commands
```help```          Display usage summary. `pio help <command>` to read about a specific subcommand.
  
```version```       Displays the version of the installed PredictionIO.

```status```        Displays install path and running status of PredictionIO system and its dependencies.


##Event Server Commands
```app```           Manage apps that are used by the Event Server. 

```pio app data-delete <name>``` deletes all data associated with the app. 
  
```pio app delete <name>``` deletes the app and its data.

```eventserver```   Launch an Event Server. 

  ```--ip <value>``` IP to bind to. Default to localhost. 
  
  ```--port <value>``` Port to bind to. Default to 7070.


```accesskey```     Manage app access keys.


##Engine Commands
Engine commands need to be run from the directory that contains the engine project. ```--debug``` and ```--verbose``` flags will provide debug and third-party informational messages.

```build```         Build the engine at the current directory. 

```train```         Kick off a training using an engine.

```deploy```        Deploy an engine as an engine server. If no instance ID is specified, it will deploy the latest instance. 



    

    
    

    



