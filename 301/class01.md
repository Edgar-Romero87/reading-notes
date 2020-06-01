# Responsive Web Design
With the growth in mobile Internet usage comes the question of how to build websites suitable for all users. The industry response to this question has become responsive web design, also known as RWD.

## Responsive Overview
Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop. Responsive web design is focused around providing an intuitive and gratifying experience for everyone. Desktop computer and cell phone users alike all benefit from responsive websites.

### Responsive vs. Adaptive vs. Mobile
Responsive and adaptive web design are closely related, and often transposed as one in the same. Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation, such as change. 
Mobile, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users. While this does occasionally have its place, it normally isn’t a great idea. Mobile websites can be extremely light but they do come with the dependencies of a new code base and browser sniffing, all of which can become an obstacle for both developers and users.
Currently the most popular technique lies within responsive web design, favoring design that dynamically adapts to different browser and device viewports, changing layout and content along the way. This solution has the benefits of being all three, responsive, adaptive, and mobile.

### Flexible Layouts

Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media. The first part, flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. Flexible grids are built using relative length units, most commonly percentages or **em** units. These relative lengths are then used to declare common grid property values such as **width, margin, or padding.**
Website layouts need to adapt to this change and fixed values have too many constraints. Fortunately, Ethan pointed out an easy formula to help identify the proportions of a flexible layout using relative values.
The formula is based around taking the target width of an element and dividing it by the width of it’s parent element. The result is the relative width of the target element.

target ÷ context = result

Using the flexible grid formula we can take all of the fixed units of length and turn them into relative units. In this example we’ll use percentages but **em** units would work equally as well. Notice, no matter how wide the parent **container** becomes, the **section** and **aside** margins and widths scale proportionally.

### Media Queries

Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example. Being able to apply uniquely targeted styles opens up a world of opportunity and leverage to responsive web design.

#### Initializing Media Queries

There are a couple different ways to use media queries, using the @media rule inside of an existing style sheet, importing a new style sheet using the @import rule, or by linking to a separate style sheet from within the HTML document. Generally speaking it is recommend to use the @media rule inside of an existing style sheet to avoid any additional HTTP requests.
Each media query may include a media type followed by one or more expressions. Common media types include all, screen, print, tv, and braille. The HTML5 specification includes new media types, even including 3d-glasses. Should a media type not be specified the media query will default the media type to screen.

The media query expression that follows the media type may include different media features and values, which then allocate to be true or false. When a media feature and value allocate to true, the styles are applied. If the media feature and value allocate to false the styles are ignored.

#### Logical Operators in Media Queries

Logical operators in media queries help build powerful expressions. There are three different logical operators available for use within media queries, including and, not, and only.

Using the and logical operator within a media query allows an extra condition to be added, making sure that a browser or devices does both a, b, c, and so forth. Multiple individual media queries can be comma separated, acting as an unspoken or operator. The example below selects all media types between 800 and 1024 pixels wide.
#### Omitting a Media Type
When using the not and only logical operators the media type may be left off. In this case the media type is defaulted to all.

#### Media Features in Media Queries

Knowing the media query syntax and how logical operators work is a great introduction to media queries but the true work comes with media features. Media features identify what attributes or properties will be targeted within the media query expression.

#### Height & Width Media Features

One of the most common media features revolves around determining a height or width for a device or browser viewport. The height and width may be found by using the height and width media features. Each of these media features may then also be prefixed with the min or max qualifiers, building a feature such as min-width or max-width.

The height and width features are based off the height and width of the viewport rendering area, the browser window for example. Values for these height and width media features may be any length unit, relative or absolute.
@media all and (min-width: 320px) and (max-width: 780px) {...}

#### Using Minimum & Maximum Prefixes

The min and max prefixes can be used on quite a few media features. The min prefix indicates a values of greater than or equal to while the max prefix indicates a value of less than or equal to. Using min and max prefixes avoid any conflict with the general HTML syntax, specifically not using the < and > symbols.
#### Orientation Media Feature

The orientation media feature determines if a device is in the landscape or portrait orientation. The landscape mode is triggered when the display is wider than taller, and the portrait mode is triggered when the display is taller than wider. This media feature plays a large part with mobile devices.
@media all and (orientation: landscape) {...}

#### Aspect Ratio Media Features

The aspect-ratio and device-aspect-ratio features specifies the width/height pixel ratio of the targeted rendering area or output device. The min and max prefixes are available to use with the different aspect ratio features, identifying a ratio above or below that of which is stated.

The value for the aspect ratio feature consist of two positive integers separated by a forward slash. The first integer identifies the width in pixels while the second integer identifies the height in pixels.
@media all and (min-device-aspect-ratio: 16/9) {...}

#### Pixel Ratio Media Features

In addition to the aspect ratio media features there are also pixel-ratio media features. These features do include the device-pixel-ratio feature as well as min and max prefixes. Specifically, the pixel ratio feature is great for identifying high definition devices, including retina displays. Media queries for doing so look like the following.

@media only screen and (-webkit-min-device-pixel-ratio: 1.3), only screen and (min-device-pixel-ratio: 1.3) {...}
#### Resolution Media Feature

The resolution media feature specifies the resolution of the output device in pixel density, also known as dots per inch or DPI. The resolution media feature does accept the min and max prefixes. Additionally, the resolution media feature will accept dots per pixel (1.3dppx), dots per centimeter (118dpcm), and other length based resolution values.
@media print and (min-resolution: 300dpi) {...}

#### Other Media Features

Other media features include identifying available output colors with use of the color, color-index, and monochrome features, identifying bitmap devices with the grid feature, and identifying the scanning process of a television with the scan feature. These features are less common but equally as helpful when needed.
#### Media Queries Demo

Using media queries we will now rewrite the flexible layout we built previously. One of the current problems within the demo appears when the aside width becomes uselessly small within smaller viewports. Adding a media query for viewports under 420 pixels wide we can change the layout by turning off the floats and changing the widths of the section and aside.
#### Identifying Breakpoints

Your instinct might be to write media query breakpoints around common viewport sizes as determined by different device resolutions, such as 320px, 480px, 768px, 1024px, 1224px, and so forth. This is a bad idea.

When building a responsive website it should adjust to an array of different viewport sizes, regardless of the device. Breakpoints should only be introduced when a website starts to break, look weird, or the experience is being hampered.

Additionally, new devices and resolutions are being released all of the time. Trying to keep up with these changes could be an endless process.

### Mobile First

One popular technique with using media queries is called mobile first. The mobile first approach includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.

The operating belief behind mobile first design is that a user on a mobile device, commonly using a smaller viewport, shouldn’t have to load the styles for a desktop computer only to have them over written with mobile styles later. Doing so is a waste of bandwidth. Bandwidth that is precious to any users looking for a snappy website.

The mobile first approach also advocates designing with the constraints of a mobile user in mind. Before too long, the majority of Internet consumption will be done on a mobile device. Plan for them accordingly and develop intrinsic mobile experiences.

A breakout of mobile first media queries might look at bit like the following.

/* Default styles first then media queries */

@media screen and (min-width: 400px)  {...}

@media screen and (min-width: 600px)  {...}

@media screen and (min-width: 1000px) {...}

@media screen and (min-width: 1400px) {...}

### Viewport

Mobile devices generally do a pretty decent job of displaying websites these days. Sometimes they could use a little assistance though, particularly around identifying the viewport size, scale, and resolution of a website. To remedy this, Apple invented the viewport meta tag.
#### Viewport Height & Width

Using the viewport meta tag with either the height or width values will define the height or width of the viewport respectively. Each value accepts either a positive integer or keyword. For the height property the keyword device-height value is accepted, and for the width property the keyword device-width is accepted. Using these keywords will inherit the device’s default height and width value.

For the best results, and the best looking website, it is recommend that you use the device defaults by applying the device-height and device-width values.
#### Viewport Scale

To control how a website is scaled on a mobile device, and how users can continue to scale a website, use the minimum-scale, maximum-scale, initial-scale, and user-scalable properties.

The initial-scale of a website should be set to 1 as this defines the ratio between the device height, while in a portrait orientation, and the viewport size. Should a device be in landscape mode this would be the ratio between the device width and the viewport size. Values for initial-scale should always be a positive integer between 0 and 10.
The minimum-scale and maximum-scale values determine how small and how large a viewport may be scaled. When using minimum-scale the value should be a positive integer lower than or equal to the initial-scale. Using the same reasoning, the maximum-scale value should be a positive integer greater than or equal to the initial-scale. Values for both of these must also be between 0 and 10.
#### CSS Viewport Rule

Since the viewport meta tag revolves so heavily around setting the styles of how a website should be rendered it has been recommend to move the viewport from a meta tag with HTML to an @ rule within CSS. This helps keep the style separated from content, providing a more semantic approach.

Currently some browsers have already implemented the @viewport rule, however support isn’t great across the board. The previously recommended viewport meta tag would look like the following @viewport rule in CSS.

### Flexible Media

The final, equally important aspect to responsive web design involves flexible media. As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.

One quick way to make media scalable is by using the max-width property with a value of 100%. Doing so ensures that as the viewport gets smaller any media will scale down according to its containers width.
#### Flexible Embedded Media

Unfortunately the max-width property doesn’t work well for all instances of media, specifically around iframes and embedded media. When it comes to third party websites, such as YouTube, who use iframes for embedded media this is a huge disappointment. Fortunately, there is a work around.

To get embedded media to be fully responsive, the embedded element needs to be absolutely positioned within a parent element. The parent element needs to have a width of 100% so that it may scale based on the width of the viewport. The parent element also needs to have a height of 0 to trigger the hasLayout mechanism within Internet Explorer.

Padding is then given to the bottom of the parent element, the value of which is set in the same aspect ratio of the video. This allows the height of the parent element to be proportionate to that of it’s width. Remember the responsive design formula from before? If a video has an aspect ratio of 16:9, 9 divided by 16 equals .5625, thus requiring a bottom padding of 56.25%. Padding on the bottom and not the top is specifically used to prevent Internet Explorer 5.5 from breaking, and treating the parent element as an absolutely positioned element.

# All About Floats
## What is “Float”?

Float is a CSS positioning property. To understand its purpose and origin, we can look to print design. In a print layout, images may be set into the page such that text wraps around them as needed. This is commonly and appropriately called “text wrap”. Here is an example of that.
In page layout programs, the boxes that hold the text can be told to honor the text wrap, or to ignore it. Ignoring the text wrap will allow the words to flow right over the image like it wasn’t even there. This is the difference between that image being part of the flow of the page (or not). Web design is very similar. In web design, page elements with the CSS float property applied to them are just like the images in the print layout where the text flows around them. Floated elements remain a part of the flow of the web page. This is distinctly different than page elements that use absolute positioning. Absolutely positioned page elements are removed from the flow of the webpage, like when the text box in the print layout was told to ignore the page wrap. Absolutely positioned page elements will not affect the position of other elements and other elements will not affect them, whether they touch each other or not.
There are four valid values for the float property. **Left** and **Right** float elements those directions respectively. **None** (the default) ensures the element will not float and **Inherit** which will assume the float value from that elements parent element.

### What are floats used for?

Aside from the simple example of wrapping text around images, floats can be used to create entire web layouts.

### Clearing the Float

Float’s sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float. Again an illustration probably does more good than words do.
Clear has four valid values as well. **Both** is most commonly used, which clears floats coming from either direction. **Left** and **Right** can be used to only clear the float from one direction respectively. **None** is the default, which is typically unnecessary unless removing a clear value from a cascade. **Inherit** would be the fifth, but is strangely not supported in Internet Explorer.

### The Great Collapse

One of the more bewildering things about working with floats is how they can affect the element that contains them (their “parent” element). If this parent element contained nothing but floated elements, the height of it would literally collapse to nothing. This isn’t always obvious if the parent doesn’t contain any visually noticeable background, but it is important to be aware of.

### Techniques for Clearing Floats

If you are in a situation where you always know what the succeeding element is going to be, you can apply the clear: both; value to that element and go about your business. This is ideal as it requires no fancy hacks and no additional elements making it perfectly semantic. Of course things don’t typically work out that way and we need to have more float-clearing tools in our toolbox.

### Problems with Floats

Floats often get beat on for being fragile. The majority of this fragility comes from IE 6 and the slew of float-related bugs it has. As more and more designers are dropping support for IE 6, you may not care, but for the folks that do care here is a quick rundown.

### Alternatives

If you need text wrapping around images, there really aren’t any alternatives for float. Speaking of which, check out this rather clever technique for wrapping text around irregular shapes. But for page layout, there definitely are choices. Eric Sol right here on A List Apart has an article on Faux Absolute Positioning, which is a very interesting technique that in many ways combines the flexibility of floats with the strength of absolute positioning. CSS3 has the Template Layout Module that, when widely adopted, will prove to be the page layout technique of choice.