<p align="center"><img width="200" src="https://image.flaticon.com/icons/svg/332/332106.svg" alt="jsmarquee" /></p>

[![Build Status](https://travis-ci.org/rogervila/jsmarquee.svg?branch=master)](https://travis-ci.org/rogervila/jsmarquee)
[![StyleCI](https://github.styleci.io/repos/234736708/shield?branch=master)](https://github.styleci.io/repos/234736708)
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=rogervila_jsmarquee&metric=coverage)](https://sonarcloud.io/dashboard?id=rogervila_jsmarquee)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=rogervila_jsmarquee&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=rogervila_jsmarquee)

[![NPM](https://nodei.co/npm/jsmarquee.png?compact=true)](https://nodei.co/npm/jsmarquee/)

# jsmarquee

## About
**jsmarquee** is a pure javascript implementation of the old [HTML marquee tag](https://www.w3docs.com/learn-html/html-marquee-tag.html).

It is **not tied to any css or javascript library**, so it can be easily implemented on any frontend project.

## Usage

### Javascript setup

This is the default setup:

```js
import Marquee from 'jsmarquee'

const m = new Marquee({
  element: '#marquee-demo',
  velocity: 1
})

m.run()
```

These are the accepted properties:

| name  | value |
|----|---|
| **element**  | string with a query selector value |
| **velocity** | number. integer usage is recommended |

### HTML and CSS setup

As said before, **jsmarquee** is not tied to any CSS library.

In order to work correctly this is the basic CSS needed:

```html
<div class="my-marquee" id="marquee-demo">
    <div>
        content goes here. you can use any html tag, including images
    </div>
</div>
```

```css
.my-marquee {
  overflow: hidden;
}

.my-marquee > div {
  display: inline-flex;
  position: relative;
}
```

## Demos

- [CSS only](https://codepen.io/rogervila-1472551995/pen/JjoePwm)
- [Tailwind](https://codepen.io/rogervila-1472551995/pen/yLyQLQR)

## License

**jsmarquee** is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

Icons made by <a href="https://www.flaticon.com/authors/alfredo-hernandez" title="Alfredo Hernandez">Alfredo Hernandez</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
