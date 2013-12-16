# Guidelines

## Folders / files

Names in folder / files are separated by dashes. Always use dashes. Some conventions about plural and exceptions are explained just below.

Folder |
---|
cache/ |
public/ |
log/ |
lib/ |
bin/ |
web/ |
vendor/ |
models/ |
routers/ |
collections/ |
index.js |
list.js |
list-item.js |
grunt-tasks/ |
bower_components/ |
node_modules/ |


## JavaScript

#### Namespace

Namespaces are in PascalCase: ```App.Core.Views```.

#### Classes

There's no real class (yet) in JavaScript but functions you have to instanciate are in PascalCase: ```new Class()```.

#### Function

Function are in camelCase: ```myFunction = function()```.

#### Global objects

Objects which aren't an instance of a _class_ and have to be global are in PascalCase: ```Browser```, ```Moment```.

Not answer yet for singleton. Have to think about it.

#### Constantes

```MY_CONSTANT_IS_BEAUTY = true```

#### Some examples

```javascript
// namespace
App.Core.Models = {}
App.Core.Collections = {}
App.Core.Views = {}
App.Core.Routers = {}
App.Instances.Models = {}
App.Instances.Collections = {}
App.Instances.Views = {}
App.Utils = {}
App.Events = {}

// function
{
  myMethod: function( opts ) {
  }
}

// variables
var myVar = "hello"
  , MY_CONST = 100

// instances
App.Instances.Views.myView = new App.Core.Views.MyView()
// or
var myView = App.Core.Views.MyView()

// constructor
function MyConstructor(){
}

MyConstructor.create = function(){}

// scope
;(function( win, doc, App ) {

// your code here

})( window, window.document, window.App || (window.App = {}) )

```

## CSS

BEM

```
org-(js-)-Block-element--modifier
```

An exemple: ```kud-(js-)-MyAlert-thisContent--hiddenStatus```
