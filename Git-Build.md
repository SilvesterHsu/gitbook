## Outline
* Gitbook essential document
* git initialization
* GitHub tocken

## Gitbook Essential Document
There are two essential files `SUMMARY.md` and `README.md` to build gitbook project. We need to create these files before build.

Find the place where you want to write a book, you can also create a new project folder:
```
mkdir <your project>
```
and then create files `SUMMARY.md` and `README.md`.

>content in `SUMMARY.md`
>```
>* [README](README.md)
>```

>content in `README.md`
>```
># This is my firt markdown
>```

## Git Initialization
Enter `<your project>` folder through the terminal.
```
git init
git add .
git commit -m "Basic gitbook files"
```
## GitHub Tocken
We need `GITHUB_TOKEN` for Travis to build gitbook. So we generate one in [Personal access tokens](https://github.com/settings/tokens).(or you can go `Settings -> Developer settings -> Personal access tokens` to generate one).

![Jietu20190409-223830](/assets/Jietu20190409-223830.jpg)

And make sure click every selection.

![FireShot Capture 018 - Edit personal access token - github.com](/assets/FireShot%20Capture%20018%20-%20Edit%20personal%20access%20token%20-%20github.com.png)

Copy the token we generated for later use.
