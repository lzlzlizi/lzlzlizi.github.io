---
title: FirstBlog
date: 2019-07-25 13:06:10
tags: 
    - trivial
    - little tips
mathjax: true
---

A quick guide to remind you how to set up a github page.

<!-- more -->

<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width=330 height=86 src="//music.163.com/outchain/player?type=2&id=29829683&auto=1&height=66"></iframe>

1. 创建仓库 ....io
2. 创建两个分支：master 与 hexo, 设置hexo为默认分支
3. 使用git clone 拷贝仓库
4. 在....io文件夹下通过
   1. npm install hexo
   2. hexo init（要空文件夹，所以先mkdir temp 然后在temp 中执行再 移到io文件夹中）
   3. npm install 
   4. npm install hexo-deployer-git
5. 同步源文件git add .、git commit -m "..."、**git push origin hexo**
6. 生成网页 hexo g -d


## math inline

change the renderer to:
```
npm i hexo-renderer-markdown-it-plus --save
```

## How to setup tf1.14

1. make sure kernel is around 5.01?? (really necessary??)
2. download cuda-toolkit 10.0, and responding cudnn from nvidia website
3. dpkg local deb file
4. add key according to the instruction on the website
5. install cuda-10-0 according to the instruction on the website
6. bingo!
7. F**K TENSORFLOW, pytorch is the right thing to go!!!

