# attr-grid

attr-grid is a super simple, unobtrusive & light weight responsive grid.

No resets, defaults, or extra utility classes - just an easy to use and easy to comprehend, 12 column grid system. attr-grid uses attributes rather than conventional css classes, to define the grid.
[View Demo](https://rawgit.com/mooce/attr-grid/master/index.html)

### Why?

A few years ago I was looking around for an unobtrusive, lightweight grid system for a couple of projects I was working on. After playing around with SASS, I eventually built a variant of attr-grid. Working with [Angular Material's grid system](https://material.angularjs.org/latest/layout/introduction), I was inspired by the use of attributes to achieve responsive grid  control - attr-grid is an attribute based adaption of my original simple grid system.

### Build

Install npm dev dependencies.

```
npm install
```

Build the stylesheet.
```
npm run build
```

### Installation

#### Link stylesheet

Add the following to your HTML's `<head>` section:

```html
    <link rel="stylesheet" href="/dist/grid.css" type="text/css">
```

#### Viewport scales

Add the following to your HTML's `<head>` section:

```html
    <meta name="viewport" content="width=device-width, initial-scale=1">   
```

This meta tag ensures mobile and tablet resize page content to match the devices actual viewport width.

### Usage

#### Fluid grid

```html
  <div row>
    <div col="8">8</div>
    <div col="4">4</div>
  </div>
  <div row>
    <div col="12">12</div>
  </div>
```

#### Fixed grid

```html
<div fixed>
  <div row>
    <div col="8">8</div>
    <div col="4">4</div>
  </div>
  <div row>
    <div col="6">6</div>
    <div col="6">6</div>
  </div>
</div>
```

#### Nested grids

```html
  <div row>
    <div col="6">
      <div row>
        <div col="3">3 in 6</div>
        <div col="6">6 in 6</div>
      </div>
    </div>
    <div col="6">
      <div row>
        <div col="3">3 in 6</div>
        <div col="3">3 in 6</div>
        <div col="3">3 in 6</div>
      </div>
    </div>
  </div>
```
