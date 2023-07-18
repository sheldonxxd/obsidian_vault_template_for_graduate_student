---
date: 2023-07-18 14:12:37
rating: ⭐
status: inprogress
excerpt: 为啥要做？做完后有何收获感想体会？
tags: 
alias: 
---

### 文献入库

1. 在zotero中通过doi号新建文献条目。
	![[Pasted image 20230718142134.png]]
2. 下载原文pdf文件到桌面（或用户在 ZotFile 插件设置的自定义路径），再右键点击该文献条目 Attach New File
	![[Pasted image 20230718142425.png]]
3. 为该文献条目设置固定的 citation key
	![[Pasted image 20230718142536.png]]
4. 生成 mdnotes 文件，注意这个文件仅需生成一次，否则会因为按空白模板刷新文件内容导致过去的阅读批注丢失。
	![[Pasted image 20230718142707.png]]


### 文献泛读

通过 zotero 在obsidian库的 `02-Reading/mdnotes` 目录中生成的 mdnotes 文件页面打开显示如下：

![[Pasted image 20230718143810.png]]

您需要立刻做的事情包括：

1. 将 tags 的 unread 修改为该文献最重要的关键词
2. 在 annotation-target 中填写文献正文 pdf 文件名，这个可以从下方的 PDF Attachments 中拷贝，以激活 annotator 插件。
3. 在某个阅读主题下的obsidian白板中为这个文献条目制作一张卡片：
	![[Pasted image 20230718143955.png]]基于对文献标题，摘要的阅读，以及对文章figure的快速过目，用一句简单的话概括此文工作，插入指向该文献mdnote文件的双链，并且贴上一张代表性的图。然后和比较相关的其他文献卡片放得靠近一点或者连线。

### 文献精读

文献精读通过 annotator 插件完成。如下图所示：

![[Pasted image 20230718144535.png]]

回到 mdnote 页面，确认 annotation-target 的值填写无误，页面右上角三点面板中可以看到  Annotate 选项。点击即可进入到阅读批注界面。

![[Pasted image 20230718144649.png]]

后面可以在任意指向该 mdnote 的双链处悬停预览查看批注情况：

![[Pasted image 20230718144911.png]]

