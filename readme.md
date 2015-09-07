## Examples
Global gutters(for lg, md, sm, xs):
```sass
body {
  @include grid-gutters(20px, 10px, 10px, 10px);
}
````
Columns(3/12 for lg, 6/12 for md, 12/12 for sm, 12/12 for xs):
```sass
.gallery {
  @include row();
  .col {
    @include col(3, 6, 12, 12);
  }
}
```

Auto row, columns and clear:
```sass
.gallery {
  @include grid(3, 6, 12, 12);
}
```

Scope gutters:
```sass
.gallery {
  @include with-gutters(20px, 20px, 20px, 20px) {
    @include row();
    .col {
      @include col(4, 6, 12);
    }
  }
}
```


