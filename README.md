Basic structure for Meteor

<pre>
+ client (클라이언트에서만 실행되는 폴더)
|-+ helpers
| |- config.coffee (전역 설정 파일 - Accounts config 등)
| |- handlebars.coffee (전역 헬퍼 - pluralize 등)
|
|-+ stylesheets
| |- style.css
|
|-+ templates
| |-+ application (전체적인 틀 마크업 파일)
| | |- layout.html (기본 라우팅을 위한 틀)
| | |- not_found.html (404 not found 페이지)
| |
| |-+ includes (공통 인클루드 파일 - 헤더, 로딩 등)
|   |- access_denied.html
|   |- header.html
|   |- loading.html
|
|-+ posts
  |- post_item.coffee
  |- post_item.html
  |- posts_list.coffee
  |- posts_list.html

+ lib (제일 먼저 로드되는 폴더)
|-+ collections (컬렉션)
| |- posts.coffee
|
|- permissions.coffee (접근 권한 설정 파일)
|- router.coffee (라우터)

+ server (서버에서만 실행되는 폴더)
|- fixtures.coffee (더미 데이터)
|- publications.coffee (발행관련 파일)
</pre>
