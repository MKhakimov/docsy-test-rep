> Snippets are files containing chunks of reusable code. They reside in the snippets folder. They have the . ... They are most often used for code that appears on more than one page but not across the entire theme.

# article-pagination

> Description

### Accepts:

Name       | Type     | Default | Description
---------- | -------- | ------- | ---------------
pagination | {String} |         | pagination type

# blog-layout

> Description

### Accepts:

Name    | Type          | Default | Description
------- | ------------- | ------- | -----------
content | {String/HTML} |         |

# card

> Description

### Accepts:

Name         | Type      | Default | Description
------------ | --------- | ------- | -----------
animate      | {Boolean} |         |
padded       | {Boolean} |         |
class        | {String}  |         |
media_curved | {Boolean} |         |
shadow       | {Boolean} |         |
link         | {String}  |         |
media        | {String}  |         |
body         | {String}  |         |

# collection-sidebar-filter

> Renders a list of filters by tags

### Accepts:

Name      | Type     | Default | Description
--------- | -------- | ------- | -----------
filter_by | {String} |         |
title     | {String} |         |

# float-caption

> Description

### Accepts:

Name          | Type             | Default | Description
------------- | ---------------- | ------- | -------------------------------------------------------------------
content       | {String}         |         | content for caption
Y             | {String}         |         | Y coordinate of caption (top/center/bottom)
X             | {String}         |         | X coordinate of caption (left/center/right)
class         | {String}         |         |
container     | {Boolean/String} |         |
parent_layout | {String}         |         | (full/container) !do not use container prop is parent_layout is set
width         | {Number}         |         | Width of caption %
width_unit    | {String}         |         | Unit of a width
align_text    | {Boolean}        |         | if true, text alignment will follow X direction

# gallery-card

> Renders gallery card

### Accepts:

Name   | Type     | Default | Description
------ | -------- | ------- | -----------
image  | {Object} |         |
height | {Number} |         |
link   | {String} |         |
title  | {String} |         |
text   | {String} |         |

# get-col

> Calculate Bootstraps css system grid for columns render

### Accepts:

Name       | Type      | Default | Description
---------- | --------- | ------- | -----------
value      | {Number}  |         |
with_class | {Boolean} | true    |

### Usage:

```
{% capture col %}{% render 'get-columns', columns: 3 %}{% endcapture %}
```

# media

> Renders media content like image or video

### Accepts:

Name               | Type          | Default                        | Description
------------------ | ------------- | ------------------------------ | --------------------------
class              | {String}      |                                | Additional container class
wrapper_class      | {String}      |                                | Additional wrapper class
aspect_ratio       | {String}      |                                |
width              | {Number}      |                                |
width_u            | {String}      | 'px'                           |
height             | {Number}      |                                |
height_u           | {String}      | 'px'                           |
content_height     | {Boolean}     |                                |
overlay            | {Number}      |                                |
overlay_gradient   | {Boolean}     |                                |
overlay_blur       | {Boolean}     |                                |
overlay_blur_value | {Number}      |                                |
background_color   | {String/hex}  | optional                       | background color
image_class        | {String}      |                                | Additional image class
image              | {Object}      |                                |
image_position     | {String}      | 'center'                       |
image_cover        | {Boolean}     |                                |
image_resolution   | {String}      |                                |
icon               | {String}      |                                |
icon_size          | {String}      |                                |
icon_color         | {String/hex}  |                                |
icon_class         | {String}      |                                |
video              | {Object}      |                                |
video_class        | {String}      | Additional video class         |
video_scale        | {Number}      | default: 100                   |
video_selector     | {String}      | default 'data-video-container' |
link               | {String/link} |                                |
content_direction  | {String}      |                                |
content            | {String/HTML} |                                |
placeholder        | {String}      |                                |
placeholder_index  | {Number}      |                                |

# hero-media-text

> Description

### Accepts:

Name                  | Type      | Default | Description
--------------------- | --------- | ------- | ---------------
title                 | {String}  |         |
text_body             | {String}  |         |
button                | {String}  |         |
text_color            | {String}  |         |
text_Y                | {String}  |         |
text_X                | {String}  |         |
text_with             | {String}  |         |
text_align_to_X       | {Boolean} |         |
parent_layout         | {String}  |         |
bg_size               | {String}  |         |
bg_class              | {String}  |         |
bg_link               | {String}  |         |
bg_image              | {Object}  |         |
bg_image_resolution   | {String}  |         |
bg_cover              | {Boolean} | true    |
bg_video              | {Object}  |         |
bg_video_scale        | {Number}  |         |
bg_video_selector     | {String}  |         | (data-selector)
bg_overlay            | {Number}  |         |
bg_overlay_gradient   | {Boolean} |         |
bg_overlay_blur       | {Boolean} |         |
bg_overlay_blur_value | {Number}  |         |
bg_placeholder        | {String}  |         |
bg_placeholder_index  | {Number}  |         |

# hsl-color

> Description

### Accepts:

Name   | Type     | Default | Description
------ | -------- | ------- | -----------
name   | {String} |         |
target | {String} |         |

# icon

> Description

### Accepts:

Name          | Type     | Default | Description
------------- | -------- | ------- | -----------
name          | {String} |         |
size          | {String} |         |
color         | {String} |         |
load          | {String} |         |
data_selector | {String} |         |

# media-hero-size

> Description

### Accepts:

Name               | Type          | Default | Description
------------------ | ------------- | ------- | -------------------
size               | {String}      |         |
class              | {String}      |         |
link               | {String}      |         |
content            | {String/HTML} |         |
content_direction  | {String}      |         | (left/right/center)
image              | {Object}      |         |
image_resolution   | {String}      |         |
cover              | {Boolean}     | true    |
video              | {Object}      |         |
video_scale        | {Number}      |         |
video_selector     | {String}      |         | (data-selector)
overlay            | {Number}      |         |
overlay_gradient   | {Boolean}     |         |
overlay_blur       | {Boolean}     |         |
overlay_blue_value | {Number}      |         |
placeholder        | {String}      |         |
placeholder_index  | {Number}      |         |

# media-overlay

> Description

### Accepts:

Name       | Type      | Default | Description
---------- | --------- | ------- | ---------------------
value      | {Number}  |         |
base_class | {String}  |         | inherited from parent
blur       | {Boolean} |         |
direction  | {String}  |         | left/center/right
gradient   | {Boolean} |         |
base       | {Boolean} | true    |

# media-placeholder

> Description

### Accepts:

Name       | Type     | Default | Description
---------- | -------- | ------- | ---------------------
base_class | {String} |         | inherited from parent
name       | {String} |         |
index      | {Number} |         |

# modal

> Bootstrap v5 modal

### Accepts:

Name     | Type     | Default | Description
-------- | -------- | ------- | ----------------------
id       | {String} |         | id assignable to modal
content  | {String} |         | content for modal body
size     | {String} |         |
centered | {String} |         |

### Usage:

```
{% render 'price', product: product %}
```

# nav

> Renders navigation element based on linklists[menu].links

### Accepts:

Name  | Type     | Default | Description
----- | -------- | ------- | -----------
menu  | {String} |         |
class | {String} |         |

# page-header

> Renders page header ¯-(ツ)_/¯

### Accepts:

Name         | Type      | Default | Description
------------ | --------- | ------- | -----------
title        | {String}  |         |
subtitle     | {String}  |         |
bg_image     | {Object}  |         |
use_bg_image | {Boolean} |         |
as_section   | {Boolean} |         |

# placeholder

> Renders placeholder ¯-(ツ)_/¯

### Accepts:

Name      | Type      | Default | Description
--------- | --------- | ------- | -----------
name      | {String}  |         |
index     | {Number}  |         |
class     | {String}  |         |
svg_class | {String}  |         |
fill      | {Boolean} |         |

# price

> Renders a list of product's price (regular, sale)

### Accepts:

Name               | Type      | Default | Description
------------------ | --------- | ------- | -------------------------------------------------------------------------------------
product            | {Object}  |         | Product Liquid object (optional)
variant            | {Boolean} |         | Renders selected or first variant price instead of overall product pricing (optional)
show_titles        | {Boolean} |
show_compare_price | {Boolean} |
show_save_price    | {Boolean} |
class              | {String}  |         |
highlight_price    | {Boolean} | true

### Usage:

```
{% render 'price', product: product %}
```

# product-reviews

> Renders a product-reviews block

### Accepts:

Name    | Type     | Default | Description
------- | -------- | ------- | -----------
product | {Object} |         |
class   | {String} |         |

# product-stock-alert

> Renders a stock information if inventory_quantity > remaining

### Accepts:

Name      | Type     | Default | Description
--------- | -------- | ------- | --------------------------------------------
remaining | {String} |         | amount of remainig items to display an alert
variant   | {Object} |         |

# product-tabs

> Renders a product-tabs

### Accepts:

Name      | Type            | Default    | Description
--------- | --------------- | ---------- | -----------
class     | {String}        |            |
tabs      | {Object/blocks} |            |
nav_align | {String}        |            |
UID       | {String}        | section.id |

# section-body

> Description

### Accepts:

Name            | Type      | Default | Description
--------------- | --------- | ------- | -------------------------------------
class           | {String}  |         | optional, class for section container
id              | {String}  |         | optional, id for section container
type            | {String}  |         | section type for js hooks
content         | {String}  |         | section content
title           | {String}  |         |
container       | {Boolean} |         |
spaced          | {Boolean} |         |
button_text     | {String}  |         |
button_link     | {String}  |         |
use_settings    | {Boolean} |         |
from_blocks     | {Boolean} |         |
content_wrapper | {Boolean} |         |
full_container  | {Boolean} |         |

# social-list

> Description

### Accepts:

Name         | Type      | Default | Description
------------ | --------- | ------- | -----------
color_schema | {String}  |         |
centered     | {Boolean} |         |
rounded      | {Boolean} |         |

# social-sharing

> Description

### Accepts:

Name         | Type      | Default | Description
------------ | --------- | ------- | -----------
color_schema | {String}  |         |
centered     | {Boolean} |         |
rounded      | {Boolean} |         |

# ui-atts

> It's hot!

### Accepts:

Name | Type     | Default | Description
---- | -------- | ------- | -----------
atts | {String} |         |

# video-box

> It's hot!

### Accepts:

Name              | Type          | Default | Description
----------------- | ------------- | ------- | ------------------------------------------------------------------------------------------------------------
class             | {String}      |         | optional class for section container
video             | {Object}      |         |
aspect_ratio      | {String}      |         |
overlay           | {Number}      |         |
overlay_direction | {String}      |         | left/center/right only for overlay_blur and overlay_gradient should be the same as injected content aligment
overlay_blur      | {Boolean}     |         |
overlay_gradient  | {Boolean}     |         |
content           | {String/HTML} |         |
