All leaf.js plugins are written in common module pattern. It will require a common module compatible script loader like [leaf-require](https://github.com/NStal/leaf-require) to load.

Plugins should looks like below:

```coffee-script
class CustomHelper extends Leaf.EventEmitter
    constructor:()->
        return
module.exports = CustomHelper
```


And used like below(using leaf-require):
```coffee-script
CustomHelper = require "/components/customHelper"
helper = new CustomHelper()
```


