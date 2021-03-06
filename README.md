# 系统设计
## 项目名称
使用python语言爬取豆瓣网信息
## 开发环境及工具
python3.7
MySQL数据库
## 项目目标
自动爬取豆瓣网信息不少于1000条
## 数据库建立
  先建立数据库douban_movie,再在数据库中建表movies，表中需包含编号，电影名，评分，链接，是否可播放等表项。
  用pymysql库连接数据库服务器。

# 操作说明
## 启动MySQL数据库连接
  首先在管理员模式下启动cmd，在配置好MySQL的前提下，输入 net start mysql命令启动MySQL数据库。
## 修改配置
  需要注意的是，目前设置的MySQL密码为root，如果需要在另外的机器上运行，需要确认该计算机配置的MySQL密码。
  如有不同，需要分别在creat_table和run文件中更改MySQL密码后才可以正常运行。具体修改位置如下图所示。
    
![image](https://github.com/QRuuuuu/python/blob/master/creat.png)

![image](https://github.com/QRuuuuu/python/blob/master/run.png)
## 运行
  在确认更改好MySQL密码之后，在python3.7环境下，首先运行creat_table文件，进行数据库的建表等准备操作。
  然后运行run文件，即可进行对豆瓣网相关信息的爬虫。

# 测试结果
  系统可以自动对豆瓣网进行爬虫，对收集到的电影名称，评分等信息按行存入数据库中。
  系统可以容纳爬取1000条以上的豆瓣网电影信息。部分爬取信息截图如下图所示。
    
![image](https://github.com/QRuuuuu/python/blob/master/IMG_1522.PNG)

![image](https://github.com/QRuuuuu/python/blob/master/IMG_1527.PNG)
 

