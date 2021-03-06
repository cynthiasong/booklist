# BookList：利用GiHub搭建个人/团队书单系统

信息最后更新时间：2017-02-23 09:19:16

**运行环境：**
Python 3 + requests

[安装Python 3](https://www.python.org/download/releases/3.0/)

[安装requests](http://docs.python-requests.org/en/master/user/install)

**使用方法：**

1. 将本版本库Fork到自己的GitHub账号上
2. 将建立的新版本库Clone到本地
3. 在本地修改`INTRO.md`（生成在顶部的固定信息）
4. 修改`RAWLIST.md`（转换前的书单）
5. 运行`main.py`，自动从豆瓣API获取书籍信息，格式化保存到`README.md`
6. 完成后提交到自己的远程库

**`RAWLIST.md`填写说明：**

1. 每一行代表一本书，基本格式：`《书名》补充信息 id00000000`
2. 建议使用`《书名》`格式添加大多数书籍
3. 如果书名搜索结果不唯一，可选择添加补充信息或者指定书籍id
4. 书籍id为豆瓣网址最后的一串数字，如书籍网址为`https://book.douban.com/subject/5421787/`，则id为`5421787`
5. 可以使用`find_book.py`从控制台搜索书籍id
6. Markdown二级标题代表分类

可接受的格式示例如下：
```
《重新定义公司》
《人类简史》从动物到上帝
《经济学原理》第7版 id26435630
id11445548
```

以下为`RAWLIST.md`转换后的示例书单：


##思维
|书名|豆瓣评分|评分人数|常用标签|出版时间|页数|作者|
|---|---|---|---|---|---|---|
|[人类简史](https://book.douban.com/subject/25985021)|9.3|21458|历史; 人类简史; 人类学|2014-11|440|[以色列]尤瓦尔·赫拉利|
|[金字塔原理](https://book.douban.com/subject/1020644)|8.1|3695|思维; 金字塔原理; 逻辑|2002-12|290|[美] 巴巴拉·明托|

##数据分析
|书名|豆瓣评分|评分人数|常用标签|出版时间|页数|作者|
|---|---|---|---|---|---|---|
|[统计数字会撒谎](https://book.douban.com/subject/3595095)|7.5|2175|统计学; 统计; 经济|2009-3|154|[美] 达莱尔·哈夫|
|[精益数据分析](https://book.douban.com/subject/26278639)|8.3|203|数据分析; 商业; 互联网|2014-12|356|[加] 阿利斯泰尔·克罗尔,[加] 本杰明·尤科维奇|
|[鲜活的数据](https://book.douban.com/subject/19952397)|7.6|272|数据可视化; 数据分析; 数据|2012-10-1|281|[美] Nathan Yau|

##经济学
|书名|豆瓣评分|评分人数|常用标签|出版时间|页数|作者|
|---|---|---|---|---|---|---|
|[经济学的思维方式（原书第13版）](https://book.douban.com/subject/26604224)|9.0|74|经济学; 经济; 思维|2015-9|432|保罗·海恩 (Paul Heyne),彼得•勃特克（Peter Boettke）,大卫•普雷契特科（David Prychitko）|
|[经济学原理(第7版):微观经济学分册+宏观经济学分册(套装共2册)](https://book.douban.com/subject/26435630)|9.4|423|经济学; 经济; 曼昆经济学|2015-5-1|918|曼昆 (N.Gregory Mankiw)|
|[经济学](https://book.douban.com/subject/20502310)|9.4|92|经济学; 萨缪尔森; 教材|2013-1|652|[美] 保罗·萨缪尔森,[美] 威廉·诺德豪斯|

##心理学
|书名|豆瓣评分|评分人数|常用标签|出版时间|页数|作者|
|---|---|---|---|---|---|---|
|[改变心理学的40项研究](https://book.douban.com/subject/1147347)|8.8|2473|心理学; 改变心理学的40项研究:探索心理学研究的历史; 心理|2004-1-1|425|〔美〕Roger R Hock著|
|[这才是心理学](https://book.douban.com/subject/26287453)|9.1|467|心理学; 批判性思维; 心理|2014-11-1|238|基思·斯坦诺维奇 (Keith E.Stanovich)|
