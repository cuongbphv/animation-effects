# Animation Effects and SCSS Document
Repository is place to save animation effects which use HTML5, CSS3 and pure Javascript

### **Keywords in SCSS**
------
- @import : import partials, font, url, libraries,...
- @extend : inheritance in SCSS
- @include : use function by keyword @mixin
- @mixin : function in SCSS with parameter
- @if...@else : conditional in SCSS
- @for : loop for in SCSS with counter (from...through or from...to)
- @while : loop while in SCSS with counter
- @each : loop elements in list such as Maps
- map-get($map, $key) : map in SCSS get value by key
- @media : define properties CSS by screen and orientation

### **Work with variables**
------
- $variable : define variable
- #{$variable} : to access to variable in syntax or scope

*Variable* has 2 scope: **global** and **local**
1. Global: define outside function and selector, can use for all 
2. Local: define inside function and selector, can not use outside, only for it and children

### **Work with pseudo-classes and pseudo-elements**
------
- **&:before , &:after** : use to style to pseudo-elements
- **&:hover , &:active** : use to style for pseudo-classes