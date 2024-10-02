---
title: Introduce
date: 2022-10-24

type: landing

sections:
  - block: people
    content:
      title: An Hyun
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
          - Student
      sort_by: Params.last_name
      sort_ascending: true
    design:
      show_interests: true
      show_role: true
      show_social: true
      show_education: true
      show_languages: true
      show_certifications: true
      show_goals: true  
  # Markdown 텍스트 블록을 추가하여 문구 출력
  - block: markdown
    content:
      text: |
        <p style="font-size: 0.8em; text-align: center; color: #ffffff;">
          details - <strong>click the name</strong>
        </p>
    design:
      columns: '1'
---