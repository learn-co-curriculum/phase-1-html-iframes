# HTML Iframes

## Problem Statement

Some sites let us use _their_ creations in _our_ HTML documents. We're sure
you've noticed how many pages have Google maps built into them. The HTML tag
that lets us put someone else's web page _inside_ our page is the `iframe` tag.
We'll explore it in this lesson.


## Objectives

1. Describe how `iframe` elements work
2. State the `iframe` attributes

## Describe How `iframe` Elements Work

We can display HTML from other pages by using an `iframe` tag. The `iframe`
creates a window inside the page where this "shared" information appears.

An `iframe`'s `src` attribute points to the location of the shared material.
Examples are a custom search bar or YouTube video.

Here's an example:

```html
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d335994.89219194185!2d2.0673752159642937!3d48.8589713267984!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e66e1f06e2b70f%3A0x40b82c3688c9460!2sParis%2C+France!5e0!3m2!1sen!2sus!4v1457911182825" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
```

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d335994.89219194185!2d2.0673752159642937!3d48.8589713267984!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e66e1f06e2b70f%3A0x40b82c3688c9460!2sParis%2C+France!5e0!3m2!1sen!2sus!4v1457911182825" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>

## Some Important Iframe Attributes

### `src`

The `iframe` element has one required attribute: `src`. The `src` attribute takes a
URL (`http://example.com/....`) and displays the page requested.

### `width` and `height`

`width` and `height` allow us to control the size of the `iframe` that we'd
like to display. Depending on the website that you are using in your `iframe`,
it might have a size built in, but to be safe you always want to specify a
size. It's worth noting that if you know CSS, you can control height and width
there as well.

### `frameborder` and `style`

In earlier HTML versions, `iframe`s were put inside of borders by default.
Many people found that ugly. The `frameborder` allowed us to turn the border
off.  

The `frameborder` attribute is considered _deprecated_, meaning "likely to be
removed from the standard." In modern browsers, we can control borders _just_
using CSS, as with our example, `style="border:0"`.

Google and sites like YouTube still provide a `frameborder` attribute in their
embedded map examples. We see this appear often in `iframe` links as providers
try to support _as many browsers as possible_. It's important to understand what
it means, but you probably won't need to write it much.  If you do, you'll want
to set both `frameborder="0"` AND `style="border:0"`.

### `allowfullscreen`

Like the `required` attribute for HTML form elements, `allowfullscreen` is built
into HTML5. The `allowfullscreen` attribute uses a JavaScript method called
`requestFullScreen()` to send the `iframe` to full screen. If `allowfullscreen`
isn't included, the element can't be placed into full screen mode.. It's
important to be able to understand this attribute and realize that you can't get
around any restrictions unless the _provider_ wants you to. For more details
visit [MDN][mdn-allowfull].

[mdn-allow]: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe

## Conclusion

Iframes are powerful tools that allow us to show content from one website
within a different site. You can put any website you'd like in an `iframe`, but
certain sites make more sense than others. Search or mapping sites in `iframe`s
are the most frequently used. However, we've seen many inventive uses of
`iframe`s!

## Resources
- [HTML Forms and Iframes](https://www.youtube.com/embed/eiCtXc2YMKc?rel=0)
- [Presentation Slides](https://docs.google.com/presentation/d/115ECvsMyDnFBcc-Rvb4Jn876JhOycXxKVN6sv7OiJ1Y/edit?usp=sharing)
- [MDN - HTML - Iframe](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe)
- [Google Maps iframe documentation](https://developers.google.com/maps/documentation/embed/guide)
