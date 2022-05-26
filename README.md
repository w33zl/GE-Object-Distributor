# GE Object Distributor

At the heart of it, _Object Distributor_ is a script for Giants Editor that will replace any number of objects with any custom object, similar to an advanced search and replace. The script can be used to place trees, light poles or other objects on a map. This is especially useful in combination with a random/procedurally generated collection of objects (destination markers).

The script gives control of the rotation and tilt of the replaced object and also support different kinds of randomization (e.g. rotation and angle of trees or placing rocks of different sizes).

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
1. Download the [latest release](https://github.com/w33zl/GE-Object-Distributor/releases/download/v0.9.3-beta/GE_Object_Distributor_v0.9.3beta.zip) (zip archive)
2. Extract the contents to a temporary place
3. Copy the entire `"WZL Object Distributor"` folder to the `"%LocalAppData%\GIANTS Editor 64bit 9.0.2\scripts\"` folder _(you might need to change the version number if using a different version of Giants Editor)_
   * Optionally you could also drag-and-drop the `"WZL Object Distributor"` folder onto the supplied shortcut *(only works if you are using version 9.0.2)*
4. (Re)start Giants Editor

## Prepare (getting started)
The script requires a node (transform group) with two child nodes ("source" and "target"). You can either set this up manually or use the supplied _Configure Node_ script (recommended). 


Please refer to the [user guide](UserGuide.pdf) for detailed explanation.

**This is the expected node structure:**
```
- "Main node"
  - source
    - (one or more sourece objects)
  - target
    - (one or more target objects/destination markers)
```

> Note: The name of the main node doesn't matter, however "source" and "target" must have these exact names (unless specifically configured otherwise, see "Configure" section below) *

### Automatically configure node via the script
If using the script the child nodes "source" and "target" will be automatically created along with different settings available.

[![image](https://user-images.githubusercontent.com/7383510/155886082-24aeb8b3-9088-4a10-a444-24ea2c2703cc.png)](https://user-images.githubusercontent.com/7383510/155886155-06960e07-97cc-4f29-99a6-a7c666f1512d.png)


This is the expected output after running the script:

[![image](https://user-images.githubusercontent.com/7383510/155886127-d39d4ec1-586f-4740-9fcc-060b107271a9.png)](https://user-images.githubusercontent.com/7383510/155886191-02ee1173-9856-4077-a12c-39628c475059.png)



### Configure
After running the _Configure Node_ script you should have a number of settings/configurations on your main node. These settings control the behaviour of the _Distribute Objects_ script.

[![image](https://user-images.githubusercontent.com/7383510/155885792-78dea4b0-b234-49e5-872f-cf5b0f0d92d3.png)](https://user-images.githubusercontent.com/7383510/155885817-5b571e68-5280-4692-bc9d-f6e099cd0d2a.png)


## Usage (replace objects)

1. Add one (or more) source objects as childs to the "source" node
2. Add one (or more) target objects as childs to the "target" node
3. Select the main node
4. Execute _Distribute Objects_ script.
5. Check the log for errors and warnings

[![image](https://user-images.githubusercontent.com/7383510/155886272-f73ff98e-41f4-4fc2-920f-c4dae16c1fc5.png)](https://user-images.githubusercontent.com/7383510/155886264-90170bf3-77a3-4f93-8b11-e7fffaf338f0.png)


Please refer to the [user guide](UserGuide.pdf) for more details.
