#README
    
1.Users #사용자 있어야, 많은 포스팅 코멘트 달 수 있어야 한다 #has_many 가질수 있다
    -Relationships
      has_many :Postings
      has_many :Comments
    -Elements
      email/password #있어야

2.Posting
    -Relationships
      belongs_to :Users
      has_many :Comments
    -Elements
      title, body, user_id

3.Comments
    -Relationships
      belongs_to :Users
      belongs_to :Postings
    -Elements
      content, user_id, posting_id
      
      
------------------------------------------------------------

#Controllers
 posting Controllers
 
 Comment Controllers
 
 User => devise gemfile() # 이미 만들어진거(디바이즈라는 젬) 가져다쓴다
 
--------------------------------------------------------------------

#CSS/JS : Bootstrap CDN

--------------------------------
#GIT에 올린다 보험용
다른 사람과의 공유 용이
컴퓨터 고장나도 언제든 다시 다운로드 받을 수 있다

밑에 git init
git status
git add . 1.모든 파일 추가 한다
git commit -m#(message 준말)
git commit -m"update README.md" 2.변경된거 메세지 남기기
git remote add origin https://github.com/yyr9353/POSTINGS.git #처음 연결시만 리코트로 
나머지는 푸쉬를 쓴다 3.깃허브에 파일 올림
 git push -u origin master
 아이디 비번 누른다
 rails g model posting
 db 파일로 들어감
 
 rake db migrate
 
 nav bar 넣을때 어플리케이션에 넣는게 좋다 body 뒤에 넣는다 그래야 다른 페이지로 넘어가더라도 네비바 항상 나오게 할 수 있다
 