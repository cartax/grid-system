# Grid System 2(Beta)
Grid System 2(Beta) is a responsive and desktop project and is based on sass and typescript.   



## Github   
<https://github.com/w3labkr/grid-system/>   



## Document   
Please see [Document](https://w3labkr.github.io/grid-system/) for more information.   



## Structure   
```
o
|-- dist
|   |-- component/
|   |-- essential/
|   |-- slim/
|   |-- grid-system-component.min.css
|   |-- grid-system-essential.min.css
|   |-- grid-system-slim.min.css
|   |-- grid-system.min.css
|   `-- grid-system.min.js
|-- LICENSE
|-- CHANGELOG
`-- README.md
```


## Installation   
```
| filename               | filesize | breakpoint | component |
|------------------------|----------|------------|-----------|
| grid-system.min.css    | 11.7kb   | o          | o         |
| grid-component.min.css | 1.05kb   | x          | o         |
| grid-essential.min.css | 11.7kb   | o          | x         |
| grid-slim.min.css      | 3.84kb   | x          | x         |
```

Link:   
```
<link rel="stylesheet" href="path/to/grid-system.min.css" />
<link rel="stylesheet" href="path/to/grid-system-component.min.css" />
<link rel="stylesheet" href="path/to/grid-system-essential.min.css" />
<link rel="stylesheet" href="path/to/grid-system-slim.min.css" />
```

CDN:   
```
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/grid-system/dist/grid-system.min.css" />
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/grid-system/dist/grid-system-component.min.css" />
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/grid-system/dist/grid-system-essential.min.css" />
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/grid-system/dist/grid-system-slim.min.css" />
```



## Usage   

### Breakpoints   
```
| breakpoints | classes     |
|-------------|-------------|
| 1920px      | .desktop-*  |
| 1440px      | .notebook-* |
| 1024px      | .tablet-*   |
| 767px       | .mobile-*   |
```



### Layout      
```
| layout        | class                             | value                         |
|-------------- |--------------------------------   |-----------------------------  |
| gutter        | .gutter-{value}                   | 5, 10, 15, 20, 25, 30         |
| container     | .container, .container-{value}    | fluid                         |
| column        | .columns, .column-{value}         | between number from 1 to 12   |
| column-count  | .column-count-{value}             | between number from 1 to 12   |
| row           | .rows, .row-{value}               | between number from 1 to 12   |
| row-count     | .row-count-{value}                | between number from 1 to 12   |
| cell          | .cells, .cell-{value}             | between number from 1 to 12   |
| cell-count    | .cell-count-{value}               | between number from 1 to 12   |
| order         | .orders, .order-{value}           | between number from 1 to 12   |
```

#### Example   
column:   
```
<div class="columns mobile-orders">
  <div class="column-3 mobile-order-2">content</div>
  <div class="column-6 mobile-order-1">content</div>
  <div class="column-3 mobile-order-3">content</div>
</div>
```

column-count:   
```
<div class="columns gutter-10 column-count-4 mobile-column-count-2">
  <div class="column">content</div>
  <div class="column">content</div>
  <div class="column">content</div>
  <div class="column">content</div>
</div>
```



### Alignment   
```
| alignment  | class                           | value                                 |
|------------|---------------------------------|---------------------------------------|
| text       | .text-{value}                   | left, center, right, justify          |
| horizontal | .align-{value}                  | left, center, right                   |
| vertical   | .aligns, .align-{value}         | top, middle, bottom                   |
| transform  | .translates, .translate-{value} | top, middle, bottom                   |
|            |                                 | topleft, topcenter, topright          |
|            |                                 | middleleft, middlecenter, middleright |
|            |                                 | bottomleft, bottomcenter, bottomright |
```

#### Example   

text:   
```
<div class="text-center notebook-text-left">
  ...
</div>
```

horizontal:   
```
<div class="align-left tablet-align-right">
  ...
</div>
```

vertical:   
```
<div class="aligns vh-100">
  <div class="align-middle">
    ...
  </div>
</div>
```

transform:   
```
<div class="translates">
  <div class="translate-middlecenter">
    ...
  </div>
</div>
```


### Display   
```
| display       	| value                                                                        	|
|---------------	|------------------------------------------------------------------------------	|
| .show         	| block                                                                        	|
| .hide         	| none                                                                         	|
| .show-{value} 	| block, inline, inline-block, flex, inline-flex, table, table-row, table-cell 	|
| .visible      	|                                                                              	|
| .hidden       	|                                                                              	|
```



### A11y   
```
| A11y          	| class               	|
|---------------	|---------------------	|
| Disabled      	| .disabled           	|
| IR Method     	| .ir-phark           	|
| Ellipsis      	| .ellipsis           	|
| Accessibility 	| .screen-reader-text 	|
```



### Font   
```
| font         | value                          | increase |
|--------------|--------------------------------|----------|
| font-{value} | between number from 10 to 90   | 10       |
| font-{value} | between number from 100 to 900 | 100      |
```



### Utility   

pixel:   
```
| class         | value                        | increase |
|---------------|------------------------------|----------|
| w-{value}     | between number from 0 to 100 | 10       |
| h-{value}     | between number from 0 to 100 | 10       |
| min-w-{value} | between number from 0 to 100 | 10       |
| min-h-{value} | between number from 0 to 100 | 10       |
```

percent:   
```
| class          | value                        | increase |
|----------------|------------------------------|----------|
| pw-{value}     | between number from 0 to 100 | 10       |
| ph-{value}     | between number from 0 to 100 | 10       |
| min-pw-{value} | between number from 0 to 100 | 10       |
| min-ph-{value} | between number from 0 to 100 | 10       |
```

viewport:   
```
| class          | value                        | increase |
|----------------|------------------------------|----------|
| vw-{value}     | between number from 0 to 100 | 10       |
| vh-{value}     | between number from 0 to 100 | 10       |
| min-vw-{value} | between number from 0 to 100 | 10       |
| min-vh-{value} | between number from 0 to 100 | 10       |
```



## Browser Support   
IE9+, Edge, Chrome, Firefox, Opera, Safari   



## Changelog   
Please see [CHANGELOG](CHANGELOG) for more information what has changed recently.   



## License   
Grid System 2(Beta) is licensed under the [MIT LICENSE](LICENSE)   