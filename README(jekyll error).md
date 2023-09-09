3. bundle exec jekyll serve 오류 해결하기(tzinfo error)
bundle exec jekyll serve 명령어를 입력했는데
jekyll 4.1.1 | Error: tzinfo 이런 오류가 발생하시는 분들이 계실겁니다.

이런 오류가 뜨시는 분들은 다음과 같이 진행하시면 됩니다.
레파지토리 폴더 내에 보면 루트 디렉토리에 Gemfile이라는 파일이 있을 것입니다.
이 파일을 열고 다음과 같은 내용을 추가해주시면 됩니다.
gem 'tzinfo'
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw]

아래와 같은 오류가 뜬다 하시는 분들은 tzinfo를 수동으로 설치해 줘야 합니다.
C:/Ruby26-x64/lib/ruby/gems/2.6.0/gems/bundler-2.1.4/lib/bundler/resolver.rb:290:in `block in verify_gemfile_dependencies_are_found!': Could not find gem 'tzinfo x64-mingw32' in any of the gem sources listed in your Gemfile. (Bundler::GemNotFound)

레파지토리 폴더의 위치에서 다음 명령어를 입력해서 tzinfo를 설치하면 문제가 해결될 것입니다.
$ gem install tzinfo -v "~> 1.2"
$ gem install tzinfo-data
이번에는 깃 허브 블로그의 개발환경을 만드는 방법에 대해서 다뤄보았습니다. 이렇게 설정을 해두면 일일이 commit 해서 확인하는 과정을 거칠 필요 없이 실시간으로 변경 사항을 확인할 수 있습니다.
다음에는

disqus

를 이용해서 블로그에 댓글 기능을 추가하는 방법에 대해 알아보도록 하겠습니다.

