<p align="center">
  <a href="https://github.com/SlimDogs/sass-ultimate-boilerplate"><img src="https://github.com/SlimDogs/sass-ultimate-boilerplate/blob/master/docs/assets/logo.png?raw=true" alt="Sass ultimate boilerplate" height="200px"></a>
  <br>
  <br>
</p>

<p align="center">
  <a href="https://www.npmjs.com/package/sass-ultimate-boilerplate"><img src="https://badge.fury.io/js/sass-ultimate-boilerplate.svg" alt="npm version"></a>
  <a href="#" target="_blank"><img src="https://travis-ci.org/SlimDogs/sass-ultimate-boilerplate.svg?branch=master" alt="Latest CI build status" title="Latest CI build status"></a>
  <a href="https://github.com/SlimDogs/sass-ultimate-boilerplate" target="_blank"><img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic release" title="Semantic release"></a>
  <a href="https://greenkeeper.io" target="_blank"><img src="https://badges.greenkeeper.io/SlimDogs/sass-ultimate-boilerplate.svg" alt="Greenkeeper" title="Greenkeeper"></a>
  <a href="http://commitizen.github.io/cz-cli" target="_blank"><img src="https://img.shields.io/badge/commitizen-friendly-brightgreen.svg" alt="Commitizen friendly" title="Commitizen friendly"></a>
  <a href="https://www.npmjs.com/package/sass-ultimate-boilerplate" target="_blank"><img src="https://img.shields.io/npm/dw/sass-ultimate-boilerplate.svg" alt="NPM Downloads" title="NPM Downloads"></a>
  <a href="https://opensource.org/licenses/MIT" target="_blank"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License" title="MIT License"></a>
</p>

## Table of content
- [About](#about)
- [Installation](#installation)
- [How to use?](#how-to-use)
- [Features](#features)

## About
Sass boilerplate which is useful when starting a new web project. Includes: variables, functions, mixins, animations and other useful bits!

## installation
* If you are using yarn run `yarn add sass-ultimate-boilerplate --save`
* If you prefer npm run `npm install sass-ultimate-boilerplate --save`

## How to use
* In one of your sass files (preferably top of the root sass file) import sass-ultimate-boilerplate with a fallowing code:
```@import "~sass-ultimate-boilerplate/src/sass-boilerplate";```

## Features
## Animations
- [Float](#float)
- [Pulse](#pulse)
- [Spin](#spin)

## Functions
- [Pixels to rem](#pixels-to-rem)
- [Fixed Z index](#fixed-z-index)

## Mixins
- [Absolute](#absolute)
- [Blur](#blur)
- [Border radius](#border-radius)
- [Box shadow](#box-shadow)
- [Flex order](#flex-order)
- [Gradient](#gradient)
- [Animation and keyframes](#animation-and-keyframes)
- [Opacity](#opacity)
- [Parallax background](#parallax-background)
- [Placeholder](#placeholder)
- [Prefix or Vendorize](#prefix-or-vendorize)
- [Transition](#transition)

### Absolute
- `Type:` Mixin
- `Description:` Shortcut for setting position absolute with all positions containing same value

Usage:
```scss
div {
@include absolute(10px);
}
```

### Blur
- `Type:` Mixin
- `Description:` Vendorized blur

Usage:
```scss
.blured-text {
@include blur(0.8);
}
```

### Border-radius
- `Type:` Mixin
- `Description:` Vendorized border-radius shortcut

Usage:
```scss
.card {
@include border-radius(0.8);
}
```

### Box-shadow
- `Type:` Mixin
- `Description:` Vendorized box-shadow shortcut

Usage:
```scss
.element {
@include box-shadow(5px, 3px, 10px, #000);
}
```

### Flex-order
- `Type:` Mixin
- `Description:` Vendorized flex-order shortcut

Usage:
```scss
.card {
@include flex-order(-1);
}
```

### Gradient
- `Type:` Mixin
- `Description:` Comfortable way of setting css gradients!

Usage:
```scss
.test-1 {
@include linear-gradient(#31B7D7, #EDAC7D);
}

.test-2 {
@include linear-gradient(to right, #E47D7D 0%, #C195D3 50%, #4FB4E8 100%);
}

.test-3 {
@include linear-gradient(42deg, #B58234 0%, #D2B545 50%, #D7C04D 50.01%, #FFFFFF 100%);
}
```

### Animation and keyframes
- `Type:` Mixin
- `Description:` Vendorized animation & keyframes shortcut

Usage:
```scss
@include keyframes(slide-down) {
0% { opacity: 1; }
90% { opacity: 0; }
}

.element {
width: 100px;
height: 100px;
background: black;
@include animation('slide-down 5s 3');
}
```

### Media queries
- `Type:` Mixin
- `Description:` Easy media queries!

Usage:
```scss
.element {
width: 100px;
height: 100px;
background-color: black;

@include media-xs() {
background-color: white;
};
}
```

### Opacity
- `Type:` Mixin
- `Description:` Vendorized opacity shortcut

Usage:
```scss
.faded-text {
@include opacity(0.8);
}
```

### Parallax background
- `Type:` Mixin
- `Description:` Set parallax image backfround easy!

Usage:
```scss
div.msm-header {
@include parallax-background('/assets/images/header2_offset.jpg');
}
```

### Placeholder
- `Type:` Mixin
- `Description:` Easy way of setting placeholder stylings

Usage:
```scss
input.element {
@include placeholder {
font-style:italic;
color: white;
font-weight:100;
}
}
```

### Prefix or Vendorize
- `Type:` Mixin
- `Description:` Prefix or vendorize your style attributes

Usage:
```scss
span.icon {
@include prefix(transform, rotate(45deg), webkit ms);
}
```

### Transition
- `Type:` Mixin
- `Description:` Vendorized transitions

Usage:
```scss
a {
color: gray;
@include transition(color .3s ease);
}
```

### Float
- `Type:` Animation
- `Description:` Floating/hovering animation

Usage:
```scss
div {
@extend %animation-float;
}
```

### Pulse
- `Type:` Animation
- `Description:` Pulsing shadow/outline animation

Usage:
```scss
div {
@extend %pulse;
}
```

### Spin
- `Type:` Animation
- `Description:` 360deg infinite spinning animation

Usage:
```scss
div {
@extend %spin;
}
```

### Pixels to rem
- `Type:` Function
- `Description:` Convert pixels to rems easealy

Usage:
```scss
div {
height: pxToRem(45px);
}
```

### Fixed Z index
- `Type:` Function
- `Description:` Have and use a ordered and listed z-index values!

Usage:
```scss
div.header {
z-index: z('site-header');
}
```
