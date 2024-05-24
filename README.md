![banner](https://github.com/QuadSpinner/Gaea2Houdini_beta/blob/main/help/images/banner.png)


# Gaea2Houdini Beta
The Gaea 2.0 plugin for Houdini 20.0 and newer, developed by QuadSpinner.
By using this plugin you are able to use many of the nodes found inside Gaea directly inside Houdini. By using this plugin you are able to work interactively inside of Houdini, while using Gaea technology to create the desired end result.

## Installing for Houdini
To install the plugin for the first time, follow the below steps. Please note that the distribution of this toolset will change.
1. Clone this repository and make note of the directory you have cloned it to.
2. Copy the `Gaea2Houdini.json` file found in the repository root, and paste it in the $HOUDINI_USER_PREF_DIR/packages/ folder.
3. Edit the `Gaea2Houdini.json` file you just pasted, and modify the `$GAEA2HOUDINI` path found inside. Set the path to where you cloned the repository to in step one.
4. Open Gaea 2.0 and activate the software with your license if you have not yet done so.
5. Boot Houdini and enjoy!

## Using the Plugin
After installing the Gaea2Houdini plugin, open Houdini and create any `Gaea` node in your SOP network. It will automatically connect with Gaea 2.0 and process your input HeightField in Houdini. You can use these nodes the same way like any other SOP in Houdini. Most common use-cases have been tested already, while complex setups may not have been yet. Please let us know if things don't work as expected!

## Troubleshooting
So far there are no known issues.
- If you are having issues please contact QuadSpinner support.

## Notes
- We have provided a basic example file in this repo. You can find it in the `hip/` folder.
- The HDAs provided in this toolset are blackboxed. This means you cannot modify or inspect them yourself. If you are having issues please contact Quadspinner support.
- The Gaea nodes will look for an instance of the Gaea.Service.exe process running in the background, and if found connect to it for processing. If none is found, it will spin up a new instance.
-  Under `Advanced Cook Settings` in each Gaea node you are able to set the port used for the TCP communication between Houdini and Gaea. You are also able to configure the plugin to shut down the `Gaea.Service.exe` process down after each cook; Please note that this will incur significantly slower cooking times.
- This repository is a temporary place for beta testing. Actual contents will be moved to the official repository soon.

## LEGAL DISCLAIMER

The contents of this repository are provided as-is without any warranties, express or implied. Contents are copyright (C) 2024 QuadSpinner. All rights reserved.

Usage of Gaea through this plugin is governed by the [Gaea 2.0 End-User License Agreement](https://quadspinner.com/legal/#heading4)
