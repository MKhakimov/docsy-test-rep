## Sections API

### Basic usage

    import { Section } from '@lib';

    const selectors = {
      buttons: '[data-button]',
      select: '[data-select]'
    };

    const elements = ['*buttons', 'select'];

    Section('section-name', {
      onLoad() {
        *onLoad logic here*
        *this._privateFuction(value)*
      },
      _privateFuction(value) {
        //privateFuction logic here
      }
    }, { elements, selectors });

### Available methods:
    - .hide() Hide an element
    - .show() Displays hidden element
    - .on(event, function) same as element.addEventListener
    - .HTML(htmlString) set HTML content for element
    - .text(textString)
    - .attr(attributeName, attributeValue) Get element's attribute, if second arguemnt set, it will change it's value
    - .css({Object}) Custom styles
### Properties:
    - .exists {Boolean} check if element exists
    - .isHidden {Boolean} check if element is hidden
