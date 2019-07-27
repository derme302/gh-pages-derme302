---
id: 118
title: 'Cookie &#8211; Surfaces in GameMaker: Studio'
date: 2014-05-31T02:25:41+00:00
author: Derme
layout: post
guid: http://derme.coffee/?p=118
permalink: /2014/05/surfaces-in-gamemaker-studio/
image: /uploads/2014/05/banner_image-624x159.png
categories:
  - GameMaker
tags:
  - guide
---
Getting started with drawing to a surface in GameMaker can be scary, especially when you see all the warnings and mystical properties that are associated with them.

The good news is that in reality, there isn't really that much to them. In the latest release of GameMaker 1.3 the main draw area IS a surface. So you're working with them already, you just don't know it.

The main thing you have to remember about surfaces is they aren't guaranteed to be there, just like biscuits in a biscuit jar, so you have to check they exist before drawing (or eating).

So to get started with surfaces you have to create one, if it doesn't already exist that is!

<pre class="EnlighterJSRAW" data-enlighter-language="c">if (!surface_exists(surf))
     surf = surface_create(width, height);
</pre>

Then you set the target, all drawing after this will be done to the surface.

<pre class="EnlighterJSRAW" data-enlighter-language="c">surface_set_target(surf);
// Here you just draw as normal
// i.e draw_sprite(sprite, subimg, x, y);
</pre>

Then once you're done set it back to the application surface. (The standard draw area)

<code class="EnlighterJSRAW" data-enlighter-language="c">surface_reset_target();‏</code>

Finally you draw the surface to the screen.

<code class="EnlighterJSRAW" data-enlighter-language="c">draw_surface(surf, x, y);</code>

You can download a example of this from [GitHub](https://github.com/derme302/gms-guide-surfaces), just navigate to the page a click &#8220;Download Zip&#8221;.

So really drawing to a surface isn't difficult, it just takes a little getting used to. Still have a question? Leave a comment or go ask the very helpful folks at the [GameMaker Community](http://gmc.yoyogames.com/index.php?showforum=2).