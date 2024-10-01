---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: |
        An Hyun
      image:
        filename: welcome.jpg
      text: |
        <br>
        
        I am a student studying computer science and am interested in web programming.
  
  - block: slider
    content:
      slides:

      - title: <span style="font-size:70%">coding</span>
        content: <span style="font-size:70%">study code</span>
        align: center
        background:
          image:
            filename: code1.jpg
            filters:
              brightness: 0.4
          position: center
          color: '#000'
        #link:
        #  icon: user
        #  icon_pack: fas
        #  text: <span style="font-size:60%">Join Us</span>
        #  text-color: '#000'
        #  url: contact

      - title: <span style="font-size:70%">AI</span>
        content: <span style="font-size:70%">learning ai!<span style="font-size:70%">
        align: center
        background:
          image:
            filename: code2.jpg
            filters:
              brightness: 0.4
          position: center
          color: '#000'

      - title: <span style="font-size:70%">Cat</span>
        content: <span style="font-size:70%">Look at the cute cat</span>
        align: center
        background:
          image:
            filename: catimage.jpg
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
      title: <span style="font-size:75%">Interests</span>
      text: I am currently studying the following fields of interest.<br><br><br><br>
      items:
        - name: Artificial Intelligence (AI)
          icon: code-branch
          icon_pack: fas
          description: <span style="font-size:90%">AI technologies such as machine learning, computer vision, and natural language processing.</span><br><br>
        - name: Web Crawling
          icon: globe
          icon_pack: fas
          description:  <span style="font-size:90%">Collecting and utilizing large amounts of data through web crawling.</span><br><br>
        - name: Mathematics
          icon: calculator
          icon_pack: fas
          description:  <span style="font-size:90%">Mathematical theories related to AI, such as linear algebra.</span><br><br>
        - name: Backend Development 
          icon: server
          icon_pack: fas
          description:  <span style="font-size:90%">Server construction and database utilization.</span><br><br>
        - name: Frontend Development 
          icon: laptop
          icon_pack: fas
          description:  <span style="font-size:90%">Building websites using tools like React.</span><br><br>
        - name: App Development
          icon: app-store-ios
          icon_pack: fab
          description:  <span style="font-size:90%">App development using Android Studio!</span><br><br>

  - block: collection
    content:
      id: section-1
      title: Skills
      subtitle:
      text:
      count: 3
      offset: 0
      order: desc
      filters:
        folders:
          - notification
          - post
          - event
    design:
      view: community/custom_card
      columns: '2'

  - block: collection
    content:
      id: section-2
      title: Lastest Activities
      subtitle:
      text:
      count: 3
      offset: 0
      order: desc
      filters:
        folders:
          - notification
          - post
          - event
    design:
      view: community/custom_card
      columns: '2'

  - block: collection
    content:
      id: section-3
      title: Lastest Project
      subtitle:
      text:
      count: 3
      offset: 0
      order: desc
      filters:
        folders:
          - notification
          - post
          - event
    design:
      view: community/custom_card
      columns: '2'

  - block: contact
    content:
      title: Contact
      text: |-
        <br> <span style="font-size:95%">전북대학교 의료 AI 및 계산 수학 연구실 (Macs)의 학부연구생/석사 position에 관심 있으시면 아래로 연락주시면 감사드리겠습니다.</span> <br>
      email: ksl(at)jbnu.ac.kr
      phone: +82-63-270-2406
      address:
        street: 전북대학교 공과대학 7호관 626호
        city: 전주시
        region: 전라북도
        postcode: '54896'
        country: 대한민국
        country_code: KO
      coordinates:
        latitude: '35.84601324617979'
        longitude: '127.13444961966684'
      directions: 
      #contact_links:
      #  - icon: comments
      #    icon_pack: fas
      #    name: Discuss on Forum
      #    link: 'https://discourse.gohugo.io'
    
      # Automatically link email and phone or display as text?
      autolink: true
    
      # # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
      #     # Enable CAPTCHA challenge to reduce spam?
      #     captcha: true
    design:
      columns: '3'

#  - block: collection
#    content:
#      title: Latest Publications
#      subtitle:
#      text:
#      count: 3
#      filters:
#        author: ''
#        category: ''
#        exclude_featured: false
#        publication_type: ''
#        tag: ''
#      offset: 0
#      order: desc
#      page_type: publication
#    design:
#      view: community/custom_card
#      columns: '2'
#    advanced:
#      css_style: "text-align: center;"


#  - block: markdown
#    content:
#      title:
#      subtitle:
#      text: |
#        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
#    design:
#      columns: '1'
---