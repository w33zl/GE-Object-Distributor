# GE Object Distributor

At the heart of it, _Object Distributor_ is a script for Giants Editor that will replace any number of objects with any custom object, similar to an advanced search and replace. The script can be used to place trees, light poles or other objects on a map. This is especially useful in combination with a random/procedurally generated collection of objects (destination markers).

The script gives control on the rotation and tilt of the replaced object and also support different kinds of randomization (e.g. rotation and angle of trees or placing rocks of different sizes).

![image](https://user-images.githubusercontent.com/7383510/155875595-58f485cf-1d14-4687-ad35-6eb44cbd7eb7.png)


## Like the work I do?
I love to hear you feedback so please check out my [Facebook](https://www.facebook.com/w33zl). If you want to support me you can become my [Patron](https://www.patreon.com/wzlmodding) or buy me a [Ko-fi](https://ko-fi.com/w33zl) :heart:

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/X8X0BB65P) [![Support me on Patreon](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dwzlmodding%3F%26type%3Dpatrons&style=for-the-badge)](https://patreon.com/wzlmodding?)


## Features
* Use tilt/angle/rotation from target or use random values (see settings)
* Random tilt/angle (X & Z axis)
* Fixed tilt/angle offset (X & Z axis)
* Random rotation (Y axis)
* Randomly choose source object from a collection of objects (e.g. different sized objects)

## Installation
1. Download the zip archive
2. Extract the contents to a temporary place
3. Copy the entire `"WZL Object Distributor"` folder to the `"%LocalAppData%\GIANTS Editor 64bit 9.0.2\scripts\"` folder _(you might need to change the version number if using a different version of Giants Editor)_
   * Optionally you could also drag-and-drop the `"WZL Object Distributor"` folder onto the supplied shortcut *(only works if you are using version 9.0.2)*
4. (Re)start Giants Editor

## Prepare (getting started)
The script requires a node (transform group) with two child nodes ("source" and "target"). You can either set this up manually or use the supplied _Configure Node_ script (recommended).

**This is the expected node structure:**
```
- "Main node"
  - source
    - (one or more sourece objects)
  - target
    - (one or more target objects/destination markers)
```

> Note: The name of the main node doesn't matter, however "source" and "target" must have these exact names (unless specifically configured otherwise, see "Configure" section below) *


### Configure
After running the _Configure Node_ script you should have a number of settings/configurations on your main node. These settings control the behaviour of the _Distribute Objects_ script.

## Usage (replace objects)

1. Add one (or more) source objects as childs to the "source" node
2. Add one (or more) target objects as childs to the "target" node
3. Select the main node
4. Execute _Distribute Objects_ script.
5. Check the log for errors and warnings

Please refer to the [user guide](UserGuide.pdf) for more details.
