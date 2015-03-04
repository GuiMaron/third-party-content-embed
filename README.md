# Third Party Content Embed

Simple workaround to embed third party content inside articles, keeping everything neat and tidy! or in other words, ~~responsive~~ fluid.

It works as a proxy, creating a layer that will resize the content if needed to fit everything inside the available width. All modern browsers are supoorted and Internet Explorer 9+.

## How to build

With [Node.js](http://nodejs.org/) installed run the following commands from the cloned project folder:

```sh
npm install
npm run build
```

## How to use

Publish all the files within the `dist` project's folder, then add the following code wherever you want to embed something:

```
<iframe src="path/to/main.html?content=http%3A//example.com/&amp;width=800&amp;height=600"></iframe>
```

Make sure this `iframe` has properly styles to be fluid, otherwise the magic won't happen.

## Paramters

The `main.html` has the following query string paramters:

* `content` url that is intented to be embeded.
* `width` the original width of the content.
* `height` the original height of the content, make sure to also set the same height in the `iframe`.
