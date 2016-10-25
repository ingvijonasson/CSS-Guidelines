#CSS Guidelines


## Basics

Use two spaces or one tab for indentation

```css
p {
  color: deepskyblue;
}
```

One selector per line:

```css
p,
li {}
```

Comments should always appear on a separate line and always top and never behind the declaration:

```css
/* Module */
.box {}
```

Leave a space after a colon:

```css
color: #efefef;
```

Use color shortcodes whenever possible because it is more readable:

```css
color: #000;
```

##Declaration order

It is a good practise to write CSS in some order. Alternatively you can use a tool such as [css comb](http://csscomb.com/).

```css
.selector {

  /* Positioning */
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 100;

  /* Box-model */
  display: block;
  float: right;
  margin: 0;
  padding: 0;
  width: 100%;
  height: auto;

  /* Typography */
  font: normal 13px "Helvetica Neue", sans-serif;
  line-height: 1.5;
  color: #333;
  text-align: center;

  /* Visual */
  background-color: #f5f5f5;
  border: 1px solid #e5e5e5;
  border-radius: 3px;

  /* Misc */
  transform: skew(30deg, 20deg);
  transition: background-color .3s;
  opacity: 1;
}
```

## Tips

Never use `id`s for styling, it simply makes things more complicated. Use classes. 

If a classname has any JavaScript attached to it prefix it with `js-` and make sure you do not style that class as well.
 
Use BEM. If you do not like BEM come up with another naming scheme and stick with it. 

Learn itcss. 
