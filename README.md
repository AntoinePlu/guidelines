# Guidelines

## Naming

### Folders

Dossier |
---|
cache |
public |
web |
models |
routers |
log |
collections |
lib |
bower_components |

### Code

```javascript
// global
app.models = {}
app.models.instances = {}
app.collections = {}
app.collections.instances = {}
app.views = {}
app.views.instances = {}
app.routers = {}
app.routers.instances = {}
app.events = {}

// function
{
  myMethod: function(){
  }
}

// variables
var myVar = "hello"
  , MY_CONST = "HELLO"

// instances
app.views.instances.myView = new app.views.MyView()

function MyConstructor(){
}

MyConstructor.create = function(){}
```

## Styles

BEM
