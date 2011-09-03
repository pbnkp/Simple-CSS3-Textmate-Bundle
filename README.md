#Simple CSS3 Textmate Bundle
Making CSS3 "just work"...

##About

Adds cross-browser support for (most) CSS3 techniques. Yes, it even adds support (with some properties) to IE 6-9.

###**It adds Support for the following CSS3 properties**

*   `border-radius`
*   `@font-face`
*   `background-size`
*   `background-clip`
*   `box-shadow`
*   `text-shadow`
*   Linear Gradients
*   CSS3 Transitions

##Installation

`cd ~/Library/Application Support/TextMate/Bundles/`

if that directory wasn't found, you'll need to create it, then:

`git clone git://github.com/ekdevdes/Simple-CSS3-Textmate-Bundle.git "CSS3.tmbundle"`

##Documentation

The bundle only works when you are inside of a CSS file.

**round > tab**

*   Round all corners equally **round > tab > 1 > Amount of `border-radius` to apply**
	*   *Example:* If I wanted to round all corners equally with 6px I would do **round > tab > 1 > 6**
*   Round each corner separately **round > tab > 2 > (Amount of `border-radius` to apply > tab) x4**
*   Round only the top corners **round > tab > 3 > Amount of `border-radius` to apply**
	*   *Example:* If I wanted to round only the top corners 6px I would do **round > tab > 3 > 6**
*   Round only the bottom corners **round > tab > 4 > Amount of `border-radius` to apply**
	*   *Example:* If I wanted to round only the bottom corners 6px I would do **round > tab > 4 > 6**
*   Round only the bottom left corner **round > tab > 5 > Amount of `border-radius` to apply**
	*   *Example:* If I wanted to round only the bottom left corner 6px I would do **round > tab > 5 > 6**
*   Round only the bottom right corner **round > tab > 6 > Amount of `border-radius` to apply**
	*   *Example:* If I wanted to round only the bottom right corner 6px I would do **round > tab > 6 > 6**
*   Round only the left corners **round > tab > 7 > Amount of `border-radius` to apply**
	*   *Example:* If I wanted to round only the left corners 6px I would do **round > tab > 7 > 6**
*   Round only the right corners **round > tab > 8 > Amount of `border-radius` to apply**
	*   *Example:* If I wanted to round only the right corners 6px I would do **round > tab > 8 > 6**
*   Round only the top right corner **round > tab > 9 > Amount of `border-radius` to apply**
	*   *Example:* If I wanted to round only the top right corner 6px I would do **round > tab > 9 > 6**
*   Round only the top left corner **round > tab > 0 > Amount of `border-radius` to apply**
	*   *Example:* If I wanted to round only the top left corner 6px I would do **round > tab > 0 > 6**
*	Round every corner except the top right corner ** round > tab > Select "Round-Corners-Not-Top-Right"

**@ff > tab**

*	Cross-browser (even IE 6-9) @font-face ** @ff > tab > Web font name (can be anything) > tab > file name of font without the extension
	*	*Example:* If I have a font names "mywebfont.ttf" and I want to call it "My Web Font" in my CSS file I would do **@ff > tab > My Web Font (no quotes, done for you :)) > tab > mywebfont**
	*	The `@font-face` Texmate Snippet makes reference to a *.eof,.woff,.ttf* files, if you do not physically have these files than the cross-browser `@font-face` implementation will not be complete. To generate those font files for @font-face you must have the font you wish to use on your system in some format *.eot,.ttf,.dfont,.otf.woff* then you can head over to [The Font Squirrel @font-face generator](http://www.fontsquirrel.com/fontface/generator)
	*	If you are on a Mac, you can use any font on your system just go to Font Book (~/Applications/Font Book) Right Click on the font you want to use and Choose "Reveal in Finder" to get a font file that you can run [The Font Squirrel @font-face generator](http://www.fontsquirrel.com/fontface/generator) through. Sometimes the file you get will be a *.dfont* file though. Here's a [ a free Mac App ](http://peter.upfold.org.uk/projects/dfontsplitter) that can decompress that *.dfont* file for you. 
	
**bgsize > tab**

*	Apply to CSS3 `background-size` property to an element with cross-browser support **bgsize > tab > Amount of width as percentage (percent sign is added for you) > tab > Amount of height as percentage (percent sign is added for you)**

**shad > tab**

*	Text-shadow **shad > 1 > Amount of pixels for x-offsett > tab > Amount of pixels for y-offset > tab > Amount of pixels for shadow blur (0 for no sharp shadow with no blur) > tab > color of shadow in hexadecimal (without the # sign)**
	*	*Example:*  **shad > 1 > 2 > tab > 2 > tab > 0 > tab > ffffff** that would add a `text-shadow` with a x-offset of 2px, a y-offset of 2px, a blur of 0px and a shadow color ffffff (or white)	
*	Box-shadow **shad > 2 > Amount of pixels for x-offsett > tab > Amount of pixels for y-offset > tab > Amount of pixels for shadow blur (0 for no sharp shadow with no blur) > tab > color of shadow in hexadecimal (without the # sign)**
	*	*Example:*  **shad > 2 > 2 > tab > 2 > tab > 0 > tab > ffffff** that would add a `text-shadow` with a x-offset of 2px, a y-offset of 2px, a blur of 0px and a shadow color ffffff (or white)

**grad > tab**

*	Use CSS3 Linear Gradients with Cross-browser support (even in IE) **grad > tab > gradient beginning color (in hexadecimal, without # sign) > tab > gradient ending color (in hexadecimal, without # sign)**
	*	*Example:* **grad > tab > ffffff > tab > c6c6c6** would create a cross-browser CSS3 linear gradient with IE Support that goes from #ffffff to #c6c6c6 with #ffffff as the background color (for really old browsers that don't understand linear gradients)
	
**tran > tab**
*	Use CSS3 transitions with cross-browser compatibility **tran > tab > property to animate > tab > animation duration (without the 's') > tab > timing function**
	*	*Example:* **tran > tab > color > tab > 0.3 > tab > ease-out** this would create a cross-browser CSS3 transition that transitions the color property over 0.3 seconds and uses the "ease-out" timing function
	
**⌘ + ⇧ + P    (Prefixize)**

* Prefixize *
	*Usage: Select a single css declaration, an entire class, or your whole stylesheet then press CMD + SHIFT + P  and your css will automatically be prefixized. All the CSS3 browser prefixes like `-moz` and `-ms-` and `-webkit-`, even `-kthml` and `-o-` that all us designers need need to add to the new CSS3 properties like `border-radius` and such will automatically be added to your css file. Now you can you use only the W3C recommended syntax for CSS3 properties like `border-radius` and `linear-gradient` and `transition`. To prefixize your entire stylesheet and add cross-browser support for your css!
	*   **Disclaimer: Prefixize uses the API of Jeffrey Way's (of Nettuts+) new service Prefixr which was just released today in its Alpha release so if there are any issues please report them on Github...and ideally Prefixr.com too** 

##Support & Questions

If you have any questions you can [email me at ethankr@comcast.net](mailto:ethankr@comcast,net?subject=Simple-CSS4-Texmate-Bundle-Support)

[Prefixr by Jeffrey Way](http://prefixr.com)

##Thanks & Credits

This textmate bundle was made possible in large part by [CSS3 Please.com](http://css3please.com)

[Prefixr by Jeffrey Way](http://prefixr.com)

[@font-face cross-browser font generator](http://www.fontsquirrel.com/fontface/generator)

[Decompress .dfont files on the Mac](http://peter.upfold.org.uk/projects/dfontsplitter)

##License

SIMPLE CSS3 TEXTMATE BUNDLE IS DOUBLE LICENSED UNDER THE MIT LICENSE AND GPL LICENSE

MIT LICENSE

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

GPL LICENSE

A TextMate Bundle that adds cross-browser support for CSS3, enjoy!
    Copyright (C) 2011  Ethan Kramer

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.