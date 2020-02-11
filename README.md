# 评注
http://101.camp 's commentes hosting

## 背景

- 101.camp 为首有一系列蟒营™课程网站
- 需要统一的评注入口

## 问题
> 以往使用的 DISQUS 服务已和谐

- 发现 [utterances](https://utteranc.es/)
    + 基于 github-api
    + 利用 Issue 接口
    + 将指定仓库的公开 Issue 变成对应网页的评注入口
    + 优雅/精巧/合理/免费/稳定...


## 应对
https://github.com/101camp/comments

- 创建仓库
- 配置 [utterances](https://utteranc.es/)
- 将所有相关网络模板中的评注入口, 都指向这儿
- [Issues · 101camp/comments](https://github.com/101camp/comments/issues) 

## 以及
> 功能如此完备的一个仓库, 只使用 Issue 是不科学的

基于 MkDocs 改造的一系列网站

- 因为, 并没被 github 官方支内置构建
- 所以, 只能自行完成自动化构建
- 最简洁的方案:
    + 在公网主机中
    + 部署自动化构建环境
    + 通过 crontab 定期检验是否有`触发物`
        * 有, 就构建并发布
        * 冇, 就略过
- 自动过程,总是会有一些意外发生
- 但是, 自己不一定在合理的环境中, 能随时查看编译/发布过程
- 那么, 如果将自动发布过程的日志, 收集到一个仓库中
    + 不就可以随时通过网页来查询详细过程了?
- 当前仓库就是一个天然的容器
    + 只是, 每个具体网站的编译过程没什么关联
    + 所以, 自然想到分离的 orphan 分支


当前针对性收集的编译日志索引:

    /
    +- dlog101camp    <- 101.camp
    +- dlog_py101camp <- py.101.camp
    +- dlog_tm101camp <- tm.101.camp
    ...



## logging

- 200211 ZQ 增补 dlog_tm101camp
- 200201 ZQ 追加捐助入口
- 181208 ZQ init.
