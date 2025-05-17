# glowing-journey
This guide explains how to use the Google Fonts API to add fonts to your web pages. You don't need to do any programming; all you have to do is add a special stylesheet link to your HTML document, then refer to the font in a CSS style.

# A quick example
Here's an example. Copy and paste the following HTML into a file:

<html>
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet"
          href="https://fonts.googleapis.com/css?family=Tangerine">
    <style>
      body {
        font-family: 'Tangerine', serif;
        font-size: 48px;
      }
    </style>
  </head>
  <body>
    <div>Making the Web Beautiful!</div>
  </body>
</html>

Then open the file in a modern web browser. You should see a page displaying the following, in the font called Tangerine:

# Making the Web Beautiful!
That sentence is ordinary text, so you can change how it looks by using CSS. Try adding a shadow to the style in the previous example:

body {
  font-family: 'Tangerine', serif;
  font-size: 48px;
  text-shadow: 4px 4px 4px #aaa;
}

You should now see a drop shadow under the text:

# Making the Web Beautiful!
And that's only the beginning of what you can do with the Fonts API and CSS.

# Overview
You can start using the Google Fonts API in just two steps:

1. Add a stylesheet link to request the desired web font(s):
   <link rel="stylesheet"href="https://fonts.googleapis.com/css?family=Font+Name">
2. Style an element with the requested web font, either in a stylesheet:
   .css-selector {font-family: 'Font Name', serif;}

or with an inline style on the element itself:
<div style="font-family: 'Font Name', serif;">Your text</div>

# Note: When specifying a web font in a CSS style, always list at least one fallback web-safe font in order to avoid unexpected behaviors. In particular, add a CSS generic font name like serif or sans-serif to the end of the list, so the browser can fall back to its default fonts if need be.

See a complete list of font families provided by the Google Fonts API on Google Fonts.
https://fonts.google.com/
