## **everything**——一个搜索文件的软件

下载方式：

- 官网下载

- 利用winget下载

​	按下键盘上的win+R键，输入cmd打开命令提示符，然后输入下面这行命令并回车来确认一下：

```bash
winget --version
```

如果看到了版本号，那就继续

==先搜索，再安装==

```bash
winget search everything
```

执行命令后，你会看到一个表格，里面列出了匹配的软件。找到你想要的软件，记下它的 **ID** 那一列的内容。之后安装就OK了

```bash
winget install --id voidtools.Everything
```

### winget命令

| 用途               | 命令                             |
| ------------------ | -------------------------------- |
| **列出已装软件**   | ` winget list`                   |
| **查看可更新软件** | `winget upgrade`                 |
| **更新所有软件**   | `winget upgrade --all`           |
| **卸载软件**       | `winget uninstall --id <软件ID>` |

> 如果你打算在新电脑上批量安装软件，`winget` 还能通过 `winget export` 和 `winget import` 命令，一键还原你的软件列表，非常方便