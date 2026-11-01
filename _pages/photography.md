---
layout: page
permalink: /photography/
title: Photography
nav: true
nav_order: 4
# To add a photo: save it as assets/img/photo_<name>.jpg (about 1600 px on the long side) and add an entry here.
# The gallery is a masonry layout (.photo-gallery in _sass/_custom.scss), so portrait and landscape photos mix freely.
photos:
  - file: photo_tower_autumn.jpg
    caption: The McFarland Memorial Bell Tower in autumn
  - file: photo_curtis_apple.jpg
    caption: Apples at Curtis Orchard
  - file: photo_colorado_riders.jpg
    caption: Riders on a mountain road, Colorado
  - file: photo_colorado_road.jpg
    caption: A road-trip stop in the Colorado mountains
  - file: photo_pictured_rocks.jpg
    caption: Fog on the shore near Pictured Rocks, Michigan
  - file: photo_neworleans_anhinga.jpg
    caption: An anhinga drying its wings, New Orleans
  - file: photo_neworleans_raccoon.jpg
    caption: A raccoon, New Orleans
  - file: photo_campfire.jpg
    caption: A campfire at night
  - file: photo_cat_window.jpg
    caption: A cat by the window
  - file: photo_cat.jpg
    caption: A cat looking up
---

Some photos I have taken. Click a photo to see it larger.

<div class="photo-gallery">
{% for photo in page.photos %}
  {% assign photo_path = 'assets/img/' | append: photo.file %}
  {% include figure.liquid loading="lazy" path=photo_path class="img-fluid rounded z-depth-1" zoomable=true alt=photo.caption caption=photo.caption sizes="(min-width: 930px) 300px, (min-width: 576px) 45vw, 95vw" %}
{% endfor %}
</div>
