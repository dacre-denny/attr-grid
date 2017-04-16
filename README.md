# attr-grid

attr-grid is a super simple, unobtrusive & light weight responsive grid.

No resets, defaults, or extra utility classes - just an easy to use and easy to comprehend, 12 column grid system. attr-grid uses attributes rather than conventional css classes, to define the grid.
[View Demo](https://rawgit.com/mooce/attr-grid/master/index.html)

## Why?

I was looking around for an unobtrusive, lightweight grid system for a couple of projects I was working on. I eventually built a simple grid, and, after working with [Angular Material's grid system](https://material.angularjs.org/latest/layout/introduction), I was inspired by the use of attributes to achieve responsive grid  control. attr-grid is an attribute based adaption of my original simple grid system.

## Grid system

attr-grid is a 12 column grid system. 

Columns are spaced with a `10px` gutter.

Breakpoints for attr-grid are:

- sm: 600px
- md: 960px
- lg: 1280px

## Build

Install npm dev dependencies.

```
npm install
```

Build the stylesheet.
```
npm run build
```

## Installation

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

## Usage

#### Fluid grid

Use the `row` attribute on element to define a grid row. Add a `col` attribute to specify the column's width under that row:

```html
  <div row>
    <div col="8">eight column</div>
    <div col="4">four column</div>
  </div>
  <div row>
    <div col="12">tweleve column</div>
  </div>
```

#### Fixed grid

Use the `fixed` attribute on element wrapping the grid to achieve a center fixed grid:

```html
<div fixed>
  <div row>
    <div col="8">eight column</div>
    <div col="4">four column</div>
  </div>
  <div row>
    <div col="6">six column</div>
    <div col="6">six column</div>
  </div>
</div>
```

#### Nested grids

Nested grids are supported:

```html
  <div row>
    <div col="6">
      <div row>
        <div col="3">3 column in 6 column</div>
        <div col="6">6 column in 6 column</div>
      </div>
    </div>
    <div col="6">
      <div row>
        <div col="3">3 column in 6 column</div>
        <div col="3">3 column in 6 column/div>
        <div col="3">3 column in 6 column</div>
      </div>
    </div>
  </div>
```

#### Grid utilities

Maybe you need full width blocks, at certian breakpoints? No worries! Here's how:

```html
  <div row>
    <div col="8" col-md-block>eight column, full width on md breakpoint</div>
    <div col="4" col-md-block>four column, full width on md breakpoint</div>
  </div>
  <div row>
    <div col="6" col-sm-block>six column, full width on sm breakpoint</div>
    <div col="6" col-sm-block>six column, full width on sm breakpoint</div>
  </div>
```
