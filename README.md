# zoterosearch

## 中文说明

具体可见少数派文章：https://sspai.com/post/72459

本文件是一个是Launchbar的Action，主要作用是通过Zotero制作一个可供Launchbar的json文件，实在在Launchbar中搜索和打开Zotero中的文献和附件，

### 使用前需要完成以下准备工作：

1.在 Zotero 安装 Better BibTeX 插件，安装好 Better BibTeX 后并重启 Zotero，在 Zotero的 File->Export Library... 所弹出的界面中选择 BetterBibTex JSON ，找到此 json 文件，并复制路径，并将 Keep updated 的勾打上，以便 Zotero 更新时自动更新 JSON 文件。

2.下载Zotero Refresh.lbaction和Zotero Search.lbaction，双击安装。之后在 Launchbar 的 Action Editor 中找到 Zotero Refresh.lbaction ，点击其中的 Edit
键，将代码中的zotJson变量的 json 路径更改为以上的路径；并设定 File.writeJSON 下的 json 路径，以供下一步使用。

3.在 Launchbar 的 Action Editor 中找到 Zotero Search.lbaction，同样地打开代码界面，将变量 zoteroJson 的路径更改为上一步的路径。

4.在 Zotero 的数据库更新时可以运行一遍 Zotero Refresh.lbaction。

5.需要搜索 Zotero 中文献时，运用 Zotero Search.lbaction，然后输入标题字符可以检索出需要的文献。

### 本Action尚存在问题

1.所有文献均需要有 title，无 title 则无法生成正常 json 文件，运行Zotero Search.lbaction时将报错。

2.不能有不依附于文献的笔记，否则结果同上。


## English description 

see minority articles for details: https://sspai.com/post/72459 

this document is an action of LaunchBar. Its main function is to make a JSON file available for LaunchBar through Zotero. It is necessary to search and open the documents and attachments in Zotero in LaunchBar.

#### use the following preparations: 
1.Install the better BibTex plug-in in Zotero. After installing better BibTex, restart Zotero. In file - > export Library of Zotero Select betterbibtex JSON in the pop-up interface, find the JSON file, copy the path, and tick keep updated to automatically update the JSON file when Zotero updates. 

2.Download Zotero refresh Lbaction and Zotero search Lbaction, double-click install. Then find Zotero refresh in the action editor of LaunchBar Lbaction, click the edit key to change the JSON path of the zotjson variable in the code to the above path; And set file The JSON path under writejson for the next step. 

3. Find Zotero search in the action editor of LaunchBar Lbaction, similarly open the code interface and change the path of the variable zoterojson to the path of the previous step. 

4. Zotero refresh can be run once when Zotero's database is updated lbaction.

5. When you need to search Zotero Chinese offers, use Zotero search Lbaction, and then enter the title character to retrieve the required literature. 


## there are still problems in this action 

1.All documents need a title. Without a title, normal JSON files cannot be generated. Run Zotero search Lbaction will report an error. 

2. There must be no notes that are not attached to the literature, otherwise the result is the same as above.
