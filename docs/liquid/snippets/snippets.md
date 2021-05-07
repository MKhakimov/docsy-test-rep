>Snippets are files containing chunks of reusable code. They reside in the snippets folder. They have the . ... They are most often used for code that appears on more than one page but not across the entire theme.

## modal
### Props:
    -id: {String} id assignable to modal
    -content: {String} content for modal body
    -size: {String}
    -centered: {String}
### Usage:
    {% render 'price', product: product %}

## price
> Renders a list of product's price (regular, sale)

### Accepts:
    - product: {Object} Product Liquid object (optional)
    - variant: {Boolean} Renders selected or first variant price instead of overall product pricing (optional)
    - show_titles: {Boolean}
    - show_compare_price: {Boolean}
    - show_save_price: {Boolean}
    - class: {String}
    - highlight_price: {Boolean} default: true

###  Usage:
    {% render 'price', product: product %}
