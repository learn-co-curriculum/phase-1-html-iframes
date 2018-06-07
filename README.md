# HTML Iframes

## Problem Statement

Now that we have a robust contact form built for our dog walking business, we
can focus on the next aspect of letting people contact us: helping them find our
location with Google Maps. In this lesson, we'll learn a bit about Iframe
elements and how they let us interface with information from other websites. 

## Objectives
1. Describe how iframe elements work
2. Benefits of iframe attributes

## Describe How Iframe Elements Work

At its simplest incarnation, iframe elements allow us to link to other HTML
content from within a frame window on our pages. The `src` attribute points to
the location of other HTML content elsewhere and displays it within the current
page. This can be used for anything from displaying a Google search bar, to a
Youtube video, to more complicated elements like a Google Map that displays our
exact location. 


```html
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d335994.89219194185!2d2.0673752159642937!3d48.8589713267984!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e66e1f06e2b70f%3A0x40b82c3688c9460!2sParis%2C+France!5e0!3m2!1sen!2sus!4v1457911182825" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
```

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d335994.89219194185!2d2.0673752159642937!3d48.8589713267984!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e66e1f06e2b70f%3A0x40b82c3688c9460!2sParis%2C+France!5e0!3m2!1sen!2sus!4v1457911182825" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>

## Some Important Iframe Attributes

### `src` 
Iframe elements have one required attribute: `src`. The `src` attribute takes a
link and displays the page requested. 

### `width` and `height` 
`width` and `height` allow us to control the size of the iframe that we'd like
to display. Depending on the website that you are using in your iframe, it might
have a size built in, but to be safe you always want to specify a size. This can
also be controlled with CSS (which you'll learn about a bit later), so a good
rule of thumb is to specify the biggest size that you'll want to show on your
website. 

### frameborder and style 
`frameborder` is a bit of a legacy from back when web browsers thought it was a
good idea to give elements built-in frames. Nowadays we like to control that
kind of thing with CSS, so most of the time you'll want to set both
`frameborder="0"` AND `style="border:0"`. Since different browsers handle the
attributes in multiple ways, specifying both will ensure that you won't have a
frame popping up unexpectedly. 

### allowfullscreen 
Like the `required` attribute for HTML form elements, `allowfullscreen` is built
into HTML5. Simply by including `allowfullscreen` in our attributes, browsers
understand that means that the iframe is allowed to be placed into fullscreen
mode. If you'd rather avoid that, just don't include `allowfullscreen` in your
attributes. 

## Conclusion 
Iframes are powerful tools that allow us to show content from one website within
a different site. You can iframe any website you'd like, but certain sites make
more sense to iframe than others. Iframing search sites and mapping sites is
most common, but use your imagination to be creative and play around with all
kinds of iframes!

## Resources 
- [HTML Forms and Iframes](https://www.youtube.com/embed/eiCtXc2YMKc?rel=0)
- [Presentation Slides](https://docs.google.com/presentation/d/115ECvsMyDnFBcc-Rvb4Jn876JhOycXxKVN6sv7OiJ1Y/edit?usp=sharing)
- [MDN - HTML - Iframe](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe)
- [Google Maps iframe documentation](https://developers.google.com/maps/documentation/embed/guide)