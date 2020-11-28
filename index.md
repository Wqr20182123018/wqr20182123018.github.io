## 王庆瑞
Figure 3 :
Search and Review Files用例图说明：
作者：李元祥，王庆瑞
用例图建模过程分析：
一：根据上述的Search and Review Files中的功能分析，对其进行如下描述 Files Manage中总共有以下的几大用例：
1.	查找文件（Search Files）
2.	阅读文件（Review Files）
3.	模糊查找（Fuzzy Saerch）
4.	精确查找（Exact Search）
5.	下载后查看（Download after Review）
6.	在线查看（Online Review）
其中Search and Review Files中主要有两大参与者：
1.	用户（User）
2.	管理员（Administrator）
二：模型分析
1.	管理员（Administrator）和用户（User）都共同有查找文件（Search Files）和阅读文件（Review Files）
2.	对于查找文件（Search Files），存在精确查找（Exact Search）找和模糊查询（Fuzzy Saerch）的泛化关系；
3.	对于阅读文件（Review Files），存在下载后查看（Download after Review）和在线查看（Online Review）的泛化关系
4.	由于阅读前应该是先查找文件（Search Files）到然后再阅读文件（Review Files），固然存在阅读文件（Review Files）依赖查找文件（Search Files）；

三．	模型建立： 
1.	用户（User）和管理员（Administrator）都共同指向查找文件（Search Files）和阅读文件（Review Files）
2.	阅读文件（Review Files）依赖指向于查找文件（Search Files）；
3.	精确查找（Exact Search）和模糊查询（Fuzzy Saerch）指向泛化于查找文件（Search Files）；
4.	下载后查看（Download after Review）和在线查看（Online Review）指向泛化于阅读文件（Review Files）；
