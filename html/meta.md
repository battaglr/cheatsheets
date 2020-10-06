# `meta`

## Declare character encoding

```html
<meta charset="utf-8" />
```

> [`charset` on W3C](https://www.w3.org/TR/html5/document-metadata.html#charset)


## Author, description and keywords

```html
<!-- Specify the author of the document -->
<meta name="author" content="Luciano Battagliero" />

<!-- Describe the content of the document -->
<meta name="description" content="This is a cheat sheet for meta tags" />

<!-- Specify relevant keywords -->
<meta name="keywords" content="cheat sheet, meta, html" />
```

> [`author`, `description`, `keywords` on W3C](https://www.w3.org/TR/html5/document-metadata.html#standard-metadata-names)


## Refresh or redirect

```html
<!-- Refresh current document after 5 seconds -->
<meta http-equiv="refresh" content="5" />

<!-- Immediate redirect to specified URL -->
<meta http-equiv="refresh" content="0; url=https://domain.com/" />
```

> [`refresh` on W3C](https://www.w3.org/TR/html5/document-metadata.html#attr-meta-http-equiv-refresh)


## Robots

```html
<!-- Instruct robots not to index the document -->
<meta name="robots" content="noindex" />

<!-- Instruct robots not to follow the links on the document -->
<meta name="robots" content="nofollow" />

<!-- Instruct robots not to index the document or follow its links -->
<meta name="robots" content="noindex, nofollow" />
```

> [`robots` on The Web Robot Pages](http://www.robotstxt.org/meta.html)
