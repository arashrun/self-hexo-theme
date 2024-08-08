## Hexo 主题 Tree

Fork from：[https://wujun234.github.io/](https://wujun234.github.io/)

hexo 主题使用 ejs 的方式作为模板引擎

## TODOLIST:

-   [x] 关灯
-   [x] 友链内容扩展
-   [x] post 导航目录

[可以参考改 blog](https://siricee.github.io/hexo-theme-Chic/)

## Bugs：

2. toc 内有空格标题无法跳转

-   search 页面需要二次刷新才能搜索 (pjax 导致 js 使用的缓存)
-   about 页面的 footer 组件不能正常删除 (pjax）
-   tags 和 categories 页面点击链接无效

#### 不安装 hexo 的调试方法

1. 直接访问在线博客
2. 通过浏览器内置的 override 替换功能，替换本地的 js 或 css 文件，达到了效果之后直接提交即可
