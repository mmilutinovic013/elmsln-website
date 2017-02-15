[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/arsnebula/nebula-button-behavior)

[![Build Status](https://saucelabs.com/browser-matrix/arsnebula.svg)](https://saucelabs.com/beta/builds/090abd80cd664808840fb292517260e5)

# \<nebula-button-behavior\>

A [Polymer](https://www.polymer-project.org) behavior to support button capabilities.

* Supports standard and toggle button modes
* Processes keyboard and gesture events to update button state automatically
* Supports [WAI-ARIA](https://www.w3.org/TR/wai-aria-practices-1.1/#button) authoring practices for **a11y**
* Provides attributes for styling buttons based on state changes

## Installation

```
$ bower install -S arsnebula/nebula-button-behavior
```

## Usage

Import the package behavior.

```html
<link rel="import" href="/bower_components/nebula-button-behavior/nebula-button-behavior.html"> 
```

Add the behavior to a custom element.

```js
Polymer({
  is: 'my-button',
  behaviors: [
    Nebula.ButtonBehavior
  ]
})
```

Style the element based on `pressed` and `pushed` attributes.

```css
:host([pressed]),
:host([pushed]) {
  background-color: teal;
  color: white;
}
```

*For more information on element properties and methods see the element API documentation.*

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Change Log

See [CHANGELOG](/CHANGELOG.md)

## License

See [LICENSE](/LICENSE.md)