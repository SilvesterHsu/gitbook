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

content in `SUMMARY.md`
```
* [README](README.md)
```

content in `README.md`
```
# This is my firt markdown
```

## Git Initialization
Enter `<your project>` folder through the terminal.
```
git init
git add .
git commit -m "Basic gitbook files"
```
## GitHub Tocken
We need `GITHUB_TOKEN` for Travis to build gitbook. So we generate one in [Personal access tokens](https://github.com/settings/tokens).(or you can go `Settings -> Developer settings -> Personal access tokens` to generate one).

![Git-Build-01](/assets/Git-Build-01.jpg)

And make sure click every selection.

![Git-Build-02](/assets/Git-Build-02.png)

Copy the token we generated for later use.
