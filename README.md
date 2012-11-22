Punches
=======

Punches is a tool to create holes in your web pages. It works only with some CSS3 and a few lines of HTML.

Usage
=====

You only need the file `punches.less` to make it work.  
Other files are for example and testing purpose.

### HTML

```
<div class="punch" style="">
  <div class="white">
    <div class="in">
      <div class="content">
	    <!-- Put your content here if you want to. -->
      </div>
    </div>
  </div>
</div>
```

### LESS

First of all, you have to import the style file.  
Then, you just have to call the mixin.

```
@import "punches";

#your-punch {
  .punch(@size: 100px, @left: 0px, @top: 0px, @background: none, @grid: false, @z-index: 0);
}
```
You can see that every parameters have default values. So, you can just call `.punch;` if you want to.

Dependencies
============

Punches needs [LESS](http://lesscss.org) to work.
