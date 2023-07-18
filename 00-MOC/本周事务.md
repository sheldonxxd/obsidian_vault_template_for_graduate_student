### Doing

```dataview
TABLE file.cday AS Start
FROM "01-Diary/本周事务"
WHERE date > date(today) - dur(1 year) AND status = "doing"
SORT rating desc
```


### Done

```dataview
TABLE excerpt AS Comment
FROM "01-Diary/本周事务"
WHERE date > date(today) - dur(1 year) AND status = "done"
SORT rating desc
```

上表仅列出存放于`01-Diary/本周事务`的事务记录文件，建议每周小结时清理一次，根据内容分类到其它目录中去。每周结束后该表可截图粘贴至周小结中，方便汇总分析。若事务持续超过一年则自动排除。

### Cancel

```dataview
TABLE excerpt AS Comment
FROM "01-Diary/本周事务"
WHERE date > date(today) - dur(1 year) AND status = "cancel"
SORT rating desc
```
