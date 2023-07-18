---
date: 2023-07-18 14:55:04
status: done
tags: obsidian入门
rating: ⭐⭐
---

### 模板库目录结构说明

- 00-MOC：内容地图，主要存放dataview查询表和obsidian白板
- 01-Diary：存放模板化的每日日志和每周小结，其中每周事务是新建笔记默认存放地
- 02-Reading：存放文献库和文献阅读笔记
- 03-Projects：按各种实际的项目分类存储相关笔记
- 06-Cards: 主要存放一些卡片
- 07-Archives：时间久远而且已经结束的project可以进行存档
- 08-Assets：存放附件，包括插图、视频、以及各种其它文件
- 09-Templates： 存放笔记模板

### zotero 设置

![[Pasted image 20220322201722.png]]

打开 zotero 之后，点击菜单栏的 「编辑」，然后选择「首选项」，进入到 zotero 的设置当中。如上图所示，需要对箭头所示的地方做修改。

特别需要注意的是「高级」中的`链接附件根目录` 和 `数据存储位置` 的路径设置。前者必须是 vault 库中存放 pdf 的子目录。

本教程 vault 根目录为 `X:\projects\working`，而`/08-Assets/pdfs`是存在于该 vault 中的子目录，专门保存文献条目的 pdf 附件。而 mdnote 文件存放于 `02-Reading/mdnotes`，所以zotero中的根目录可以设置与 vault 根目录相同（👆**图中有误**）

数据存储位置您可以选择默认（如果C盘够大）或者指定一个其它不在 vault 中的目录。

### zotfile插件安装和设置


![[Pasted image 20220321154948.png]]

zotfile 是 zotero 中最强大的插件，点击 zotero 菜单栏的「工具」> 「插件」，可以进入插件管理器，然后点开齿轮，选择从文件安装插件。插件为`.xpi`后缀的文件，在[[软件下载安装]]中已经提及。后面的 mdnotes 和 better bibtex 插件的安装同此操作。

![[Pasted image 20220322201929.png]]

然后对 zotfile 插件进行设置。点击 zotero 菜单栏的「工具」就能看到 zotfile 的插件设置选项。如上图所示，对箭头所指内容进行修改。

注意**将 pdf下载的临时目录设置为桌面**，以后可以从网上直接下载 pdf 到桌面，再选择pdf对应的文献条目，右键单击后选择`Attach New File`，调用该插件可以自动把 pdf 重命名并转移到**指定目录**（`\08-Assets\pdf`)去，并且创建指向 pdf 的链接。建议勾选下方 `Use subfolder` ，如果是windows系统的话还要把`\` 修改为 `/`。

### mdnotes 插件安装与设置

![[Pasted image 20220322202038.png]]

同 zotfile 的安装方式，其设置选项也在zotero 菜单栏的「工具」中可见，点开后如上图所示做修改，尤其要注意路径的设置。注意 mdnotes 导出目录为 `02-Reading/mdnotes`，而 mdnotes 的模板存放于 `08-Assets/Scripts` 中。

### better bibtex 插件安装与设置

![[Pasted image 20220321155719.png]]

插件安装同 zotfile，但是其设置选项已经被整合到 zotero 首选项中了（说明是个更加高级的大插件）。在这个地方，我们需要修改 citation key 的格式，如上图所示：就作者加年份即可。

此外，还需要修改 Export > Quick-Copy 中的格式为 Roam Cite Key。这样当你使用快捷键 `Ctrl+Shift+C` 从 zotero 中拷贝文献，就会拷贝一个 Roam Cite Key 格式的内容出来。

![[Pasted image 20220321160208.png]]

然后再到「导出」选项中修改 zotero 的便捷复制，选择 Better BibTex Quick Copy: Roam Cite Key，就大功告成了。

如某篇文献的 citation key 是 `xxd2022`，那么对应的 Roam Cite Key 就是 `[[@xxd2022]]`，然后你把这个 Roam Cite Key 直接粘贴到 obsidian 中就完成了引文的插入，非常便捷。
