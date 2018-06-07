# HTML Iframes

## Problem Statement

Now that we have a robust contact form built for our dog walking business, we can focus on the next aspect of letting people contact us: helping them find our location with Google Maps. In this lesson, we'll learn a bit about Iframe elements and how they let us interface with information from other websites. 

## Objectives
1. Describe how iframe elements work

### Describe How Iframe Elements Work

At its simplest incarnation, iframe elements allow us to link to other HTML content from within a frame window on our pages. The `src` attribute points to the location of other HTML content elsewhere and displays it within the current page. This can be used for anything from displaying a Google search bar, to a Youtube video, to more complicated elements like a Google Map that displays our exact location. 

Iframe elements have one required attribute: `src`. The `src` attribute takes a link and displays the page requested. 


```html
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d335994.89219194185!2d2.0673752159642937!3d48.8589713267984!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e66e1f06e2b70f%3A0x40b82c3688c9460!2sParis%2C+France!5e0!3m2!1sen!2sus!4v1457911182825" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
```

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d335994.89219194185!2d2.0673752159642937!3d48.8589713267984!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e66e1f06e2b70f%3A0x40b82c3688c9460!2sParis%2C+France!5e0!3m2!1sen!2sus!4v1457911182825" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>


## Resources
- [HTML Forms and Iframes](https://www.youtube.com/embed/eiCtXc2YMKc?rel=0)
- [Presentation Slides](https://docs.google.com/presentation/d/115ECvsMyDnFBcc-Rvb4Jn876JhOycXxKVN6sv7OiJ1Y/edit?usp=sharing)
- [MDN - HTML - Iframe](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe)