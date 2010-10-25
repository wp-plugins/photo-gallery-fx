=== Photo Gallery FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, photo, image, gallery, as3, effect, animation, text, xml, slideshow, auto, frame, html, css, thumb, scroll, alignment
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

An original "Photo Gallery". Completely XML customizable, without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without any Flash knowledge. It's completely customizable and it uses the Image Scroller FX component with the same customizable variables of the scroller. It also adds many gallery properties, image transitions and text effects. The image scroller can be placed on different position. The properties of the Image Scroller FX like roll over behaviors, HTML/CSS formatted tooltip, vertical or horizontal alignment, thumb spacing, scrolling and speed properties, background and shade properties are also available.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/photo-gallery-fx.zip "Photo Gallery FX Plugin") (that you have to install and activate) & [Free package](http://www.flashxml.net/free/download/photo-gallery.zip "Photo Gallery FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **photo-gallery-fx** and copy the content of the **free package** there
3. If you copied the **free package** to a location different than the one above, go to **Photo Gallery FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[photo-gallery-fx width="600" height="400"][/photo-gallery-fx]` where you want the Flash to show up in your post/page. Don't forget to provide your own width and height values, since 600 and 400 are just examples
5. If you want to make the Photo Gallery FX part of your theme, edit the template files and add `<?php photogalleryfx_echo_embed_code(600, 400); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Photo Gallery FX](http://www.flashxml.net/photo-gallery.html "Photo Gallery FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/photo-gallery-fx/settings.xml`, `wp-content/flashxml/photo-gallery-fx/fxImageScroller/settings.xml` and `wp-content/flashxml/photo-gallery-fx/holder/settings.xml` files accordingly
7. To use your own images, upload them to `wp-content/flashxml/photo-gallery-fx/images/` and update the `wp-content/flashxml/photo-gallery-fx/images/thumbs.xml` and `wp-content/flashxml/photo-gallery-fx/images/big.xml` files accordingly

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[photo-gallery-fx width="600" height="400"]` and `[/photo-gallery-fx]`. If you made the Flash part of your theme, add the text as **the third argument** of the `photogalleryfx_echo_embed_code()` function call (for example `<?php photogalleryfx_echo_embed_code(600,400,"Alternative content"); ?>`).

= Additional settings file =

To embed the Photo Gallery FX more than once, you will need another set of settings file and (probably) another set of images. Let's assume your new files are called `settings2.xml`. Add `[photo-gallery-fx width="600" height="400" settings="settings2.xml"][/photo-gallery-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the fourth argument** of the `photogalleryfx_echo_embed_code()` function call (for example `<php photogalleryfx_echo_embed_code(600,400,"Alternative content","settings2.xml"); >`).

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/photo-gallery.html" Photo Gallery FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/photo-gallery-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/photo-gallery.html "Photo Gallery FX") is the utility that helps easily customize your Photo Gallery FX to fit all your needs.