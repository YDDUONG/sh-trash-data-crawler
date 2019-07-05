# 上海垃圾分类数据爬虫

这个脚本用来爬取[上海垃圾分类信息查询网页](http://trash.lhsr.cn/sites/feiguan/trashTypes_2/TrashQuery_h5.aspx)中的数据集。

- 用`get_keywords.py`调用关键词接口，通过单字查询获取关键词列表  
（注意：这个接口的行为已改变，之前对返回的关键词数量未做限制，现在已限制为3个，难以获取完整的关键词列表，可考虑使用已经抓取的列表或者其他语料库）
- 用`get_trash_data.py`调用查询网页，解析返回页面中的垃圾分类信息
- 本repo中提供了已抓取的数据集
