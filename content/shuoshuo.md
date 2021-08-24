---
title: "说说"
date: 2021-08-23
slug: shuoshuo
draft: false
comment: false
--- 
<div id='speak'></speak>
<script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ispeak-bber/ispeak-bber.min.js" charset="utf-8" ></script>
<script>
ispeakBber
    .init({
      el: '#speak', // 容器选择器
      name: 'Cat Tom', // 显示的昵称
      envId: 'blog-bb-6gvuymj7b6dae24e', // 环境id
      region: 'ap-shanghai', // 腾讯云地址，默认为上海
      limit: 10, // 每次加载的条数，默认为5
      avatar: 'https://static.cattom.site/image/icon/32.png?x-oss-process=style/webp',
      fromColor:'rgb(245, 150, 170)', // 下方标签背景颜色 默认 rgb(245, 150, 170)
      loadingImg: 'https://7.dusays.com/2021/03/04/d2d5e983e2961.gif', // 自定义loading的图片，示例值为默认值
      dbName:'talks' // 数据的名称，默认talks，避免有人的命名不是这个，所以加入此配置字段。
    })
    .then(function() {
      // 哔哔加载完成后的回调函数，你可以写你自己的功能
      console.log('哔哔 加载完成')
    })
</script>
