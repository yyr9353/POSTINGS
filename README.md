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
