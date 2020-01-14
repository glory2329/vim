### vim 撤销 回退操作:
    在vi中按u可以撤销一次操作
    u 撤销上一步的操作 Ctrl+r 恢复上一步被撤销的操作

#### 注意
    如果你输入“u”两次，你的文本恢复原样，那应该是你的Vim被配置在Vi兼容模式了。
    如果你撤销得太多，你可以输入CTRL-R（redo）回退前一个命令。
    换句话说，它撤销一个撤销。
    要看执行的例子，输入CTRL-R两次。字符A和它后面的空格就出现了：
    young intelligent turtle 有一个特殊版本的撤销命令：“U”（行撤销）。
    行撤销命令撤销所有在前一个编辑行 上的操作。 
    输入这些命令两次取消前一个“U”： 
    A very intelligent turtle xxxx 删除very
    A intelligent turtle xxxxxx 删除turtle
    A intelligent 用“U”恢复行
    A very intelligent turtle 用“u”撤销“U”
    A intelligent “U”命令自己改变自己，“u”命令撤销操作，CTRL-R命令重做操作。
    这有点乱，但不用 担心，用“u”和CTRL-R命令你可以切换到任何状态。
    流行的文本编辑器通常都有前进和后退功能，可以在文件中曾经浏览过的位置之间来回移动。
    在 vim 中使用 Ctrl-O 执行后退，使用 Ctrl-I 执行前进。
    相关帮助： :help CTRL-O :help CTRL-I :help jump-motions

# react项目-硅谷直聘的运行说明
## 1. 准备
	1) 确保安装了node环境
		查看是否已经安装: node -v
		如果没有安装: 可以根据尚硅谷node课程视频去操作: http://www.atguigu.com/html5_video.shtml#nodejs

	2) 确保安装了mongodb, 并启动了对应的服务
		查看是否安装并启动了服务: 右键-->任务管理器-->服务-->MongoDB
		如果没有安装: 可以根据尚硅谷mongodb课程视频教程操作: http://www.atguigu.com/html5_video.shtml#nodejs
	
## 2. 启动后台应用
	1). 进入gshop-server_final
	2). 执行命令: npm start

## 3. 启动前台应用并访问
	1). 进入gshop-client_final
	2). 执行命令: npm start


