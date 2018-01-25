# attachshadow

[![donate](https://img.shields.io/badge/$-donate-ff69b4.svg?maxAge=2592000&style=flat)](https://github.com/WebReflection/donate)
[![License: ISC](https://img.shields.io/badge/License-ISC-yellow.svg)](https://opensource.org/licenses/ISC)

An iframe based Shadow DOM poorlyfill


### Features

  * compatible down to **IE9** with a size of about 1.3K
  * provides an `element.attachShadow(mode)` method out of the box
  * both mode `open` and `closed` are available. `open` is set to the `shadowRoot` property as expected.
  * events are synthetically re-targeted to the owner, hence propagated to the parent document
  * encapsulation is preserved, including `:host` CSS declarations
  * each _iframe_ transparently resize accordingly to its content

### What this is not

  * this is not a Custom Elements or an HTMLTemplateElement polyfill. This is only the `attachShadow` method.
  * this is not, and never will be, a 100% reliable polyfill for Shadow DOM, for the simple reason that Shadow DOM cannot be polyfilled (this is _a poorlyfill_ indeed)
  * not yet a battle tested solution. If you have any experience with _iframe_ shenanigans please help making this poorlyfill less poor, thank you!

### CDN

You can use `https://unpkg.com/attachshadow` as CDN for this library.

### Test

Please visit the [test page](https://webreflection.github.io/attachshadow/test/) and click on the button to see in console the propagated event.