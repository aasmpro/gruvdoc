check [mkdocs-material/code-blocks](https://squidfunk.github.io/mkdocs-material/reference/code-blocks/) for more information.

### Specifying the language
```
 ``` python
 import tensorflow as tf
 ```
```

```python
import tensorflow as tf
```

### Showcases
#### python
```python
from People import Person as PersonClass

# a random comment!
class MyPersonClass(PersonClass):
    """
    simple class to represent a person
    """
    name = "some default name"
    age = 20
    data = [1, 2.3, (4,), {"key": "value"}]

    def __init__(self):
        super().__init__()
    
    @property
    def in_10_years(self):
        return self.age + 10
```
#### javascript
```javascript
import React from "react";
import ReactDOM from "react-dom";

import { BrowserRouter } from "react-router-dom";

// Redux
import Store from "./store";
import { Provider } from "react-redux";

// App
import App from "./App";

// CSS
import "./assets/css/main.min.css";

ReactDOM.render(
  <BrowserRouter>
    <Provider store={Store}>
      <App />
    </Provider>
  </BrowserRouter>,
  document.getElementById("root")
);
```
#### css
```css
[data-md-color-accent="orange"] {
  --md-accent-fg-color: var(--color-orange0);
  --md-accent-fg-color--transparent: var(--color-orange0-rgba01);
  --md-accent-bg-color: var(--color-orange0-rgba09);
  --md-accent-bg-color--light: var(--color-orange0-rgba05);
}

#id .class {
    color: red;
}
```
#### html
```html
<head>
    <title>Page Title</title>
</head>
<body>
    <h1>Hello World!</h1>
    <p id="anId" class="text-red">
        we still here... :):
    </p>
</body>
```
#### yaml
```yaml
## Theme settings
theme:
  name: material
  favicon: assets/images/favicon.png
  features:
    - navigation.tabs
  palette:
    scheme: gruvbox
    primary: green
    accent: green
  icon:
    logo: assets/images/favicon.svg
  logo: assets/images/favicon.svg
```
#### json
```json
{
    "name": "random name",
    "age": 123,
    "data": [
        {
            "title": "random title"
        }
    ]
}
```

### Line numbers
```
 ```python linenums="1"
 def bubble_sort(items):
     for i in range(len(items)):
         for j in range(len(items) - 1 - i):
             if items[j] > items[j + 1]:
                 items[j], items[j + 1] = items[j + 1], items[j]
 ```
```
```python linenums="1"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

### Highlighting specific lines
```
 ```python hl_lines="2 3"
 def bubble_sort(items):
     for i in range(len(items)):
         for j in range(len(items) - 1 - i):
             if items[j] > items[j + 1]:
                 items[j], items[j + 1] = items[j + 1], items[j]
 ```
```
```python hl_lines="2 3"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```
Line ranges can also be used for conveniently specifying multiple lines.
```
 ```python hl_lines="2-5"
 def bubble_sort(items):
     for i in range(len(items)):
         for j in range(len(items) - 1 - i):
             if items[j] > items[j + 1]:
                 items[j], items[j + 1] = items[j + 1], items[j]
 ```
```
```python hl_lines="2-5"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

### Highlighting inline code blocks
```
The `#!python range()` function is used to generate a sequence of numbers.
```
The `#!python range()` function is used to generate a sequence of numbers.

### Adding keyboard keys
```
++ctrl+alt+del++
```
++ctrl+alt+del++