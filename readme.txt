=== Calendar FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, calendar, day, event, xml, as3, animation, skin, html, css
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

One of the most advanced Calendars on the web. Completely XML customizable without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without any Flash knowledge. You can modify the calendar's width and heigh and there are multiple background and shade properties. The text is HTML/CSS formatted and there is the ability to change skin for info box (event day). The features for cells/days are customizable and a other options are available on the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/calendar-fx.zip "Calendar FX Plugin") (that you have to install and activate) & [Free package](http://www.flashxml.net/free/download/calendar.zip "Calendar FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **calendar-fx** and copy the content of the **free package** there
3. If you copied the **free package** to a location different than the one above, go to **Calendar FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[calendar-fx][/calendar-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Calendar FX part of your theme, edit the template files and add `<?php calendarfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Calendar FX](http://www.flashxml.net/calendar.html "Calendar FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/calendar-fx/settings.xml`

= Additional settings file =

To embed the Calendar FX more than once, you will need another settings file. Let's assume your new file is called `settings2.xml`. Add `[calendar-fx settings="settings2.xml"][/calendar-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `calendarfx_echo_embed_code()` function call (for example `<?php calendarfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[calendar-fx]` and `[/calendar-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `calendarfx_echo_embed_code()` function call (for example `<?php calendarfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[calendar-fx width="600" height="300"][/calendar-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `calendarfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/calendar.html "Calendar FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/calendar-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/calendar.html "Calendar FX") is the utility that helps easily customize your Calendar FX to fit all your needs.