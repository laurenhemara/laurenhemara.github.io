---
# Leave the homepage title empty to use the site title
title: "Lauren Hemara"
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "2rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      #button:
      #  text: Download CV
      #  url: uploads/resume.pdf
    design:
      background:
        #gradient_start: '#9ebd13'
        #gradient_end: '#508708'
        #gradient_angle: 180
        color: '#F7F7F7'
        #image:
        #  # Add your image background to `assets/media/`.
         #filename: green.svg
        # filters:
        #    brightness: 1.0
        # size: cover
        # position: center
        # parallax: false
  #- block: markdown
  #  content:
  #    title: '📚 My Research'
  #    subtitle: ''
  #    text: |-
  #      Use this area to speak to your mission. I'm a research scientist in the Moonshot team at DeepMind. I blog about machine learning, deep learning, and moonshots.

  #  design:
  #    columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    content:
      title: Recent Publications
      text: ""
      count: 3
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: compact
      columns: '1'
      css_style: 'background-color: #F7F7F7;'
  #- block: collection
  #  id: talks
  #  content:
  #    title: Recent & Upcoming Talks
  #    filters:
  #      folders:
  #        - event
  #  design:
  #    view: article-grid
  #    columns: 1
  #- block: collection
  #  id: news
  #  content:
  #    title: Recent News
  #    subtitle: ''
  #    text: ''
      # Page type to display. E.g. post, talk, publication...
  #    page_type: post
      # Choose how many pages you would like to display (0 = all pages)
  #    count: 5
      # Filter on criteria
  #    filters:
  #      author: ""
  #      category: ""
  #      tag: ""
  #      exclude_featured: false
  #      exclude_future: false
  #      exclude_past: false
  #      publication_type: ""
      # Choose how many pages you would like to offset by
  #    offset: 0
      # Page order: descending (desc) or ascending (asc) date.
  #    order: desc
  #  design:
      # Choose a layout view
  #    view: date-title-summary
      # Reduce spacing
  #    spacing:
  #      padding: [0, 0, 0, 0]
---
