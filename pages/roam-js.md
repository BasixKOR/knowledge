---
title: roam/js
---

- {{[[roam/js]]}}
	 - ```javascript
let id = "roam-garden-plantsman"
let existingRg = document.getElementById(id)
if (!existingRg) {
    const extension = document.createElement("script")
    extension.src = "https://resources.roam.garden/js/plantsman.min.js"

    extension.id = id
    extension.async = true
    extension.type = "text/javascript"
    document.getElementsByTagName("head")[0].appendChild(extension)
}
```
