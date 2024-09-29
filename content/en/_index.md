---
# Leave the homepage title empty to use the site title
title: "My Landing Page"  # 제목 필드 추가
date: 2024-09-30
type: landing

sections:
  - block: features
    content:
      title: "<span style='font-size:70%'>An Hyun </span>"
      text: |
        <br><span style="font-size:125%">I am An Hyun</span> <br><br>
        {{% cta cta_link="./field/" cta_text="See Research Field →" %}}

  - block: slider
    content:
      slides:
        - title: "<span style='font-size:70%'>Web</span>"
          content: "<span style='font-size:70%'>Back-end, Front-end</span>"
          align: center
          background:
            image:
              filename: web.jpg
              filters:
                brightness: 0.4
            position: center
            color: '#000'

        - title: "<span style='font-size:70%'>App</span>"
          content: "<span style='font-size:70%'>IOS, Android</span>"  # 잘못된 HTML 태그 수정
          align: center
          background:
            image:
              filename: app.jpg
              filters:
                brightness: 0.4
            position: center
            color: '#000'

        - title: "<span style='font-size:70%'>AI</span>"
          content: "<span style='font-size:70%'>Vision, Natural language</span>"
          align: center
          background:
            image:
              filename: sample_images_02.png
              filters:
                brightness: 0.4
            position: center
            color: '#000'

    design:
      # Slide height is automatic unless you force a specific height (e.g. '400px')
      slide_height: '350px'
      slide_width: '100px'
      is_fullscreen: false
      # Automatically transition through slides?
      loop: true
      # Duration of transition between slides (in ms)
      interval: 3000

  - block: features
    id: features
    content:
      title: "<span style='font-size:75%'>Interests</span>"
      text: "I am currently studying the following fields of interest.<br><br><br><br>"
      items:
        - name: Artificial Intelligence (AI)
          icon: code-branch
          icon_pack: fas
          description: "<span style='font-size:90%'>AI technologies such as machine learning, computer vision, and natural language processing.</span><br><br>"
        - name: Web Crawling
          icon: globe
          icon_pack: fas
          description: "<span style='font-size:90%'>Collecting and utilizing large amounts of data through web crawling.</span><br><br>"
        - name: Mathematics
          icon: calculator
          icon_pack: fas
          description: "<span style='font-size:90%'>Mathematical theories related to AI, such as linear algebra.</span><br><br>"
        - name: Backend Development 
          icon: server
          icon_pack: fas
          description: "<span style='font-size:90%'>Server construction and database utilization.</span><br><br>"
        - name: Frontend Development 
          icon: laptop
          icon_pack: fas
          description: "<span style='font-size:90%'>Building websites using tools like React.</span><br><br>"
        - name: App Development
          icon: app-store-ios
          icon_pack: fab
          description: "<span style='font-size:90%'>App development using Android Studio!</span><br><br>"

  - block: collection
    content:
      title: Latest News
      subtitle:
      text:
      count: 3
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: post
    design:
      view: card
      columns: '1'
      background:
        # Choose a color such as from https://html-color-codes.info
        color: 'navy'
        # Text color (true=light, false=dark, or remove for the dynamic theme color).
        text_color_light: true

  - block: collection
    content:
      title: Latest Team Project
      subtitle:
      text:
      count: 3
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: team
    design:
      view: card
      columns: '2'
    advanced:
      css_style: "text-align: center;"

  # - block: awards
  #   content:
  #     title: Awards
  #     username: admin

---
