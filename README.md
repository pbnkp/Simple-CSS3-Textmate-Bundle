#Simple CSS3 Textmate Bundle

##About

Adds cross-browser support for (most) CSS3 techniques. Yes, it even adds support (with some properties) to IE 6-9.

###**It adds Support for the following CSS3 properties**

*   border-radius
*   @font-face
*   background-size
*   background-clip
*   box-shadow
*   text-shadow
*   Linear Gradients
*   CSS3 Transitions

##Installation

cd ~/Library/Application Support/TextMate/Bundles/

if that directory wasn't found, you'll need to create it, then:

git clone git://github.com/ekdevdes/Simple-CSS3-Textmate-Bundle.git "CSS3.tmbundle"

##Documentation

The bundle only works when you are inside of a CSS file.

**round > tab**

*   Round all corners equally **round > tab > 1 > Amount of border-radius to apply**
	*   *Example:* If I wanted to round all corners equally with 6px I would do **round > tab > 1 > 6**
*   Round each corner separately **round > tab > 2 > (Amount of border-radius to apply > tab) x4**
*   Round only the top corners **round > tab > 3 > Amount of border-radius to apply**
	*   *Example:* If I wanted to round only the top corners 6px I would do **round > tab > 3 > 6**
*   Round only the bottom corners **round > tab > 4 > Amount of border-radius to apply**
	*   *Example:* If I wanted to round only the bottom corners 6px I would do **round > tab > 4 > 6**
*   Round only the bottom left corner **round > tab > 5 > Amount of border-radius to apply**
	*   *Example:* If I wanted to round only the bottom left corner 6px I would do **round > tab > 5 > 6**
*   Round only the bottom right corner **round > tab > 6 > Amount of border-radius to apply**
	*   *Example:* If I wanted to round only the bottom right corner 6px I would do **round > tab > 6 > 6**
*   Round only the left corners **round > tab > 7 > Amount of border-radius to apply**
	*   *Example:* If I wanted to round only the left corners 6px I would do **round > tab > 7 > 6**
*   Round only the right corners **round > tab > 8 > Amount of border-radius to apply**
	*   *Example:* If I wanted to round only the right corners 6px I would do **round > tab > 8 > 6**
*   Round only the top right corner **round > tab > 9 > Amount of border-radius to apply**
	*   *Example:* If I wanted to round only the top right corner 6px I would do **round > tab > 9 > 6**
*   Round only the top left corner **round > tab > 0 > Amount of border-radius to apply**
	*   *Example:* If I wanted to round only the top left corner 6px I would do **round > tab > 0 > 6**
*	Round every corner except the top right corner ** round > tab > Select "Round-Corners-Not-Top-Right"

**@ff > tab**

*	Cross-browser (even IE 6-9) @font-face ** @ff > tab > Web font name (can be anything) > tab > file name of font without the extension
	*	*Example:* If I have a font names "mywebfont.ttf" and I want to call it "My Web Font" in my CSS file I would do **@ff > tab > My Web Font (no quotes, done for you :)) > tab > mywebfont**
	*	The @font-face Texmate Snippet makes reference to a *.eof,.woff,.ttf* files, if you do not physically have these files than the cross-browser @font-face implementation will not be complete. To generate those font files for @font-face you must have the font you wish to use on your system in some format *.eot,.ttf,.dfont,.otf.woff* then you can head over to [The Font Squirrel @font-face generator](http://www.fontsquirrel.com/fontface/generator)
	*	If you are on a Mac, you can use any font on your system just go to Font Book (~/Applications/Font Book) Right Click on the font you want to use and Choose "Reveal in Finder" to get a font file that you can run [The Font Squirrel @font-face generator](http://www.fontsquirrel.com/fontface/generator) through. Sometimes the file you get will be a *.dfont* file though. Here's a [ a free Mac App ](http://peter.upfold.org.uk/projects/dfontsplitter) that can decompress that *.dfont* file for you. 
	
**bgsize > tab**

*	Apply to CSS3 background-size property to an element with cross-browser support **bgsize > tab > Amount of width as percentage (percent sign is added for you) > tab > Amount of height as percentage (percent sign is added for you)**

**shad > tab**

*	Text-shadow **shad > 1 > Amount of pixels for x-offsett > tab > Amount of pixels for y-offset > tab > Amount of pixels for shadow blur (0 for no sharp shadow with no blur) > tab > color of shadow in hexadecimal (without the # sign)**
	*	*Example:*  **shad > 1 > 2 > tab > 2 > tab > 0 > tab > ffffff** that would add a text-shadow with a x-offset of 2px, a y-offset of 2px, a blur of 0px and a shadow color ffffff (or white)	
*	Box-shadow **shad > 2 > Amount of pixels for x-offsett > tab > Amount of pixels for y-offset > tab > Amount of pixels for shadow blur (0 for no sharp shadow with no blur) > tab > color of shadow in hexadecimal (without the # sign)**
	*	*Example:*  **shad > 2 > 2 > tab > 2 > tab > 0 > tab > ffffff** that would add a text-shadow with a x-offset of 2px, a y-offset of 2px, a blur of 0px and a shadow color ffffff (or white)

**grad > tab**

*	Use CSS3 Linear Gradients with Cross-browser support (even in IE) **grad > tab > gradient begining color (in hexadecimal, without # sign) > tab > gradient ending color (in hexadecimal, without # sign)**
	*	*Example:* **grad > tab > ffffff > tab > c6c6c6** would create a cross-browser CSS3 linear gradient with IE Support that goes from #ffffff to #c6c6c6 with #ffffff as the background color (for really old browsers that don't understand linear gradients)
	
**tran > tab**
*	Use CSS3 transitions with cross-browser compatibility **tran > tab > property to animate > tab > animation duration (without the 's') > tab > timing function**
	*	*Example:* **tran > tab > color > tab > 0.3 > tab > ease-out** this would create a cross-browser CSS3 transition that transitions the color property over 0.3 seconds and uses the "ease-out" timing function
	

##Support & Questions

If you have any questions you can [email me at](mailto:ethankr@comcast,net?subject=Simple-CSS4-Texmate-Bundle-Support)

##Thanks & Credits

This textmate bundle was made possible in large part by [CSS3 Please.com](http://css3please.com)

[@font-face cross-browser font generator](http://www.fontsquirrel.com/fontface/generator)

[Decompress .dfont files on the Mac](http://peter.upfold.org.uk/projects/dfontsplitter)