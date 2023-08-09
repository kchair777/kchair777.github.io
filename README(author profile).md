# author profile 
1. _posts폴더 md화일
  ---
  layout : single 
  title : 4.한글 타이틀_박문호박사의 뇌과학이란
  category: python, coding
  tag: coding
  nav:  blog
  theme: 깃헙
  author_profile: false
  ---
# sidebar navigation
1. _data > navigation.yml
  1. docs: 
    -title : "내목차"
    children:
      - title: "Category"
        url: /Categories/
      - title: "Tag"
        url: /tags/

# 검색기능 추가 
1. _pages
  1.search.md추가 
    ---
    title: search
    layout: search
    permalink: /search/
    ---
1. _data
  1. navigation.yml main밑에 
    -title: "Search"
     url: /search/
  2. 만약search필요 없다면 
     search: false 추가
