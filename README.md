## What?

Bring your Cinema4D light-setup from Cinema4D to Houdini with the click of a button!
## Why?

At the moment is FBX the standard format to transfer scenes between different software. The problem is that FBX does not recognize a plugin data and just throws it away.
It is handy to have exactly the same light-setup in both the software-packages.
Otherwise the simulation's will not align  when brought together.
## How?

First place the script in `\AppData\Roaming\MAXON\{cinemaversion}\library\scripts`
Inside cinema4D, copy the lights you want to export into a new scene.
Select the lights, run the script and select a location to export the .json and .fbx.

![b6f94ff2bc3d9c61472fbcd84554e7b8](https://user-images.githubusercontent.com/44348300/49300374-59aad200-f4c2-11e8-99bd-6692a7d9fedb.png)

Open Houdini, open the source editor and run HoudiniC4D_importer.py, select the .json and the lights are imported.


![0ff36ec841eb3d64d4298753de060f3f](https://user-images.githubusercontent.com/44348300/47940627-8bdd0a00-deeb-11e8-89af-e0f9c20ff044.png)


### what does not work?

Only works for physical lights (you should use them 99% of the time).

In Earlier versions of Redshift there is a problem, take the latest.

Path select with ``$HIP/Desktop/`` in Houdini does not work.

Just insert ``C:/Users/Desktop/`` as path.
