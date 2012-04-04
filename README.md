# CSS3 Pie Chart

A SASS/Compass mixin for pure CSS pie charts.

## Usage

Based on the follwing HTML/HAML structure

``` haml
%ul#pie-chart
  - 4.times do
    %li.section
      .section-fill
```

use the _pie-chart_ mixin in your SASS-file like this:

``` sass
$sections: red 20, orange 40, yellow 160, cyan 120, green 20
  
#pie-chart
  +pie-chart(300px, $sections)
```

Parameters

* $diameter (in px)
* $sections (color and degrees of each section)
* $gradient (if you want a radial gradient, default is true)

## Todo
1. allow sections > 180°
2. specify sections in %
3. test in non-Webkit browsers