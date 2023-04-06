# HTML

## Basic Structure

```
<!DOCTYPE html>
<html>
<head>
  <title>Page Title</title>
</head>
<body>
  Page content goes here
</body>
</html>
```

## Head Elements

* `<title>` - Sets the title of the webpage, shown on the browser's title bar or tab
* `<meta>` - Provides metadata about the HTML document
* `<link>` - Defines relationships between the current document and external resources (e.g., CSS files)
* `<style>` - Contains CSS styles for the HTML document
* `<script>` - Contains JavaScript code or links to external JavaScript files

## Text Formatting

* `<h1>` to `<h6>` - Headings (largest to smallest)
* `<p>` - Paragraph
* `<br>` - Line break
* `<strong>` - Bold text
* `<em>` - Italic text
* `<u>` - Underlined text
* `<s>` - Strikethrough text
* `<blockquote>` - Block quote
* `<code>` - Inline code
* `<pre>` - Preformatted text

## Lists

* `<ul>` - Unordered list
  * `<li>` - List item
* `<ol>` - Ordered list
  * `<li>` - List item

## Links and Images

* `<a href="URL">` - Link
* `<img src="URL" alt="Description">` - Image

## Tables

```
<table>
  <thead>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Row 1, Cell 1</td>
      <td>Row 1, Cell 2</td>
    </tr>
    <tr>
      <td>Row 2, Cell 1</td>
      <td>Row 2, Cell 2</td>
    </tr>
  </tbody>
</table>
```

## Forms

```
<form action="URL" method="GET/POST">
  <label for="input-id">Label:</label>
  <input type="text" id="input-id" name="input-name">
  <input type="submit" value="Submit">
</form>
```

## Other Common Elements

* `<div>` - Generic container for block-level elements
* `<span>` - Generic container for inline elements
* `<iframe src="URL">` - Inline frame for embedding other content
* `<button>` - Clickable button


# Meta Tags

## SEO

### General SEO Meta Tags

```
<meta name="title" content="Page Title">
<meta name="description" content="Page description up to 155 characters">
<meta name="keywords" content="keyword1, keyword2, keyword3">
```

### Robots

```
<meta name="robots" content="index, follow">
```

## Facebook (Open Graph)

```
<meta property="og:title" content="Page Title">
<meta property="og:description" content="Page description up to 155 characters">
<meta property="og:type" content="website">
<meta property="og:url" content="https://example.com">
<meta property="og:image" content="https://example.com/image.jpg">
<meta property="og:site_name" content="Website Name">
```

## Twitter

```
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Page Title">
<meta name="twitter:description" content="Page description up to 155 characters">
<meta name="twitter:image" content="https://example.com/image.jpg">
<meta name="twitter:site" content="@username">
<meta name="twitter:creator" content="@username">
```

## Schema.org (Structured Data)

### Organization

```
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "Organization Name",
  "url": "https://example.com",
  "logo": "https://example.com/logo.png",
  "sameAs": [
    "https://www.facebook.com/example",
    "https://twitter.com/example",
    "https://www.instagram.com/example"
  ]
}
</script>
```

### Breadcrumbs

```
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "BreadcrumbList",
  "itemListElement": [
    {
      "@type": "ListItem",
      "position": 1,
      "item": {
        "@id": "https://example.com",
        "name": "Home"
      }
    },
    {
      "@type": "ListItem",
      "position": 2,
      "item": {
        "@id": "https://example.com/page",
        "name": "Page"
      }
    }
  ]
}
</script>
```
