# Less 文本阅读

**参考文档**

[9 Practical Example of Less Command in Linux](https://linuxhandbook.com/less-command/)

[Linux less 命令](https://www.runoob.com/linux/linux-comm-less.html)

---

## 打开与关闭

对于需要阅读的文件只需通过 less 关键词加上文件即可。

```bash
less [option] <filename>
```

less 的好处在于它不是一下加载整个文件，同时是一个只读的阅读器，相比 vim 更加快速也更加安全。

当需要关闭阅读器时，只需要按下 `q` 即可。

&emsp;

## 常见参数选项

`-N`：打开文件后显示行数信息。

`-I`：less 中默认的文本搜索是大小写敏感，加上这个选项可以忽略大小写。

&emsp;

## 常用快捷键

`g` - 跳转到文档第一行，即开始部分。

`G` - 跳转到文档最后一行，即结束部分。

`Up arrow / Down arrow` – 文档向上/下移动一行。

`b` - 向上移动一页。

`Space` - 向下移动一页。

`/pattern` - 向后搜索。先按下 `/`，然后输入想要查找的内容，敲击回车即可返回。如果搜索结果有多个，通过 `n` 可以查找下一个，`N` 查找上一个。

`?pattern` - 向前搜索。先按下 `?`，然后输入想要查找的内容，敲击回车即可返回。如果搜索结果有多个，通过 `n` 可以查找下一个，`N` 查找上一个。

&emsp;

## 文档标记

less 允许阅读者对文件进行标记，只需要通过 `m` 加上一个 字母即可。当后面需要回到标记处时，只需要通过 `'` 加上相同的字母。一个文档可以标注多处地方，只要确保使用的字母不同。

```less
// 标记为 a
ma
// 返回 a 的地方
'a
```
