[![Published on NPM](https://img.shields.io/npm/v/@polymer/iron-swipeable-container.svg)](https://www.npmjs.com/package/@polymer/iron-swipeable-container)
[![Build status](https://travis-ci.org/PolymerElements/iron-swipeable-container.svg?branch=master)](https://travis-ci.org/PolymerElements/iron-swipeable-container)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://webcomponents.org/element/@polymer/iron-swipeable-container)

## &lt;iron-swipeable-container&gt;
`<iron-swipeable-container>` is a container that allows any of its nested
children (native or custom elements) to be swiped away. By default it supports
a curved or horizontal transition, but the transition duration and properties
can be customized.

See: [Documentation](https://www.webcomponents.org/element/@polymer/iron-swipeable-container),
  [Demo](https://www.webcomponents.org/element/@polymer/iron-swipeable-container/demo/demo/index.html).

## Usage

### Installation
```
npm install --save @polymer/iron-swipeable-container
```

### In an html file
```html
<html>
  <head>
    <script type="module">
      import '@polymer/iron-swipeable-container/iron-swipeable-container.js';
    </script>
  </head>
  <body>
    <iron-swipeable-container>
      <div>I can be swiped</div>
      <paper-card heading="Me too!"></paper-card>
    </iron-swipeable-container>
  </body>
</html>
```

### In a Polymer 3 element
```js
import {PolymerElement, html} from '@polymer/polymer';
import '@polymer/iron-swipeable-container/iron-swipeable-container.js';

class SampleElement extends PolymerElement {
  static get template() {
    return html`
    <iron-swipeable-container>
      <div>I can be swiped</div>
      <paper-card heading="Me too!"></paper-card>
    </iron-swipeable-container>
    `;
  }
}
customElements.define('sample-element', SampleElement);
```

## Contributing
If you want to send a PR to this element, here are
the instructions for running the tests and demo locally:

### Installation
```sh
git clone https://github.com/PolymerElements/iron-swipeable-container
cd iron-swipeable-container
npm install
npm install -g polymer-cli
```

### Running the demo locally
```sh
polymer serve --npm
open http://127.0.0.1:<port>/demo/
```

### Running the tests
```sh
polymer test --npm
```
