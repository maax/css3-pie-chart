# CSS3 Pie Chart

A SASS mixin for pure CSS pie charts.

## Usage

Based on the following HTML/HAML structure:

``` haml
#pie-chart
  - 4.times do
    .pie-chart-section
```

use the ``pie-chart()`` mixin in your SASS file like this:

``` sass

$sections: 60 red, 20 green, 10 blue, 10 black

#pie-chart
  +pie-chart($sections, $diameter: 400px)
```

with the following parameters:

    $sections   	  	// percentage and color of each section
    $diameter   	  	// in px
  	$initial-rotation 	// in degrees (default is 0°)
    $gradient   	 	// if you want a radial gradient (default is true)

## Browser Support
<table width="100%" style="text-align: center;">
  <thead>
    <tr>
      <td>Safari</td>
      <td>Chrome</td>
      <td>Firefox</td>
      <td>IE9</td>
      <td>IE10</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>✔</td>
      <td>✔</td>
      <td>✔</td>
      <td>✖</td>
      <td>✔</td>
    </tr>
  </tbody>
</table>