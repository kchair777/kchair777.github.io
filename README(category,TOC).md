# starting category (라인잘맞추어야한다.)
1. _config.yml
  1. jekyll_archcive:
    enabled: 
      - categories
      - tags
    layouts:
      categeory: archive-taxonomy
      tag: archive-taxnonmy
    permalink:
      category: /categoies/:name/
      tag: /tags/:name/ 

2. _pages
  1.category-archive.md
    ---
    title: "category"
    layout: categories
    permalink: /categories/
    author_profile: true
    sidebar_main: true
    ---
  1.tag-archive.md
    ---
    title: "Tag"
    layout: tags
    permalink: /tags/
    author_profile: true
    sidebar_main: true
    ---
  1.nav-archive.md
    ---
    title: "Nav"
    layout: tags
    permalink: /navs/
    author_profile: true
    sidebar_main: true
    ---
3._data
  1.navigation.yml
    main:
  - title: "category"
    url: /categories/

  - title: "Tag"
    url: /tags/

  - title: "Nav"
    url: /navs/

  - title: "Theme"
    url: /themes/
  
  - title: "about"
    url: /about/
4._posts md화일 추가
  ---
  layout : single
  title : 깃허브 블로그
  categories: github
  tag: [github,blog,fork]
  nav: kind
  toc: true
  ---
# TOC 
1. _posts
  1.2021-09-02-first.md
    ---
    layout:single
    title: "첫번째 블로그"
    categories: coding
    tag:[python, blog, jekyll]
    toc: true
    ---
  1.
# 404 page
1. _pages
  1.404.md추가 하기전 test폴더에 가서 
    ---
    title: "Page Not Found"
    excerpt: "Page not found. Your pixels are in another canvas."
    sitemap: false
    permalink: /404.html
    ---
    Sorry, but the page your trying to view does not exist.
  2.F5 실행후 확인 