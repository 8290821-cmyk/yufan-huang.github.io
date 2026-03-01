---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
      button:
        text: Download CV
        # 修正 1：加上开头的斜杠，确保路径正确
        url: "/uploads/resume.pdf" 
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle

  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      # 修正 2：确保文本逻辑完整，去掉了末尾多余的一个引号
      text: |-
        I explore how virtual environments and digital characters can be designed to improve human well-being and social interaction. From investigating user behavior in VR to developing interactive prototypes for digital healthcare, my goal is to create seamless and meaningful experiences. I enjoy combining technical development with empirical user research to understand the impact of emerging technologies on users.
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
      title: Selected Works
      text: ''
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation

# 修正 3：这里必须有这三个横杠作为 YAML 的结束标志！
---
