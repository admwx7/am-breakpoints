[![Build Status](https://travis-ci.org/admwx7/am-breakpoints.svg?branch=master)](https://travis-ci.org/admwx7/am-breakpoints)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/admwx7/am-breakpoints)

# &lt;am-breakpoints&gt;

  Material Design: [Responsive UI](https://material.io/guidelines/layout/responsive-ui.html#responsive-ui-breakpoints)

  `<am-breakpoints>` is a hidden element for providing status updates on breakpoint changes, relies on a master-slave
  setup to prevent multiple instances of this element from creating additional media queries.

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
      <script src="../webcomponentsjs/webcomponents-light.js"></script>
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
