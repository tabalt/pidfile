
pidfile
---

Golang package for create and clear pid file.


### Version

V1.1.0

### Useage

```
package main

import (
    "github.com/tabalt/pidfile"
)

func main() {
    pf, _ := pidfile.Create("./tmp/app.pid")
    defer func() {
        _ = pf.Clear()
    }()

    //...

}
```