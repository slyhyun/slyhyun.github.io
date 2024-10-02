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
        filename: Anhyun.jpg
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
      title: Academic
      subtitle:
      text:
      count: 3
      offset: 0
      order: desc
      filters:
        folders:
          - course
    design:
      view: community/custom_compact
      columns: '2'

  - block: collection
    content:
      id: section-2
      title: Activity
      subtitle:
      text:
      count: 3
      offset: 0
      order: desc
      filters:
        folders:
          - department
          - club
    design:
      view: community/custom_card
      columns: '2'

  - block: collection
    content:
      id: section-3
      title: Project
      subtitle:
      text:
      count: 3
      offset: 0
      order: desc
      filters:
        folders:
          - personal
          - team
    design:
      view: community/custom_showcase
      columns: '2'

  - block: contact
    content:
      title: Contact
      contact_links:
      - icon: instagram
        icon_pack: fab
        name: slyhyun_
        link: https://www.instagram.com/slyhyun_
      - icon: github
        icon_pack: fab
        name: slyhyun
        link: https://github.com/slyhyun
      address:
        street: JBNU Chambit Hall 1, Room 524
        city: 전주시
        region: 전라북도
        postcode: '54896'
        country: 대한민국
        country_code: KO
      coordinates:
        latitude: '35.84601324617979'
        longitude: '127.13444961966684'
      directions: 
      autolink: true
    design:
      columns: '3'
---