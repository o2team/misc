# misc

`misc`是aotu.io的静态资源项目，其文件访问网址有下面几个：

- misc.aotu.io/{github用户名}/{文件名}
- o2team.github.io/misc/{github用户名}/{文件名}
- https://cdn.rawgit.com/o2team/misc/gh-pages/{github用户名}/{文件名}


其中,

- `misc.aotu.io`是利用webhook同步到腾讯云的镜像站点，http协议是http2，国内速度最快
- `o2team.github.io/misc`则是github自己的静态服务器，对应`gh-pages`分支
- `rawgit` 则是一个第三方的cdn服务。

> 所有博客、其他项目涉及的静态资源(图片、样式、脚本）从`2016年07月16号`开始请使用`misc`。

## misc的目录组织

`misc`项目以成员`github用户名`为二级目录，方便区分资源所属，举例如下：

```
 misc
    ├── o2   //存放非个人所属的资源
        ├── xxx.png
        ├── xxx.js
        ├── xxx.css
    ├── pfan123 //存放高大师的静态资源
        |-- xxx.svg
        |-- yyy.png
    ├── mamboer //存放LV的静态资源
        |-- aaa.png
        |-- 波多.avi
```

> 为方便大家使用，已为O2所有人创建了对应的目录，请大家上传文件的时候对号入座！
> 请勿创建非github用户名的目录！！！！会影响将来可能发生的自动化构建、迁移、部署等流程！

## 如何上传文件？

有两种办法上传文件，可根据自身习惯选用其一。将来文件多了不方便的时候再做一个页面专门用于上传。

### 方法1 - 利用Github的GUI上传

1. 打开`misc`网页 [https://github.com/o2team/misc](https://github.com/o2team/misc)
2. 找到你github用户名对应的目录
3. 利用`Upload files` 拖拽上传文件

![upload](https://cdn.rawgit.com/o2team/misc/gh-pages/mamboer/Screen%20Shot%202016-07-16%20at%205.14.23%20PM.png)

### 方法2 - 利用Git命令

1. 将`misc`项目签出到本地

```
git clone --depth 1 git@github.com:o2team/misc.git
```

2. 在`misc`项目里找到你github用户名对应的目录

3. 增删改文件，然后利用`git`命令提交即可。

