---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: 
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
    design:
      css_class: 
  - block: collection
    id: work
    content:
      title: Work
      filters:
        folders:
          - work
        exclude_featured: true
    design:
      columns: '2'
      view: compact
  - block: collection
    id: education
    content:
      title: Education
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 0
      # Filter on criteria
      filters:
        folders:
          - education
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'  
  - block: collection
    id: projects
    content:
      title: Projects
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - projects
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
 - block: github.chicurel.gallery-hugo-blox
  id: gallery-hugo-blox
  content:
    title: Gallery
    images:
      - src: gallery/CAN_exports.png
        alt: Photo 1
      - src: gallery/combined_image_2.png
        alt: Photo 2
      - src: gallery/data_viz.png
        alt: Photo 3
      - src: gallery/diplomaticos.png
        alt: Photo 4
      - src: gallery/graph_2.png
        alt: Photo 5
      - src: gallery/graph1.jpg
        alt: Photo 6
      - src: gallery/ine.png
        alt: Photo 7
      - src: gallery/map.png
        alt: Photo 8
      - src: gallery/nafta.png
        alt: Photo 9
      - src: gallery/PCA_2.png
        alt: Photo 10
      - src: gallery/PCA.png
        alt: Photo 11
      - src: gallery/pi.png
        alt: Photo 12
      - src: gallery/reap_cor.png
        alt: Photo 13
      - src: gallery/regression.png
        alt: Photo 14
      - src: gallery/rf.png
        alt: Photo 15
      - src: gallery/roc.png
        alt: Photo 16
      - src: gallery/us_cd1.png
        alt: Photo 17
      - src: gallery/usa_max_exp.png
        alt: Photo 18
      - src: gallery/words.png
  - block: contact
    id: contact
    content:
      title: Contact
      # Contact (add or remove contact options as necessary)
      email: chicureledgar@gmail.com
      address:
        street: Calle de Albasanz, 26
        city: Madrid
        region: 
        postcode: 28037
        country: Spain
        country_code: ES
      directions: Office 3D16
      phone: +34 691 345 024
      # Automatically link email and phone or display as text?
      autolink: true
    design:
      columns: '2'
---
