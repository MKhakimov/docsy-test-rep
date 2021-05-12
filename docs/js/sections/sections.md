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
Name | Description
------------ | -------------
.hide() | Hide an element
.show() | Displays hidden element
.on(event, function) | Same as element.addEventListener
.HTML(htmlString) | Set HTML content for element
.text(textString) | Set inner text content for element
.attr(attributeName, attributeValue) | Get element's attribute, if second arguemnt set, it will change it's value
.css({Object}) | Custom styles
### Properties:
Name | Type | Description
------------ | ------------- | -------------
.exists | {Boolean} | check if element exists
.isHidden | {Boolean} | check if element is hidden
