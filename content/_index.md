---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  - block: collection
    id: publications
    content:
      title: Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: features
    id: skills
    content:
      title: Skills
      items:
        - name: Chinese
          description: 100%
        - name: English
          description: 85%
        - name: Spanish
          description: 75%
        - name: Catalan
          description: 50%
        - name: Word
          description: 90%
        - name: Excel
          description: 75%
        - name: PowerPoint
          description: 75%
        - name: R
          description: 50%
          icon: r-project
          icon_pack: fab
        - name: Stata
          description: 75%
          icon: chart-line
          icon_pack: fas
        - name: Python
          description: 20%
          icon: camera-retro
          icon_pack: fas
  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Lecturer
          company: Pompeu Fabra University
          company_url: ''
          company_logo: org-gc
          location: Barcelona
          date_start: '2018-10-01'
          date_end: ''
          description: |2-
              Responsibilities include:

              * Teaching of Asian Political Systems
              * Teaching of Geopolitics and International Relations in Asia-Pacific
            
        - title: Business Manager
          company: China Railway 24th Bureau Co.,Ltd
          company_url: ''
          company_logo: org-x
          location: Beijing
          date_start: '2014-08-01'
          date_end: '2018-09-15'
          description: Marketing in Latin America, coordination of international biddings.
    design:
      columns: '2'
  - block: markdown
    id: gallery
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Feel free to send me a message (No ads please).
      # Contact (add or remove contact options as necessary
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: true
    design:
      columns: '2'
---
