---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: 'My Mission'
      subtitle: ''
      text: |-
        Dedicated to advancing knowledge through rigorous research, critical inquiry, and interdisciplinary collaboration.
        
        Committed to contributing original scholarship in Software Engineering, mentoring students, and engaging in meaningful academic service.

        My mission is to foster intellectual curiosity, support academic integrity, and promote inclusive excellence within higher education and research communities.

    design:
      columns: '1'
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
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: cta-card
    demo: false # Only display this section in the Hugo Blox Builder demo site
    content:
      title: Contact me for collaboration
      text: |-
        I welcome opportunities for academic collaboration and interdisciplinary research.

        My current interests lie in Software Engineering, and I am particularly eager to engage in projects that intersect with Economics.
      button:
        text: Send a message
        url: '#'
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
