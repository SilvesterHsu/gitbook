## Introduction
Gitbook is great for writing books, however, if you want to share it with others, you need a server and a domain name. This undoubtedly requires the cost of money. We can use GitHub Pages to solve this.

GitHub provides [GitHub Pages](https://pages.github.com/) services for all repositories. And since Gitbook almost stops open source maintenance, I don't want to install it on my mac. I tried to install Gitbook via [Docker](https://hub.docker.com/r/fellah/gitbook), but Docker consumes too much resources (about 1.5G of RAM) and I don't want to make writing so complicated. So I will compile my markdown file to a static web page file via [Travis](https://travis-ci.org) through an automatic compilation method.

**Example**
![Readme-01](/assets/Readme-01.jpg)
