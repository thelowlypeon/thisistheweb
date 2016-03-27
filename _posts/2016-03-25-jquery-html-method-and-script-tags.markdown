---
layout: post
title:  "jQuery HTML Method and Script Tags"
date:   2016-03-25 10:30:00 -0500
categories: jekyll
tags: jquery, html, script
author: andy
---

jQuery's `.html()` method is not just a wrapper of `.innerHTML`.

Using it as a getter, as in `element.html()`, will return the element's HTML contents but strip out any script tags that the content may contain. If you need to return script content as well, you'll need to use `element.innerHTML`.

Using it as a setter, as in `element.html(newContent)`, will set the element's content _and_ execute any script tags contained in `newContent`. Conversely, `element.innerHTML = newContent` will set the element's content but will _not_ execute any script tags contained in `newContent`.

Documentation for `.html()` can be found [here](https://api.jquery.com/html/).

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
