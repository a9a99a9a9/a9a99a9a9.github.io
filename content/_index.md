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
        
        안녕하세요. 저는 황도훈입니다.
        
        전북대학교에 재학 중이며 국제이공학부와 컴퓨터인공지능학부를 복수 전공 하고 있습니다.
        Kotlin, C, C++, SQL, Node.js, Flutter 를 사용해 본 적이 있습니다.

        옷과 책을 좋아하여 옷에 책 문화를 녹인 'Ohread'라는 복합 패션 브랜드를 운영하고 있습니다.

        패션 유튜브 회사에서 영상 기획자로 일하며 컨텐츠 기획, 영상 기획, 촬영 보조 등을 경험 하였습니다.
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: 수강중인 과목들
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 3
  - block: collection
    content:
      title: 수업 관련 링크
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
      title: 동아리
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
---