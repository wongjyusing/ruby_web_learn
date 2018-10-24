## 创建项目和配置
首先创建一个名为**rails_blog**的项目。  
`rails new rails_blog`  
进入rails_blog目录下并查看目录结构。  
`cd rails_blog && tree`   
如下：
```bash
.
├── app                              # 应用目录
│   ├── assets                       # 财富？？不对，应该是静态文件目录
│   │   ├── config                   # 配置目录
│   │   │   └── manifest.js          # 显示的js文件
│   │   ├── images                   # 图片目录
│   │   ├── javascripts              # js文件目录
│   │   │   ├── application.js       # 应用的js
│   │   │   ├── cable.js             # 电缆？？  
│   │   │   └── channels             # 渠道？？线槽？
│   │   └── stylesheets              # 样式目录
│   │       └── application.css      # 应用的样式css文件
│   ├── channels                     # 渠道？？线槽？目录
│   │   └── application_cable        # 应用的电缆
│   │       ├── channel.rb           # 电缆文件
│   │       └── connection.rb        # 连接文件
│   ├── controllers                  # 控制器目录
│   │   ├── application_controller.rb # 控制文件  
│   │   └── concerns                 # 关系关联目录
│   ├── helpers                      # 帮助，很像django的自定义模板方法
│   │   └── application_helper.rb    # 应用的帮助
│   ├── jobs                         # 工作？？
│   │   └── application_job.rb       # 应用工作？？
│   ├── mailers                      # 邮差
│   │   └── application_mailer.rb    # 邮件方面的文件
│   ├── models                       # 模型 ORM方面的目录
│   │   ├── application_record.rb    # 应用的记录文件
│   │   └── concerns                 # 链接目录？？  
│   └── views                        # 视图
│       └── layouts                  # 很像vue的App.vue的功能
│           ├── application.html.erb
│           ├── mailer.html.erb
│           └── mailer.text.erb
├── bin                              # 工具箱
│   ├── bundle                       # 建造
│   ├── rails                        # 主要命令，用于运行
│   ├── rake                         # 这个相当于是django的shell
│   ├── setup                          
│   ├── spring
│   ├── update
│   └── yarn
├── config
│   ├── application.rb
│   ├── boot.rb
│   ├── cable.yml
│   ├── credentials.yml.enc
│   ├── database.yml                # 这个是数据库的配置       
│   ├── environment.rb
│   ├── environments
│   │   ├── development.rb
│   │   ├── production.rb
│   │   └── test.rb
│   ├── initializers
│   │   ├── application_controller_renderer.rb
│   │   ├── assets.rb
│   │   ├── backtrace_silencers.rb
│   │   ├── content_security_policy.rb
│   │   ├── cookies_serializer.rb
│   │   ├── filter_parameter_logging.rb
│   │   ├── inflections.rb
│   │   ├── mime_types.rb
│   │   └── wrap_parameters.rb
│   ├── locales
│   │   └── en.yml
│   ├── master.key
│   ├── puma.rb
│   ├── routes.rb                   # 路由相当与django的urls.py
│   ├── spring.rb
│   └── storage.yml
├── config.ru
├── db                              # 数据库的配置
│   └── seeds.rb
├── Gemfile
├── Gemfile.lock
├── lib
│   ├── assets
│   └── tasks
├── log
├── package.json
├── public
│   ├── 404.html
│   ├── 422.html
│   ├── 500.html
│   ├── apple-touch-icon.png
│   ├── apple-touch-icon-precomposed.png
│   ├── favicon.ico
│   └── robots.txt
├── Rakefile
├── README.md
├── storage
├── test
│   ├── application_system_test_case.rb
│   ├── controllers
│   ├── fixtures
│   │   └── files
│   ├── helpers
│   ├── integration
│   ├── mailers
│   ├── models
│   ├── system
│   └── test_helper.rb
├── tmp
│   ├── cache
│   │   └── assets
│   └── storage
└── vendor

44 directories, 61 files
```
看不懂的暂时不翻译了。   
启动项目  
`bin/rails server`  
打开本地的3000端口可以看到的内容。  
和django的介绍差不多。  
一个欢迎界面，然后是文档和社区的链接。  
