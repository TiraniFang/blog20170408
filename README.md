# blog20170408
# 我的博客

## 制作过程

1：新建一个仓库 repository
2：新建一个index.tml

## 如何预览

点击setting下的网址，之前得把source的none改成markdown

## 如何将markdown变成html

1：搜索marked开源库   chjj/marked
2: 百度搜索 marked cdn js    复制链接 https://cdn.bootcss.com/marked/0.3.6/marked.js
3: 在页面引入这个js，再参考   chjj/marked的browser 使用 
    创建一个id为content的div，在插入一个script，内容为：
    <script>
    var markdown=`
    # Marked in browser
    ## Rendered by **marked**.
    [百度](www.baidu.com)  `
    var html=marked(markdown)
     document.getElementById('content').innerHTML =html;
     
    </script>
 4:添加简单的样式  搜索 typo.css
 5：也可创建一个css文件，然后在index里面引入


## 如何自己生成页面

1：下载nodeJs
