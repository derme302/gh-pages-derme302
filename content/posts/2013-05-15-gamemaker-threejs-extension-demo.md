---
id: 26
title: 'GameMaker: ThreeJS Extension &#038; Demo!'
date: 2013-05-15T05:20:00+00:00
author: Derme
layout: post
guid: http://derme.coffee/2013/gamemaker-threejs-extension-demo/
permalink: /2013/05/gamemaker-threejs-extension-demo/
blogger_blog:
  - derme.blogspot.com
blogger_author:
  - Derme
blogger_permalink:
  - /2013/05/gamemaker-threejs-extension-demo_15.html
blogger_internal:
  - /feeds/6224486094781961260/posts/default/8537451408083134917
image: /wp-content/uploads/2013/05/Screen-Shot-2013-05-10-at-10.29.09-PM-624x464.png
categories:
  - GameMaker
---
Those of you that [follow me on Twitter](https://twitter.com/Derme302) will know that I&#8217;ve spent the last week working on integrating the ThreeJS (r58) library with GameMaker: Studio. Now if you are already bursting with excitement you can skip to the end of the post for a link to the working demo!

[<img class="aligncenter" src="http://derme.coffee/wp-content/uploads/2013/05/Screen-Shot-2013-05-10-at-10.29.09-PM-300x223.png" alt="" width="320" height="238" border="0" />](http://derme.coffee/wp-content/uploads/2013/05/Screen-Shot-2013-05-10-at-10.29.09-PM.png)

The most awesome thing about this extension is that you can still do all your input control, AI and GUI though the GameMaker canvas. I&#8217;ve done this by using the CSS attribute z-order to &#8220;stack&#8221; the GameMaker canvas over the WebGL Renderer, I&#8217;m not sure this is the most conventional way to achieve this but it was easy to implement and seems to work fine.

<div>
  <div>
    <a href="http://derme.coffee/wp-content/uploads/2013/05/blog_example.png"><img class="aligncenter" src="http://derme.coffee/wp-content/uploads/2013/05/blog_example-300x271.png" alt="" width="320" height="290" border="0" /></a>
  </div>
</div>

At the moment you can draw cubes, spheres and create lights however I plan to extend the extension over the coming months to allow custom models (.obj) to be used and textures. This is going to take a bit longer as I don&#8217;t have a huge amout of free time at the moment, so I decided to release it as-is and as the extension isn&#8217;t minified you can tweek it untill your heart is content or I release a update.

At the moment the following functions have been integrated, you&#8217;ll notice that some of them still aren&#8217;t complete. e.g. Lights don&#8217;t have a id yet so they can&#8217;t be deleted which I plan to add at a later stage, once I work out a solution to clearing scenes without creating memory leaks.

<div>
  <a href="http://derme.coffee/wp-content/uploads/2013/05/Screen-Shot-2013-05-10-at-10.59.39-PM.png"><img class="aligncenter" src="http://derme.coffee/wp-content/uploads/2013/05/Screen-Shot-2013-05-10-at-10.59.39-PM-300x143.png" alt="" width="320" height="152" border="0" /></a>
</div>

Finally my personal favourite the ability to still be able to use GameMaker&#8217;s room editor for level design, here is what the current demo level looks like:

<div>
  <a href="http://derme.coffee/wp-content/uploads/2013/05/Screen-Shot-2013-05-10-at-11.02.07-PM.png"><img class="aligncenter" src="http://derme.coffee/wp-content/uploads/2013/05/Screen-Shot-2013-05-10-at-11.02.07-PM-300x157.png" alt="" width="320" height="168" border="0" /></a>
</div>

That about wraps up everything, so how about trying out the demo? (Requires: Google Chrome)

<div>
  <a href="https://dl.dropboxusercontent.com/u/34458649/J3D/Release%204/demo_upd/index.html"><img class="aligncenter" src="http://derme.coffee/wp-content/uploads/2013/05/Demo_button.png" alt="" width="240" height="96" border="0" /></a>
</div>