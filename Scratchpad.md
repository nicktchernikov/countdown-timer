# Blog

* Display posts
    * MySQL table fields: 
        * posted -> integer, timestamp
        * month -> integer, MM format
        * year -> integer
        * title -> string, post title
        * content -> string, post content
* Pagination  
* Display posts from a particular month and year
* Post editor
    * only accessible to admin
    * create new post button
    * edit existing post button
        * dropdown of existing post titles 
        * gets from MySQL 
    * textarea for content editing
    * text input for post title
    * submit button
        * posts to MySQL