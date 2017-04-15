# css-grid

css-grid is a super simple, unobtrusive & light weight responsive grid.

No resets, defaults, or extra utility classes - just an easy to use and easy to comprehend, 12 column grid system. css-grid uses attributes rather than conventional css classes, to define the grid.

### Why?

A few years ago I was looking around for an unobtrusive, lightweight grid system for a couple of projects I was working on. After playing around with SASS, I eventually built a variant of css-grid. Working with [Angular Material's grid system](https://material.angularjs.org/latest/layout/introduction), I was inspired by the use of attributes to achieve responsive grid  control - css-grid is an attribute based adaption of my original simple grid system.

## Build
```
npm run build
```

## Usage

### Fluid grid

```html
<div row>
  <div col="4">4</div>
  <div col="4">4</div>
  <div col="4">4</div>
</div>
```
