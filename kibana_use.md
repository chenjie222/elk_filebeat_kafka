# Discover

## 一、时间过滤器

**1、快速设置过滤器-Quick**

![avatar](https://raw.githubusercontent.com/chenjie222/elk_filebeat_kafka/master/image/001.png)

*从这里可以选今天昨天*

**2、相对时间过滤器-Relative** 

![avatar](https://raw.githubusercontent.com/chenjie222/elk_filebeat_kafka/master/image/002.png)



*从这里可以自定义几小时以前或者几周以前等等* 



**3、绝对时间过滤器-Absolute** 

![avatar](https://raw.githubusercontent.com/chenjie222/elk_filebeat_kafka/master/image/003.png)

*这里是一个绝对的时间，直接选就好了。* 

**4、柱状图时间过滤器** 

**直接点击柱状图即可查看明细** 

![avatar](https://raw.githubusercontent.com/chenjie222/elk_filebeat_kafka/master/image/004.png)

## 二、搜索数据

比如想查询aimachine-service这个项目日志，直接在搜索框搜索

![avatar](https://raw.githubusercontent.com/chenjie222/elk_filebeat_kafka/master/image/005.png)

也可以点击箭头处的保存，保存搜索

![avatar](https://raw.githubusercontent.com/chenjie222/elk_filebeat_kafka/master/image/006.png)*保存成功后我们可以在如下菜单查看* 

![avatar](https://raw.githubusercontent.com/chenjie222/elk_filebeat_kafka/master/image/007.png)![avatar](https://raw.githubusercontent.com/chenjie222/elk_filebeat_kafka/master/image/008.png)

*这里可以导出，也可以点击进去看es查询语法* 

![avatar](https://raw.githubusercontent.com/chenjie222/elk_filebeat_kafka/master/image/009.png)图示位置打开已存搜索

如图所示搜索为模糊查询搜索，需要精确的查询需要使用kabina语法，见下文

### 三、按字段过滤搜索

在Discover页面鼠标悬浮，出现add字段，添加`kubernetes.container.name` 和`message`  这两个字段，当然，也可以按照需求添加其他

add字段前

![avatar](https://raw.githubusercontent.com/chenjie222/elk_filebeat_kafka/master/image/010.png)

add字段后

![avatar](https://raw.githubusercontent.com/chenjie222/elk_filebeat_kafka/master/image/011.png) 

这时候可以在搜索框输入kubernetes.container.name:"aimachine-engine"

这里一定要加上双引号，加上双引号才是精确查询





