---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: markdown
    content:
      title:
      text: |
        <div style="display: flex; justify-content: center; align-items: center; gap: 50px;">
          <!-- 왼쪽: 프로필 사진과 이름, 학교 정보 -->
          <div style="display: flex; flex-direction: column; align-items: center;">
            <img src="avatar.jpg" alt="프로필 사진" style="border-radius: 100%; width: 200px; height: 200px; object-fit: cover; margin-bottom: 10px;">
            <p style="font-size: 120%; font-weight: bold; margin: 5px 0;color: white;">An Hyun</p>
            <p style="font-size: 100%;color: white;">Jeonbuk National University</p>
            <p style="font-size: 80%;color: white;">Department of Computer Science and Engineering</p>
          </div>
          <!-- 오른쪽: 소개 정보 -->
          <div style="text-align: left; max-width: 500px;">
            <p style="font-size: 120%; font-weight: bold; margin: 5px 0;color: white;">About Me</p>
            <p style="font-size: 100%;color: white;">
              I'm An Hyun, a third-year computer engineering and science student at JBNU. I want to be a back-end developer.<br>
              <a href="https://github.com/slyhyun" target="_blank" style="text-decoration: underline; color: #946efd;">Go To Github</a>
            </p>
          </div>
        </div>
    design:
      columns: '1'
      background:
        image:
          filename: star.jpg
          filters:
            brightness: 0.5
        overlay:  # 오버레이 추가
          color: '#ffffff'  # 흰색
          opacity: 0.5  # 투명도 조절
    button:
      text: 최근 작성 문서
      url: uploads/document.pdf
  
  
  - block: features
    id: features
    content:
      title: <span style="font-size:75%">Tech Stack</span>
      text: 
      items:
        - name: Python
          icon: python
          icon_pack: fab
        - name: C/C++
          icon: copyright
          icon_pack: fas
        - name: Java
          icon: java
          icon_pack: fab
        - name: Node.js
          icon: node-js
          icon_pack: fab
        - name: React
          icon: react
          icon_pack: fab
        - name: Spring Boot
          icon: leaf
          icon_pack: fas

  - block: slider
    content:
      slides:
        - title: <span style="font-size:70%">Back-end</span>
          content: <span style="font-size:70%">Spring Boot, Node.js, Django</span>
          align: center
          background:
            image:
              filename: code1.jpg
              filters:
                brightness: 0.5
            position: center
            color: '#000'
        
        - title: <span style="font-size:70%">Front-end</span>
          content: <span style="font-size:70%">React, Vue.js, Angular</span>
          align: center
          background:
            image:
              filename: code2.jpg
              filters:
                brightness: 0.5
            position: center
            color: '#000'
          
        - title: <span style="font-size:70%">Artificial Intelligence</span>
          content: <span style="font-size:70%">Natural Language Processing, Computer Vision</span>
          align: center
          background:
            image:
              filename: researchpaper.jpg
              filters:
                brightness: 0.5
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
      flip_alt_rows: true

  - block: contact  # contact 블록의 '-' 기호를 들여쓰기를 통해 해결
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
        street: JBNU Chambit Hall 1, No. 524
        city: Jeonju
        region: Jeollabuk-do
        postcode: '54896'
        country: Republic of Korea
        country_code: KO
      coordinates:
        latitude: '35.850785'
        longitude: '127.126310'
      directions: 
      autolink: true
    design:
      columns: '3'
---
