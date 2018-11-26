# reproduce

``` bash
$ yarn run stylelint app.sass --fix
```

# Result

```sass
$mobile: 640px

%hoge
  margin: 10px

=pc
  @media screen and (min-width: $mobile + 1px)
    @content

.ToggleSwitch
  @extend .hoge

.ToggleSwitch
  @extend .hoge
  padding: 10px
  border: 1px solid black

  +fuga
    padding: 20px
    border-color: blue

```


fix to

```sass
$mobile: 640px

%hoge
  margin: 10px


.ToggleSwitch

  padding: 10px
  border: 1px solid black
```
