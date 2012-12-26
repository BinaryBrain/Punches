Punches
=======

Punches is a tool to create holes in your web pages. It works only with some CSS3 and a few lines of HTML.


Result
------

Here's an example of what you can do with Punches.

![Punches Screenshot](https://github.com/BinaryBrain/Punches/blob/master/readme-images/screenshot2.png?raw=true)

_Note: It uses only two images. The black background and the brushed metal._

Usage
-----

You only need the _punches.less_ file to make it work.  
Other files are for example and testing purpose.

### HTML

```
<div id="your-punch" class="punch">
  <div class="punch-white">
    <div class="punch-in">
      <div class="punch-content">
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
  //.punch(@size: 100px, @left: 0px, @top: 0px, @background: none, @grid: false, @z-index: 0);
  .punch(150px, 20px, 20px, black);
}
```
You can see that every parameters have default values. So, you can just call `.punch;` if you want to.

Dependencies
------------

Punches needs [LESS](http://lesscss.org) to work.

Example
-------

To see the example, just download the folder _example_.  
Note that the less code has been already compiled for you.
