---
title: "说说"
date: 2021-08-23
slug: shuoshuo
draft: false
comment: false
--- 
{% note success %}
说说内容来自
{% endnote %}
<div id="tip" style="text-align:center;">ipseak加载中</div>
<div id="ispeak"></div>
<link
  rel="stylesheet"
  href="https://cdn.staticfile.org/highlight.js/10.6.0/styles/atom-one-dark.min.css"
/>
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/npm/ispeak@4.3.2/style.css"
/>

<style>
  #article-container .D-avatar {
    margin: 0 10px 0 0;
  }
  .D-footer {
    display: none;
  }
</style>
<script src="https://cdn.staticfile.org/highlight.js/10.6.0/highlight.min.js"></script>
<script src="https://cdn.staticfile.org/marked/2.0.0/marked.min.js"></script>
<script src="https://cdn1.tianli0.top/npm/discuss@0.2.2/dist/Discuss.js"></script>
<script src="https://cdn1.tianli0.top/npm/ispeak@4.3.2/ispeak.umd.js"></script>
<script>
  var head = document.getElementsByTagName('head')[0]
  var meta = document.createElement('meta')
  meta.name = 'referrer'
  meta.content = 'no-referrer'
  head.appendChild(meta)
  if (ispeak) {
    ispeak
      .init({
        el: '#ispeak',
        api: 'https://kkapi-open-psi.vercel.app/',
        author: '63ac6c02b2c15691e80ef38b',
        pageSize: 10,
        loading_img: 'https://czrui99.oss-cn-chengdu.aliyuncs.com/loading.gif',
        initCommentName: 'Discuss',
        initCommentOptions: {
          serverURLs: 'https://kkdiscuss.vercel.app/'
        }
      })
      .then(function () {
        console.log('ispeak 加载完成')
        document.getElementById('tip').style.display = 'none'
      })
  } else {
    document.getElementById('tip').innerHTML = 'ipseak依赖加载失败！'
  }
</script>