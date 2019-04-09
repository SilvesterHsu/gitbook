## 概要
* 新建Gitbook文档
* git初始化
* GitHub设置

## 新建Gitbook文档
Find the place where you want to write a book, you can also create a new project folder:
```
mkdir <your project>
```
and then create two essential files `SUMMARY.md` and `README.md`. These two files are used to build html files via gitbook.

>content in`SUMMARY.md`
>```
>* [README](README.md)
>```

>content in`README.md`
>```
># This is my firt markdown
>```

## git初始化
Enter `<your project>` folder through the terminal.
```
git init
git add .
git commit -m "Basic gitbook files"
```
## GitHub设置
