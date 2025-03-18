---
author: ["Tung Phung"]
title: "Setting up Fujitsu ix500 with Raspberry Pi 2 W"
date: "2025-03-14"
description: "Meow"
summary: "Meow2"
tags: ["fujitsu", "ix500", "iot", "raspberry", "pi"]
categories: ["themes", "syntax"]
series: ["Themes Guide"]
ShowToc: true
TocOpen: true
draft: true
---

### MOE

I'm not good with paperwork. I don't have a good file system, there's always
some sort of personal data on there that I can't just simply part with. So I
shred what I can. But what about the stuff I **need** to keep? And how will I find
it again or even know I still have it when the time comes? And how much time
will I spend continually organizing and searching for these important documents? 
Fortunately, I'm on step closer.

My sister recently passed on a Fujitsu ix500 scanner. Lucky me! I tested it and
it scans beautifully and also works well with its current Scansnap software. It
has an auto-feed and also built-in Wi-Fi! This thing has everything to scan well.
However, I wanted to keep the setup in our office cabinet minimal and thus, I 
wanted to tie it in with a Raspberry Pi 2 W I have running the CUPS server for
the Brother printer.

So two devices on one Raspberry Pi 2 W. Less Wi-Fi congestion, because I won't
use the Wi-Fi functionality of the ix500. But I still have all the portability
of the setup and the ability to archive everything and shred it (except for of
course important documents).

Firstly, the Raspberry Pi 2 W doesn't have too many USB ports, so I had to buy a
little USB Hub to split to two full-size USBs from a micro-USB, which the Pi 2 W
has. Once connected and checking that both devices could talk to the PI, I went
about the task of integrating the scanner. 

I found a post doing something similar to a debian system, but I did encounter
some difficulties that he didn't.





### Inline Code

`This is Inline Code`

### Only `pre`

<pre>
This is pre text
</pre>

### Code block with backticks

```{hl_lines=[2,8]}
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Example HTML5 Document</title>
    <meta
      name="description"
      content="Sample article showcasing basic Markdown syntax and formatting for HTML elements."
    />
  </head>
  <body>
    <p>Test</p>
  </body>
</html>
```

### Code block with backticks and language specified

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Example HTML5 Document</title>
    <meta
      name="description"
      content="Sample article showcasing basic Markdown syntax and formatting for HTML elements."
    />
  </head>
  <body>
    <p>Test</p>
  </body>
</html>
```

### Code block with backticks and language specified with line numbers

```html {linenos=true}
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Example HTML5 Document</title>
    <meta
      name="description"
      content="Sample article showcasing basic Markdown syntax and formatting for HTML elements."
    />
  </head>
  <body>
    <p>Test</p>
  </body>
</html>
```

### Code block with line numbers and <mark>highlighted</mark> lines

- PaperMod supports `linenos=true` or `linenos=table`

```html {linenos=true,hl_lines=[2,8]}
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Example HTML5 Document</title>
    <meta
      name="description"
      content="Sample article showcasing basic Markdown syntax and formatting for HTML elements."
    />
  </head>
  <body>
    <p>Test</p>
  </body>
</html>
```

- <del>With `linenos=inline` line <mark>**might not** get highlighted</mark> properly.<del>
- This issue is fixed with [045c084](https://github.com/adityatelange/hugo-PaperMod/commit/045c08496d61b1b3f9c79e69e7d3d243a526d8f3)

```html {linenos=inline,hl_lines=[2,8]}
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Example HTML5 Document</title>
    <meta
      name="description"
      content="Sample article showcasing basic Markdown syntax and formatting for HTML elements."
    />
  </head>
  <body>
    <p>Test</p>
  </body>
</html>
```

### Code block indented with four spaces

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

### Code block with Hugo's internal highlight shortcode

{{< highlight html >}}

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

### Github Gist

{{< gist adityatelange 376cd56ee2c94aaa2e8b93200f2ba8b5 >}}
