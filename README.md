# Inna Iljina's Portfolio website

Hi there! 

Welcome to the guts of [https://iiljina.github.io](https://iiljina.github.io). 
I doubt that you're looking for this specific place. 🙃

If you do happen to want to explore this place, then I assume you know it better than me anyway. 👍

## How-To's

### Add a project
To add a project, simply create a file in a folder `_projects` 
```
---
title: My cool project
gist: Amsterdam, June 2021
folder: /static/projects/my-cool-project
---
Your content
```

- `title` is obviously the title of your project.
- `gist` is a very super duper short description of your project.
- `folder` is the location of all your files for a project

### Add some content
```markdown
# Title 1
## Title 2
### Title 3
#### Title 4
##### Title 5
###### Title 6

This is a paragraph because if has an empty line before and after.

This is a list of buller points
- One
- Two
- Three


{% include image.html 
    image="my_image.jpg" 
    size="one-third"
    position="left"
    title="My image title"
%}
About this paragraph is a single image will be added before leaving the text on the side.

This single image though will be added after the paragraph. It will be also on the right side.
{% include image.html 
    image="my_image.jpg" 
    size="two-thirds"
    position="right"
    title="My image title"
%}

This three dashes will create a horizontal line separating your content. 
---

This will become a row of images that you can open in a gallery.
{% include image_row.html
    gallery="tables-images"
     
    image1="my_image.jpg" size1="one-quarter" title1="Title 1"
    image2="my_image.jpg" size2="one-quarter" title2="Title 2"
    image3="my_image.jpg" size3="one-quarter" title3="Title 3"
    image4="my_image.jpg" size4="one-quarter" title4="Title 4"
%}

This row of images will be shown seperately and could be even divided by a lot of text, 
but because of the same `gallery="tables-images"` value it will be in the same gallery as the last one.
Change it to create another virtual gallery.
{% include image_row.html
    gallery="tables-images"
     
    image1="my_image.jpg" size1="one-quarter" title1="Title 1"
    image2="my_image.jpg" size2="one-quarter" title2="Title 2"
    image3="my_image.jpg" size3="one-quarter" title3="Title 3"
    image4="my_image.jpg" size4="one-quarter" title4="Title 4"
%}
```

#### Decide your size
Sometimes you see sizes. Basic sizes are `one-quarter`, `one-third`, `two-quarters`, `half`, `two-thirds`, `three-quarters` and `full`.

Also, for more advanced usage and fine-grained, a hint: a page virtually splits into 12 equal parts. 
`1/12` is named `col-1`, `2/12 = 1/6` is called `col-2`, `col-3` is thus `3/12`, etc, etc. 
All the way to `col-12` which is an equivalent of `full`.

#### Decide you position
It can be `left` or `right` at this moment, and only for a single image.

## Credits

Thanks to AJ <aj@lkn.io | @ajlkn> for a template _Read Only_ by [HTML5 UP](https://html5up.net) provided under [CCA 3.0 license](https://html5up.net/license).
