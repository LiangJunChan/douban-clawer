# douban-clawer
## 豆瓣读书爬虫

python3 写的豆瓣图书，可以根据输入的标签爬下豆瓣读书中的书名，平分，作者/译者，出版信息，按照平分排序后保存为 .xlsx 文件。

### 实现内容

- [x] 爬取豆瓣读书标签下所有图书按评分保存到 Excel 中

- [x] 头文件用 User Agent 伪装浏览器
- [x] 加入随机延时模拟用户行为
- [ ] 使用代理 Ip池（免费 ip 不稳定，可选择使用）

### 使用说明

为头文件信息填写你豆瓣账号的 cookies（cookies 信息在浏览器开发者模式下 network 中查看）

```python
header = {
    "User-Agent":
    "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/73.0.3683.86 Safari/537.36",
    'cookie':
    ''
}
```

输入标签。如“编程”就可以愉快地使用了，结果得到 book_list-编程.xlsx如下
![结果](https://raw.githubusercontent.com/LiangJunChan/MarkdownPhoto/master/uPic/结果.png)

