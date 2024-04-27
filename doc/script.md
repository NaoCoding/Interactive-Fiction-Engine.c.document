# Script 

### Overview

```
Inteactive Fiction Engine provides lots of script function to let users/developers
create a wonderful website with their own script.yaml.

However, users/developers should still follow the format of the script in order to
make the engine generate your website properly.

Therefore, this document aims to how users/developers write their script and
express one's idea to script.yaml
```


## Format of script

#### Background

* background: [ path ]
```c
background:[path]
// set the background image src to path
// ex. background:"images/background.png"
```

#### Window

* window.title: [ string ]
```c
window.title:[string]
// set the title of website
// ex. window.title:Hello World
```

#### Character

* character.count: [ uint ]
* character.create: [ string ]
  
* character.[ name ].src.[ string ]: [ path ]
* character.[ name ].show
* character.[ name ].hide
* character.[ name ].place:[string,string,string,string]
  
* character.[ name ].control.start
* character.[ name ].control.stop
* character.[ name ].control.movingAnimation:[uint,uint]
* character.[ name ].control.standingAnimation:[uint,uint]
* character.[ name ].moving_place:[string,string,string,string]
* character.[ name ].moving.[uint]:[path]
* character.[ name ].moving_src:[path]
* character.[ name ].moveAnimation

```c
character.count:[uint]
// set the amount of characters in the script
// required before adding any new character
// ex. character.count:3

character.create:[string]
// create a character named [string]
// name should be unique
// ex. character.create:howard

character.[name].src.[string]:[path]
// create a new image for character.[name]
// required [name] is created by character.create[name]
// ex. character.howard.src.normal_stand:"images/stand.png"

character.[name].show
character.[name].hide
// show/hide the character named [name]
// ex. character.howard.hide

character.[name].place:[string,string,string,string]
//set the character css style : width/height/left/top to [string,string,string,string]
//strongly recommend to set the style using percentage(%)

character.[ name ].control.start
// display characte.[name]'s moving_src and let player can control the character

```
