# font추가 
1. google font
  1. _sass > minimal-mistakes.scss
    @import url('https://fonts.googleapis.com/css2?family=Nanum+Gothic&display=swap');
  1. _variables.scss
    /* google font */
    'Nanum Gothic'
  
# Avatar 사진 
1. _config.yml
  1.Site Author
    avator: **"/images/gallery01.jpg"**    
1. server reload 
  1. bundle exec jekyll serve --livereload