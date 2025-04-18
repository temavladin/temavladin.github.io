---
# Leave the homepage title empty to use the site title
title: ""
date: 2025-03-08
type: landing

design:
  # Default section spacing
  spacing: "1rem"

sections:
  - block: biography
    content:
      username: admin
      # Show a call-to-action button under your biography? (optional)
      #button:
      #  text: Download Résumé
      #  url: uploads/resume.pdf
    design:
      banner:
        # Upload your cover image to the `assets/media/` folder and reference it here
        filename: 3219647517.jpg
      biography:
        # Customize the style of your biography text
        style: 'text-align: justify; font-size: 0.8em;'
  - block: markdown
    content:
      title: 'Обратная связь'
      subtitle: ''
      text: |-
        Автор будет признателен за любые отзывы, пожелания и критические замечания, которые можно прислать в сообщения [Вконтакте](https://vk.com/temavladin) .
    design:
      columns: '1'
  - block: collection
    id: news
    content:
      title: Последние записи
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post, docs
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: markdown
    content:
      title: 'Карта сайта'
      subtitle: ''
      text: |-
        [sitemap](https://temavladin.github.io/sitemap.xml) .
    design:
      columns: '1'
---
