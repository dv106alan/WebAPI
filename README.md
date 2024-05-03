# WebAPI
使用 Restful API 建立 User Login 系統

API內容：
1. 登入的API會以account跟password來判斷能不能給token
2. 新增使用者的API中 role 只能接受AM / SUBAM / NORMAL 這三種值，否則不給新增
3. 透過解析token的方式來辨別改次登入的使用者權限為何，AM可以執行所有API ; SUBAM只能GET, CREATE, PATCH ; 一般使用者只能GET 以及PATCH自己

使用模組：
flask
flask_restful
marshmallow
