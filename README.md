# Initial Grid [Beta Version]

A small but powerful 12 column responsive grid system written in pure CSS. It has clearly structured code to increase the readability, that makes it very easy to conigure the code. It's build with mobile first design in mind and has 5 breakpoints. The grid works on IE9+ and all modern browsers. Download a polyfill for IE8 support.

## Quick Example
This example shows how easy it is to create a responsive lay-out with the grid for mutiple devices. The class names are kept as short as possible, which makes them easier to read comparing to other grids. Especially when you're dealing with a lot of markup.

```html
<section class="box">
  <div class="t12 m4"> t12  m4 </div>  
  <div class="t6 m4">  t6   m4 </div>  
  <div class="t6 m4">  t6   m4 </div>  
</section>
```

## Methods
|              	|    Tiny   	|   Small   	|   Medium  	|   Large   	|    Huge   	|
|:------------:	|:---------:	|:---------:	|:---------:	|:---------:	|:---------:	|
| Breakpoint   	|  <= 480px 	|  >= 481px 	|  >= 769px 	| >= 1025px 	| >= 1441px 	|
| Class prefix 	|  .t1 - 12 	|  .s1 - 12 	|  .m1 - 12 	|  .l1 - 12 	|  .h1 - 12 	|
| Forward      	| .tf1 - 12 	| .sf1 - 12 	| .mf1 - 12 	| .lf1 - 12 	| .hf1 - 12 	|
| Backward     	| .tb1 - 12 	| .sb1 - 12 	| .mb1 - 12 	| .lb1 - 12 	| .hb1 - 12 	|
| Offset       	| .to1 - 12 	| .so1 - 12 	| .mo1 - 12 	| .lo1 - 12 	| .ho1 - 12 	|
| Box          	|    .box   	            	            	            	            	|

Note: there is also the possibility to reset the forward, backward and offset methods. This can be done by adding -r to the method. As example if you have an offset on your medium breakpoint of .mo4 and you want to reset it on your large breakpoint, simply add .lo-r as a class name.

## Getting Started
First download the .zip at the top of the page or fork it on Github. After you download it just open the file and easily configure the code. If you want to use the grid immediately, just skip these steps and add the minified version in your HTML head.

Step 1: Change the max-width(1200px) to your desired value.
```css
.box {
  width: 100%;
  max-width: 1200px; /* changeable */
  margin: 0 auto;   
}
```

Step 2: Change the padding(15px) to your desired value.
```css
.t1, .t2, .t3, .t4, .t5, .t6, .t7, .t8, .t9, .t10, .t11, .t12,
.s1, .s2, .s3, .s4, .s5, .s6, .s7, .s8, .s9, .s10, .s11, .s12,
.m1, .m2, .m3, .m4, .m5, .m6, .m7, .m8, .m9, .m10, .m11, .m12,
.l1, .l2, .l3, .l4, .l5, .l6, .l7, .l8, .l9, .l10, .l11, .l12,
.h1, .h2, .h3, .h4, .h5, .h6, .h7, .h8, .h9, .h10, .h11, .h12 {
  float: left;
  position: relative;
  min-height: 1px;
  padding: 0 15px; /* changeable */
}
```

Step 3: Minify your customized grid and add it in your HTML head. Start building!
```html
<link rel="stylesheet" href="css/normalize.css"> <!--provides better cross-browser consistency in the default styling of HTML elements.-->
<link rel="stylesheet" href="css/initial.min.css"> <!--the initial grid system.-->
<link rel="stylesheet" href="css/main.css"> <!--your custom css styles.-->
```
