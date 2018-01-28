[![Build Status](https://travis-ci.org/admwx7/am-breakpoints.svg?branch=master)](https://travis-ci.org/admwx7/am-breakpoints)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg?style=flat-square)](https://www.webcomponents.org/element/admwx7/am-breakpoints)
[![GitHub license](https://img.shields.io/badge/license-Apache2.0-blue.svg)](https://raw.githubusercontent.com/admwx7/am-breakpoints/master/LICENSE)

# &lt;am-breakpoints&gt;

  Material Design: [Responsive UI](https://material.io/guidelines/layout/responsive-ui.html#responsive-ui-breakpoints)

  `<am-breakpoints>` is a hidden element for providing status updates on breakpoint changes, relies on a master-slave
  setup to prevent multiple instances of this element from creating additional media queries.

## Browsers Support

| [<img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/edge.png" alt="IE / Edge" width="16px" height="16px" />](http://godban.github.io/browsers-support-badges/)</br>IE / Edge | [<img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/firefox.png" alt="Firefox" width="16px" height="16px" />](http://godban.github.io/browsers-support-badges/)</br>Firefox | [<img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/chrome.png" alt="Chrome" width="16px" height="16px" />](http://godban.github.io/browsers-support-badges/)</br>Chrome | [<img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/safari.png" alt="Safari" width="16px" height="16px" />](http://godban.github.io/browsers-support-badges/)</br>Safari | [<img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/opera.png" alt="Opera" width="16px" height="16px" />](http://godban.github.io/browsers-support-badges/)</br>Opera | [<img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/safari-ios.png" alt="iOS Safari" width="16px" height="16px" />](http://godban.github.io/browsers-support-badges/)</br>iOS Safari | [<img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/chrome-android.png" alt="Chrome for Android" width="16px" height="16px" />](http://godban.github.io/browsers-support-badges/)</br>Chrome for Android |
| --------- | --------- | --------- | --------- | --------- | --------- | --------- |
| Edge| last 3 versions| last 3 versions| last 3 versions| last 3 versions| last 3 versions| last version

## Installation

  Build Tools: `npm i -g polymer-cli`

  Dependencies: `polymer install --variants`

  Linting: `npm i && npm run lint`

  Testing: `npm run test`

## Usage

  <!---
  ```
  <custom-element-demo>
    <template>
      <script src="../webcomponentsjs/webcomponents-lite.js"></script>
      <link rel="import" href="am-breakpoints.html">
      <style>
        [large], [small] {
          display: block;
        }
        h1 {
          display: none;
        }
      </style>
      <dom-bind>
        <template>
          <next-code-block></next-code-block>
        </template>
      </dom-bind>
    </template>
  </custom-element-demo>
  ```
  -->
  ```html
  <am-breakpoints
    active="{{smallLayout}}"
    breakpoints="xsmall,small"
  ></am-breakpoints>
  <am-breakpoints
    active="{{largeLayout}}"
    breakpoints="medium,large,xlarge"
  ></am-breakpoints>
  <h1 large$="[[largeLayout]]">Large Title</h1>
  <h1 small$="[[smallLayout]]">Small Title</h1>
  ```

## Contributing

  1. Fork it!
  2. Create your feature branch: `git checkout -b my-new-feature`
  3. Commit your changes: `git commit -am 'Add some feature'`
  4. Push to the branch: `git push origin my-new-feature`
  5. Submit a pull request :D
