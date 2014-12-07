# Palette -- a practical solution to establishing colorschemes on arbitrary sites

Palette is a wrapper around [color-schemer](https://github.com/at-import/color-schemer) to make it a bit more accessible and less coupled with the implementation of other scaffolding libraries associated with the parent project - all-your-base. Palette receives a single primary color and a coloring schemetype as input and generates a simple map with harmonizing colors and a scale of different values of grays. Subsequently this palette map can be passed as an argument to other all-your-base scaffolding tools to easily create a solid and decoupled foundation for any website development project. Simply pass the palette to the builder mixins and the sites colorscheme stays uniform across even dramatic changes.

## Example usage

```
@import 'palette';

$colors: (
  primary: #9955ff,
  scheme: accented-analogic
);

$palette: palette($colors);
```
