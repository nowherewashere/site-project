---
# Оставьте заголовок главной страницы пустым, чтобы использовать заголовок сайта
title: "Повелитель Кринжа"
date: 2022-10-24
type: landing

design:
  # Стандартное расстояние между секциями
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Выберите профиль пользователя для отображения (имя папки в `content/authors/`)
      username: admin
      text: ""
      # Показать кнопку призыва к действию под биографией? (опционально)
    design:
      css_class: dark
      background:
        color: black
        image:
          # Добавьте фоновое изображение в `assets/media/`.
          filename: polygon.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: collection
    content:
      title: Проекты
      text:
      filters:
        folders:
          - project
    design:
      view: article_grid
      full_image: false
      columns: 2
  - block: collection
    id: news
    content:
      title: Щитпостинг
      subtitle: ''
      text: ''
      # Тип страницы для отображения. Например, post, talk, publication...
      page_type: post
      # Выберите, сколько страниц вы хотите отобразить (0 = все страницы)
      count: 0
      # Фильтр по критериям
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Выберите, сколько страниц вы хотите пропустить
      offset: 0
      # Порядок страниц: по убыванию (desc) или возрастанию (asc) даты.
      order: desc
    design:
      # Выберите вид макета
      view: date-title-summary
      # Уменьшите отступы
      spacing:
        padding: [0, 0, 0, 0]
  - block: resume-experience
    content:
      title: Опыт
      username: admin
    design:
      # Формат даты Hugo
      date_format: 'January 2006'
      # Образование или Опыт в первую очередь?
      is_education_first: false
  - block: resume-skills
    content:
      title: Навыки и Хобби
      username: admin
    design:
      show_skill_percentage: false
  - block: resume-awards
    content:
      title: Награды
      username: admin
    design:
      show_skill_percentage: false
  - block: resume-languages
    content:
      title: Языки
      username: admin
---
