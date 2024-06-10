#Object

### Overview

```
Object is an important part of our engine,
if you want to create some elements or button
for player to click ( not option during dialog ),
then object is what you may targeting for.
Object support various settings for users to create their script.
```

### Format of objects

```c
object.create.[name]  // create an object named [name]
// ex. object.create.door    ->  create an object named door


object.style.[name].[target]:[value] // css object [name] style [target] : set to value [value]
// ex. object.style.door.width:"10%"  -> document.findElementById("OBJECT_door").style.width = "10%"


object.place.[name].[width,height,left,top] // css object style for width,height,left,top in one line of script
// ex. object.place.door:"10%","10%","25%","25%"
// equals to
      object.style.door.width:"10%"
      object.style.door.height:"10%"
      object.style.door.left:"25%"
      object.style.door.top:"25%"

object.show.[name]
// show the object [name] (display : block)

object.hide.[name]
// hide the object [name] (display : none)

object.src.[name].[location]
// set the src of OBJECT_ to location
// ex. object.src.door."image/door.jpg"

object.click.subscene_open.[subscene_name]
// open a subscene while click the object

```
