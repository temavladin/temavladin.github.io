---
# Leave the homepage title empty to use the site title
title: ""
date: 2025-03-08
type: landing

design:
  # Default section spacing
  spacing: "1rem"

sections:
 # - block: biography
 #   content:
 #     username: admin
 #     # Show a call-to-action button under your biography? (optional)
 #     #button:
 #     #  text: Download Résumé
 #     #  url: uploads/resume.pdf
 #   design:
 #     banner:
 #       # Upload your cover image to the `assets/media/` folder and reference it here
 #       filename: 3219647517.jpg
 #     biography:
 #       # Customize the style of your biography text
 #       style: 'text-align: justify; font-size: 0.8em;'
  - block: markdown
    content:
      title: '<h1 style="text-align: center; font-size: 0.6em;">СИСТЕМА ЭЛЕКТРОДОКУМЕНТОВ ВЛАДИНА</h1>'
      subtitle: ''
      text: '<p style="text-align: center; font-size: 0.7em;">Общедоступный узел информационно-телекоммуникационной сети.</p> <p style="text-align: center; font-size: 0.7em;">Санкт-Петербург 2025</p> {{% callout warning %}} <p style="text-align: left; font-size: 0.7em;">Если сервер возвращает ошибку, то используйте архивную версию системы.</p> {{% /callout %}} {{< cards >}} {{< card url="/docs" title="Рабочие тетради" subtitle="Основные многостраничные публикации" >}} {{< /cards >}}'
    design:
      columns: '1'
      style: 'font-size: 0.5em;'
#  - block: collection
#    id: posts
#    content:
#      title: '<h1 style="text-align: center; font-size: 0.7em;">Поздравления</h1>'
#      subtitle: ''
#      text: ''
#      # Choose how many pages you would like to display (0 = all pages)
#      count: 2
#      # Filter on criteria
#      filters:
#        # The folders to display content from
#        folders:
#          - main
#        author: ""
#        category: ""
#        tag: ""
#        publication_type: ""
#        featured_only: false
#        exclude_featured: false
#        exclude_future: false
#        exclude_past: false
#      # Choose how many pages you would like to offset by
#      # Useful if you wish to show the first item in the Featured widget
#      offset: 0
#      # Field to sort by, such as Date or Title
#      sort_by: 'Date'
#      sort_ascending: false
#    design:
#      # Choose a listing view
#      view: article-grid
#      columns: 2
  - block: collection
    id: news
    content:
      title: '<h1 style="text-align: center; font-size: 0.7em;">Новые записи в тетрадях</h1>'
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: docs
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
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
      view: citation
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: collection
    id: news
    content:
      title: '<h1 style="text-align: center; font-size: 0.7em;">Последние заметки</h1>'
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
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
      view: title
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: markdown
    content:
      title: 'Обратная связь'
      subtitle: ''
      text: |-
        Автор будет признателен за любые отзывы, пожелания и критические замечания, которые можно присылать в сообщения [Вконтакте](https://vk.com/temavladin) .
    design:
      columns: '1'
  - block: markdown
    content:
      title: 'Служебные файлы'
      subtitle: ''
      text: |-
        Карта сайта [sitemap](https://temavladin.github.io/sitemap.xml)
    design:
      columns: '1'
---
