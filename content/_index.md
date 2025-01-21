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
  - block: markdown
    id: gallery
    content:
      title: Gallery
      text: |
        <div style="display: flex; overflow-x: auto; gap: 10px; padding: 20px; scroll-behavior: smooth;">
          <style>
            /* Custom Scrollbar */
            div[style*="overflow-x: auto"]::-webkit-scrollbar {
              height: 10px;
              background-color: #f0f0f0;
            }

            div[style*="overflow-x: auto"]::-webkit-scrollbar-thumb {
              background-color: #888;
              border-radius: 10px;
            }

            div[style*="overflow-x: auto"]::-webkit-scrollbar-thumb:hover {
              background-color: #555;
            }

            /* Image hover effect */
            .gallery-image:hover {
              transform: scale(1.1);
              transition: transform 0.3s ease;
            }
          </style>
        <div style="display: flex; overflow-x: auto; gap: 10px; padding: 20px; scroll-behavior: smooth;">
          <img src="gallery/CAN_exports.png" alt="Photo 1" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/combined_image_2.png" alt="Photo 2" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/data_viz.png" alt="Photo 3" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/diplomaticos.png" alt="Photo 4" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/graph_2.png" alt="Photo 5" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/graph1.jpg" alt="Photo 6" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/ine.png" alt="Photo 7" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/map.png" alt="Photo 8" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/nafta.png" alt="Photo 9" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/PCA_2.png" alt="Photo 10" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/PCA.png" alt="Photo 11" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/pi.png" alt="Photo 12" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/reap_cor.png" alt="Photo 13" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/regression.png" alt="Photo 14" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/rf.png" alt="Photo 15" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/roc.png" alt="Photo 16" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/us_cd1.png" alt="Photo 17" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/usa_max_exp.png" alt="Photo 18" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
          <img src="gallery/words.png" alt="Photo 19" style="width: 150px; height: auto; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);">
        </div>
    design:
      columns: '1'
      view: showcase
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
