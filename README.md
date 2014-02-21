# Markel

Automatically parse markdown elements

## Usage

Include markel.js in your html page and write markdown inside <code>&lt;div data-parse="markdown"&gt;</code> elements. The markdown gets automatically converted to html as the page is loading.

So this:


    <div data-parse="markdown">
      # Heading 1
    </div>

Becomes this:

    <div data-parse="markdown">
      <h1 id="heading-1">Heading 1</h1>
    </div>

## About

Markel uses [marked](https://github.com/chjj/marked) for parsing markdown, because it's build for speed and we don't want to slow down page loading any more than necessary. Marked is included in markel.js. The actual markel code is only a few lines, so changing the parser is easy peasy if you desire.

## TODO

- Requirejs module and all that modern jazz?
- Dependencies, building with grunt and all that too?
- Browser compatibility? Latest chrome, safari & firefox work fine as usual. Need to test some mobile browsers and IE.
- Custom html5 element with polymer?
