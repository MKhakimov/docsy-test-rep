>Snippets are files containing chunks of reusable code. They reside in the snippets folder. They have the . ... They are most often used for code that appears on more than one page but not across the entire theme.

## article-pagination
>

### Accepts:
Name | Type | Default | Description
------------ | ------------- | ------------- | -------------
pagination | {String} | | pagination type


## blog-layout
>

### Accepts:
Name | Type | Default | Description
------------ | ------------- | ------------- | -------------
content | {String/HTML} | |


## card
>

### Accepts:
Name | Type | Default | Description
------------ | ------------- | ------------- | -------------
animate | {Boolean} | |
padded | {Boolean} | |
class | {String} | |
media_curved | {Boolean} | |
shadow | {Boolean} | |
link | {String} | |
media | {String} | |
body | {String} | |

## collection-sidebar-filter
> Renders a list of filters by tags

### Accepts:
Name | Type | Default | Description
------------ | ------------- | ------------- | -------------
filter_by | {String} | |
title | {String} | |


## float-caption
>

### Accepts:
Name | Type | Default | Description
------------ | ------------- | ------------- | -------------
content | {String} | | content for caption
Y | {String} | | Y coordinate of caption (top/center/bottom)
X | {String} | | X coordinate of caption (left/center/right)
class | {String} | |
container | {Boolean/String} | |
parent_layout | {String} | | (full/container) !do not use container prop is parent_layout is set
width | {Number} | | Width of caption %
width_unit | {String} | | Unit of a width
align_text | {Boolean} | | if true, text alignment will follow X direction


## gallery-card
> Renders gallery card

### Accepts:
Name | Type | Default | Description
------------ | ------------- | ------------- | -------------
image | {Object} | |
height | {Number} | |
link | {String} | |
title | {String} | |
text | {String} | |


## get-col
> Calculate Bootstraps css system grid for columns render

### Accepts:
Name | Type | Default | Description
------------ | ------------- | ------------- | -------------
value | {Number} | |
with_class | {Boolean} | true |

### Usage:
    {% capture col %}{% render 'get-columns', columns: 3 %}{% endcapture %}


## hero-media-text
>

### Accepts:
Name | Type | Default | Description
------------ | ------------- | ------------- | -------------
title | {String} | |
text_body | {String} | |
button | {String} | |
text_color | {String} | |
text_Y | {String} | |
text_X | {String} | |
text_with | {String} | |
text_align_to_X | {Boolean} | |
parent_layout | {String} | |
bg_size | {String} | |
bg_class | {String} | |
bg_link | {String} | |
bg_image | {Object} | |
bg_image_resolution | {String} | |
bg_cover | {Boolean} | true |
bg_video | {Object} | |
bg_video_scale | {Number} | |
bg_video_selector | {String} | | (data-selector)
bg_overlay | {Number} | |
bg_overlay_gradient | {Boolean} | |
bg_overlay_blur | {Boolean} | |
bg_overlay_blur_value | {Number} | |
bg_placeholder | {String} | |
bg_placeholder_index | {Number} | |


## modal
> Bootstrap v5 modal

### Accepts:
Name | Type | Default | Description
------------ | ------------- | ------------- | -------------
id | {String} | | id assignable to modal
content | {String} | | content for modal body
size | {String} | |
centered | {String} | |

### Usage:
    {% render 'price', product: product %}


## price
> Renders a list of product's price (regular, sale)

### Accepts:
Name | Type | Default | Description
------------ | ------------- | ------------- | -------------
product | {Object} | | Product Liquid object (optional)
variant | {Boolean} | | Renders selected or first variant price instead of overall product pricing (optional)
show_titles | {Boolean} |
show_compare_price | {Boolean} |
show_save_price | {Boolean} |
class | {String} | |
highlight_price | {Boolean} | true

###  Usage:
    {% render 'price', product: product %}


## media
> Renders media content like image or video

### Accepts:
Name | Type | Default | Description
------------ | ------------- | ------------- | -------------
class | {String} | | Additional container class
wrapper_class | {String} | | Additional wrapper class
aspect_ratio | {String} | |
width | {Number} | |
width_u | {String} | 'px' |
height | {Number} | |
height_u | {String} | 'px' |
content_height | {Boolean} | |
overlay | {Number} | |
overlay_gradient | {Boolean} | |
overlay_blur | {Boolean} | |
overlay_blur_value | {Number} | |
background_color | {String/hex} | optional | background color
image_class | {String} | | Additional image class
image | {Object} |
image_position | {String} | 'center' |
image_cover | {Boolean} | |
image_resolution | {String} | |
icon | {String} | |
icon_size | {String} | |
icon_color | {String/hex} | |
icon_class | {String} | |
video | {Object} | |
video_class | {String} | Additional video class
video_scale | {Number} | default: 100
video_selector | {String} | default 'data-video-container'
link | {String/link} | |
content_direction | {String} | |
content | {String/HTML} | |
placeholder | {String} | |
placeholder_index | {Number} | |
