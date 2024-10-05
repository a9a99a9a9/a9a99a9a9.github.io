---
# Leave the homepage title empty to use the site title
title: "Hwang Dohoon homepage"
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
        text: Download resume
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
      title: ' SUMMARY '
      subtitle: ''
      text: |-
        
        Hello, I'm Hwang Do Hoon.
        
        I am a student at Chonbuk National University and have a double major in the Department of International Science and Engineering and Computer Artificial Intelligence.
        I've used Kotlin, C, C++, SQL, Node.js, Flutter.

        We run a complex fashion brand called 'Ohread', which likes clothes and books and melts book culture into clothes.

        I worked as a video planner at a fashion YouTube company and experienced content planning, video planning, and filming assistance.
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: subjects in class
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 3
  - block: collection
    content:
      title: class-related links
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Club
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
---