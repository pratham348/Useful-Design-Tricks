# Useful-Design-Tricks
This repository is open to contribute for Design tricks

### Match the height of every card in list use this class
```
.match-height {
  > [class*='col'] {
    display: flex;
    flex-flow: column;

    > .card {
      flex: 1 1 auto;
    }
  }
}
```

### Mixins for responsive desinging (SCSS)
```
// responsive class

// Small tablets and large smartphones (landscape view)
$screen-sm-max: 576px;
// Small tablets (portrait view)
$screen-md-max: 768px;
// Tablets and small desktops
$screen-lg-max: 992px;
// Large tablets and desktops
$screen-xl-max: 1200px;
// Extra Large tablets and desktops
$screen-xll-max: 1399px;

// Small devices
@mixin sm {
  @media (max-width: #{$screen-sm-max}) {
    @content;
  }
}

// Medium devices
@mixin md {
  @media (max-width: #{$screen-md-max}) {
    @content;
  }
}

// Large devices
@mixin lg {
  @media (max-width: #{$screen-lg-max}) {
    @content;
  }
}

// Extra large devices
@mixin xl {
  @media (max-width: #{$screen-xl-max}) {
    @content;
  }
}

// Double Extra large devices
@mixin xll {
  @media (max-width: #{$screen-xll-max}) {
    @content;
  }
}
```
### Remove the selection of image
```
user-select: none;
```
