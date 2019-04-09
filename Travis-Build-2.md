## 概要
* 编辑构建脚本
* GitHub上传
* Travis构建

## 编辑构建脚本
Enter `<your project>` folder through the terminal, and generate travis setting file：
```
cd <your project PATH>
nano .travis.yml
```
```
language: node_js

node_js:
  - "8"

cache:
  directories:
    - $HOME/.npm

before_install:
  - export TZ='Asia/Shanghai'

install:
  - npm install gitbook-cli -g
  - gitbook install

script:
  - gitbook build . ./build

branches:
  only:
    - master

deploy:
  provider: pages
  skip_cleanup: true
  github_token: $GITHUB_TOKEN
  local_dir: build
  name: $GIT_NAME
  email: $GIT_EMAIL
  on:
    branch: master
```

## GitHub上传
After generating the travis setting file, we need to push it on GitHub.
```
git add .travis.yml
git commit -m "Travis setting file"
git push
```

## Travis构建
Enter our repository in [Travis](https://travis-ci.org/) and build our repository.
It will use our setting file `.travis.yml` to build the gitbook website.
If everything goes well, it should be in green.
![Jietu20190409-153645](/assets/Jietu20190409-153645.jpg)
