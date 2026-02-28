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
        url: uploads/resume.pdf # 确认一下这里，之前建议改成 /uploads/resume.pdf
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

  # 这里是你之前提到的 Research 介绍，你可以把文字改成你自己的，或者干脆也删掉这一段
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I am a graduate student at KTH Royal Institute of Technology, focusing on HCI and Immersive Media. (建议改掉默认的 DeepMind 文字)
    design:
      columns: '1'

  # 如果你还没有发表论文，建议把下面这两个 block 也删掉，或者暂时留着
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation

  # ----- 我已经帮你删掉了 Recent News 和 Recent & Upcoming Talks -----

  # 这个是底部的广告卡片，建议也删掉或者把 demo 设为 false
  - block: cta-card
    demo: false 
    content:
      title: 👋 Get in Touch
      text: |-
        Feel free to reach out for collaborations!
---
