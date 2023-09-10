---
title: 建站历史
date: {{ date }}
categories: programming
tags:
---

## 建站成功 ##

2023 | 4 | 15

## 加入加密功能 ##

2023 | 4 | 16

## 加入评论功能 ##
2023 | 4 | 17

## 尝试配置RSS ##
2023 | 4 | 17

## 尝试修改主题布局 ##

2023 | 4 | 18

### archive.ejs ###

> < section class="px-6 max-w-prose mx-auto gap-12 grid grid-cols-1" >

定义section元素，使用CSS网格布局(grid)

grid对应一列(column)，最多只能容纳一个子元素（主页面post略缩条），具有指定的类名
px-6,左右内边距(padding)为6px
max-w-prose， 指定内容宽度的类
gap-12 子元素（略缩条）间距12px
mx-auto类：水平居中

### set categories ###
hexo n category pages

在根目录_config.yml修改：
>Category & Tag
default_category: uncategorized
category_map:
    编程: programming
    Hexo：Hexo
    生活: life
    其他: other
tag_map:

（map为分类模板，按照post的categories属性路径分类，前为显示的名称，后为路径）

在scaffolds/post.md修改生成（hexo n ""）post时的模板。加入categories：，使生成的posts初始格式带categories

修改生成的post.md中的categories："写好的分类"
自动关联路径source/写好的分类

### 问题-已解决 ###

左上角logo在托管界面无法正常显示

已解决：把 images/logo.svg路径换为/logo.svg,让它用和favicon一样的图 相对路径错误？（上传到GitHub的文件格式与本地不同）

### 实现多主机部署 ###
2023 | 4 | 19