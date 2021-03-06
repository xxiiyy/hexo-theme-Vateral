## hexo-theme-Vateral

hexo主题 vateral 灵感来自material

示例网站：[某猫のBlog](https://www.moumaobuchiyu.com)

## 如何使用该主题

### 下载

首先下载主题，解压好后放到themes目录

### 使用

修改主题文件夹名称，将其改为 Vateral

### 配置

找到主题里的_config.yml文件

favicon：设置icon图标

headbg：设置左侧抽屉中头像部分的背景图

header：设置头像

post_header：设置首页的标语部分 img：标语背景图 about：标语 url：为标语添加一个链接

sns：添加社交账号链接，没有默认不填

sidebar：导航栏配置，如果需要某项，use为ture，反之为false

*注：about friends photo要在hexo的文章目录下单独创建配置文件 

about页面：

在 hexo 目录下的 source 文件夹内创建一个名为about的文件夹。

然后在文件内创建一个名为 index.md 的 Markdown 文件。

然后编辑里边的index.md文件

friends页面：

在 hexo 目录下的 source 文件夹内创建一个名为friends的文件夹。

然后在文件内创建一个名为 index.md 的 Markdown 文件。

在 index.md 文件内写入如下内容即可。
```
---
title: links
date:
layout: links
---
```
然后添加friends页面的数据

同样在在 hexo 目录下的 source 文件夹内创建一个名为 _data 的文件夹。

然后在文件内创建一个名为 friends.yml 的文件。

单个友情链接的格式为：
```
name:
    link: 此处为站点链接
    descr: "介绍"
```

如果想要添加多个友情链接，重复填写即可

photo界面：

在 hexo 目录下的 source 文件夹内创建一个名为 photo的文件夹。

然后在文件内创建一个名为 index.md 的 Markdown 文件。

在 index.md 文件内写入如下内容即可。
```
---
title: photo
date:
layout: photo
---
```
然后添加photo页面的数据    

同样在在 hexo 目录下的 source 文件夹内创建一个名为 _data（禁止改名）的文件夹。

然后在文件内创建一个名为 photo.yml 的文件。

单个图片的格式为：

```
name:
    large_link: /images/photo/1-large.jpg
    small_link: /images/photo/1-small.jpg
    alt: "image 1"
    descr: "简介"
```

*注：alt属性要对每照片编号

如果想要添加多个图片，重复填写即可

reading：设置自动生成摘要的字数

photo:设置photo界面属性 ，name：相册名称 ，about：相册介绍

### 本地搜索

使用本地搜索需要在hexo目录安装 hexo-generator-search 插件。

然后在 站点配置 文件中添加
```
search:
	path: search.xml
	field: all
```
至此配置基本结束
