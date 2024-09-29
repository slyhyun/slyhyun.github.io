---
# A section created with the Portfolio widget.
# This section displays content from `content/project/`.
# See https://docs.hugoblox.com/widget/portfolio/
widget: portfolio

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 20

title: ''
subtitle: ''

slides:
  content:
      - title: "Project 1"
        summary: "This project focuses on Computer Vision techniques."
        image: "/images/project1.jpg"  # 이미지 경로를 설정하세요.
        link: "/project/project1"  # 링크를 설정하세요.
        tags: ["CV"]

      - title: "Project 2"
        summary: "A web application built using React for FrontEnd development."
        image: "/images/project2.jpg"
        link: "/project/project2"
        tags: ["FrontEnd"]

      - title: "Project 3"
        summary: "A backend service developed with Node.js."
        image: "/images/project3.jpg"
        link: "/project/project3"
        tags: ["Backend"]



content:
  # Page type to display. E.g. project.
  page_type: project

  # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
  filter_default: 0

  # Filter toolbar (optional).
  # Add or remove as many filters (`filter_button` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove the toolbar, delete the entire `filter_button` block.
  filter_button:
    - name: All
      tag: '*'
    - name: Computer Vision
      tag: CV
    - name: FrontEnd
      tag: FrontEnd
    - name: BackEnd
      tag: Backend 

design:
  columns: '1'
  view: masonry
  flip_alt_rows: true
  background: {}
  spacing: {padding: [0, 0, 0, 0]}
---
