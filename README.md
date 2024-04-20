

![](https://raw.githubusercontent.com/lingyun0406/lingyun0406.github.io/master/img/readme-home.jpg)

[![Build Status](https://travis-ci.org/lingyun0406/lingyun0406.github.io.svg?branch=master)](https://travis-ci.org/lingyun0406/lingyun0406.github.io)
[![codebeat badge](https://codebeat.co/badges/5f031df3-f6c1-4ec0-911a-ff6617ca50b9)](https://codebeat.co/projects/github-com-lingyun0406-lingyun0406-github-io-master)
[![GitHub issues](https://img.shields.io/github/issues/lingyun0406/lingyun0406.github.io.svg?style=flat)](https://github.com/lingyun0406/lingyun0406.github.io/issues)
[![License MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/home-assistant/home-assistant-iOS/blob/master/LICENSE)
[![](https://img.shields.io/github/stars/lingyun0406/lingyun0406.github.io.svg?style=social&label=Star)](https://github.com/lingyun0406/lingyun0406.github.io)
[![](https://img.shields.io/github/forks/lingyun0406/lingyun0406.github.io.svg?style=social&label=Fork)](https://github.com/lingyun0406/lingyun0406.github.io)


���͵Ĵ�̳��޸��� [Hux](https://github.com/Huxpro/huxpro.github.io) 
 
��Ϊ��ϸ�Ľ̴̳��� [������ GitHub Pages ���ٴ���˲��͡�](http://www.jianshu.com/p/e68fba58f75c) �� [wiki](https://github.com/lingyun0406/lingyun0406.github.io/wiki/%E5%8D%9A%E5%AE%A2%E6%90%AD%E5%BB%BA%E8%AF%A6%E7%BB%86%E6%95%99%E7%A8%8B)

>
### [�鿴���ʹ����� ](http://lingyun0406.github.io)



## ʹ��

* ��ʼ
	* [����](#����)
	* [��ʼ](#��ʼ)
	* [׫д����](#׫д����)
* ���
	* [�����](#�����)
	* [���������](#mini-about-me)
	* [�Ƽ���ǩ](#featured-tags)
	* [��������](#friends)
	* [HTML5 ��ʾ�ĵ�����](#keynote-layout)
* ������ Google/Baidu Analytics
	* [����](#comment)
	* [��վ����](#analytics) 
* �߼�����
	* [�Զ���](#customization)
	* [�����ͼ](#header-image)
	* [����չʾ����-ͷ�ļ�](#seo-title)



### ����

����㰲װ�� [jekyll](http://jekyllcn.com/)������ֻ��Ҫ������������`jekyll serve` �� `jekyll s`�����ڱ��������������`http://127.0.0.1:4000/`Ԥ�����⣬��������޸�Ҳ��ʵʱչʾ����Ҫǿˢ���������



### ��ʼ

�����ͨ���޸� `_config.yml`�ļ������ɵĿ�ʼ��Լ��Ĳ���:

```
# Site settings
title: BY Blog                    # ��Ĳ�����վ����
SEOTitle: ��ӫ�Ĳ��� | BY Blog		# SEO ����
description: "Hey"	   	   # ���˵�㣬����һ��

# SNS settings      
github_username: lingyun0406     # ���github�˺�
jianshu_username: e71990ada2fd  # ��ļ���ID��

# Build settings
# paginate: 10              # һҳ��׼���ż�ƪ����
```

Jekyll�ٷ���վ���кܶ�Ĳ������Ե��������������µ�������ʽ...��ַ�����[Jekyll - Official Site](http://jekyllrb.com/) ���İ�������[Jekyll����](http://jekyllcn.com/).

### ׫д����

Ҫ���������һ���� **Markdown** �ĸ�ʽ��������`_posts/`����ֻҪ������ƪģ�������������������׸�������á�

yaml ͷ�ļ�������:

```
---
layout:     post
title:      ��ʱ�� ����Ļ�ʹ����
subtitle:   iOS��ʱ�����
date:       2016-12-13
author:     BY
header-img: img/post-bg-ios9-web.jpg
catalog: 	 true
tags:
    - iOS
    - ��ʱ��
---

```

### �����

���ұ�:
![](https://raw.githubusercontent.com/lingyun0406/lingyun0406.github.io/master/img/readme-side.jpg)

�������� `_config.yml`�ļ������`Sidebar settings`�ǿ顣

```
# Sidebar settings
sidebar: true  #��Ӳ����
sidebar-about-description: "�򵥵�����һ�����Լ�"
sidebar-avatar: /img/avatar-by.jpg     #��Ĵ�ͷ������ʹ�þ��Ե�ַ.ע�⣺�������ִ�Сд����׺��Ҳ��
```

���������Ӧʽ���ֵģ�����Ļ�ߴ�С��992px��ʱ�򣬲�����ͻ��ƶ����ײ����������bootstrapդ��ϵͳ <http://v3.bootcss.com/css/>


### Mini About Me

Mini-About-Me ���ģ�齫�����ͷ�����棬չʾ�����е��罻�˺š����Ҳ����Ӧʽ���֣�����Ļ��Сʱ�򣬻Ὣ���ƶ���ҳ��ײ���ֻ��������΢�е�С�仯�������뿴���롣

### Featured Tags

���������վ [Medium](http://medium.com) ���Ƽ���ǩ�ǳ����ſᣬ�����ҽ������˽�����
���ģ�������Ƕ����ģ����Գ���������ҳ�棬������ҳ�ͷ����ÿһƪ���±����ͷ�ϡ�

```
# Featured Tags
featured-tags: true  
featured-condition-size: 1     # A tag will be featured if the size of it is more than this condition value
```

Ψһ��Ҫע�����`featured-condition-size`: ���һ����ǩ�� SIZE��Ҳ����ʹ�øñ�ǩ�����������������趨������ֵ�������ǩ�ͻ�����ҳ�ϱ��Ƽ���
 
�ڲ���һ������ģ�� `{% if tag[1].size > {{site.featured-condition-size}} %}` ��������ɸѡ���˵�.

### Social-media Account

������������罻�˺ţ�û�е���ӵĲ�����ʾ�ڲ�߿��С��¼�����[����](https:/www.jianshu.com)����, <http://www.jianshu.com/u/e71990ada2fd>

	# SNS settings
	RSS: false
	jianshu_username: 	jianshu_id 
	zhihu_username:     username
	facebook_username:  username
	github_username:    username
	# weibo_username:   username
	
	

![](http://ww4.sinaimg.cn/large/006tKfTcgy1fgrgbgf77aj308i02v748.jpg)

### Friends

�������Ӳ��֡������ȫ��ҳ����ʾ��

�������� `_config.yml`�ļ������`Friends`�ǿ飬�Լ��Ӱɡ�

```
# Friends
friends: [
    {
        title: "BY Blog",
        href: "https://lingyun0406.github.io/"
    },
    {
        title: "Apple",
        href: "https://apple.com/"
    }
]
```


### Keynote Layout

HTML5�õ�Ƭ���Ű棺

![](https://camo.githubusercontent.com/f30347a118171820b46befdf77e7b7c53a5641a9/687474703a2f2f6875616e677875616e2e6d652f696d672f626c6f672d6b65796e6f74652e6a7067)

�ⲿ��������ռ��html��ʽ�Ļõ�Ƭ�ģ�һ���õ����� Reveal.js, Impress.js, Slides, Prezi �ȵ�.����Ϊһ���ִ����Ĳ�����ô�����˷�html�õƵĹ�����~

����Ҫԭ�������һ�� `iframe`������������ⲿ���ӡ������ֱ��д��ͷ�ļ�����ȥ��������������yamlͷ�ļ���д����

```
---
layout:     keynote
iframe:     "http://huangxuan.me/js-module-7day/"
---
```

iframe�ڲ�ͬ���豸�У������Զ��ĵ�����С�������ڱ߾���Ϊ�����ֻ��û��������»������Լ���Ӹ�������ݡ�


### Comment

���Ͳ���֧�� [Disqus](http://disqus.com) ����ϵͳ,�������� [Gitalk](https://gitalk.github.io/) ����ϵͳ��[֧�� Markdwon �﷨](https://guides.github.com/features/mastering-markdown/)��cool~

#### Disqus

�ŵ㣺���ʱȽ����У�����Ҳ�ܴ�������࣬����������ۣ�����ʵʱ֪ͨ��ֱ�ӻظ�֪ͨ���ʼ������ˣ�

ȱ�㣺���۱���Ҫȥע��һ��disqus�˺ţ�����һ��ֻ��Facebook��Twitter��������ǽ�ڼ����ٶ�������һ�㡣��Ҫ֪����ɶ�������Կ���ǰ�İ汾��[����](http://brucezhaor.github.io/about.html) ������Ϳ��Կ�����

> Node���кܶ��˷�ӳ Disqus ������ز�����������ǽ�ּܸ��ˣ��������Ļ�����ǽ�ͺ���~

**ʹ�ã�**

**����**������Ҫȥע��һ��Disqus�ʺš�**��Ҫֱ��ʹ���ҵİ���**

**���**����ֻ��Ҫ������� yaml ͷ�ļ�������һ�¾Ϳ����ˡ�

```
# ����ϵͳ
# Disqus��https://disqus.com/��
disqus_username: lingyun0406
```

#### Gitalk

�ŵ㣺����ɾ���࣬���� Github issue API �������۲����ʹ�� Github �ʺŽ��е�¼�����ۣ���ϲ����֧�� Markdown �﷨�����ڳ���Ա��˵����̫ cool �ˡ�

ȱ�㣺���ñȽϷ�����ÿƪ���µ����۶���Ҫ��ʼ����

**ʹ�ã�**

�ο��ҵ���ƪ���£�[��Ϊ������� Gitalk ���۲����](http://lingyun0406.top/2017/12/19/%E4%B8%BA%E5%8D%9A%E5%AE%A2%E6%B7%BB%E5%8A%A0-Gitalk-%E8%AF%84%E8%AE%BA%E6%8F%92%E4%BB%B6/)


### Analytics

��վ����������֧�ְٶ�ͳ�ƺ�Google Analytics����Ҫȥ�ٷ���վע��һ�£�Ȼ�󽫷��ص�code�������棺

```
# Baidu Analytics
ba_track_id: 4cc1f2d8f3067386cc5cdb626a202900

# Google Analytics
ga_track_id: 'UA-49627206-1'            # ����Google�˺�ȥע��һ���ͻ����һ��������id
ga_domain: huangxuan.me			# Ĭ�ϵ��� auto, ���������Զ����˵������������û���Լ�����������Ҫ�ĳ�auto��
```

### Customization

�����ϲ�����ڣ������ȥ�Զ������ģ��� Code��

**����������� `_include/` �� `_layouts/`�ļ����µĴ��루�������������沼�ֵĵط�������Ϳ���ʹ�� Jekyll ʹ�õ�ģ������ [Liquid](https://github.com/Shopify/liquid/wiki)���﷨ֱ���޸�/��Ӵ��룬�����и��д�����Զ����������**

### Header Image

����ÿҳ�ı����ͼ�ǿ����Լ�ѡ�ģ�������ƪʾ��post���֪����������ˡ�
  
�����ͼ��ѡȡ��ȫ�ǿ����˵������ˡ�ÿһƪ���¿����в�ͬ�ĵ�ͼ�������ʲô�ͷ�ʲô�������Ҫ������С��Ҫ̫�󣬷������������

> �ϴ���ͼƬ�����ѹ���������Ƽ� imageOptim ͼƬѹ�����������Ĳ�����ɡ�

������Ҫע����Ǳ�ģ��ı�����**��ɫ**�ģ����Ա���ɫҪ����Ϊ**��ɫ**����**��ɫ**����֮��ɫϵ�Ͷ��ˡ���Ȼ�㻹�����Զ����޸�������ɫ����֮����github pages���ǿ�����ȫ�ĸ��Զ����Լ��Ĳ��͡�

### SEO Title

�ҵĲ��ͱ����� **��BY Blog��** ��������Ҫ��������ʱ����ʾ **����ӫ�Ĳ��� | BY Blog��** ���������Ҫ SEO Title �������ˡ�

��ʵ��� SEO Title ���Ƕ�����<head><title>����</title></head>�������Ķ����Ͷ�˵����ı��⣬����������޸ĵġ�

### �����յ�"Page Build Warning"�� Email

����jekyll������3.0.x,��ԭ���� pygments �����������֧�֣���ֻ֧��һ��-rouge����������Ҫ�� `_config.yml`�ļ����޸�`highlighter: rouge`.���⻹��Ҫ��`_config.yml`�ļ��м���`gems: [jekyll-paginate]`.

ͬʱ,����Ҫ������ı��� jekyll ����.

ʹ��`jekyll server`��ͬѧ��Ҫ������

1. `gem update jekyll` # ����jekyll
2. `gem update github-pages` #���������İ�

ʹ��`bundle exec jekyll server`��ͬѧ�ڸ��� jekyll ����Ҫ����`bundle update`�����������İ�.

> Note��
> ����ʹ�� `jekyll -s` �����ڱ���ʵʱ���ò��ͣ����Ч�ʡ���� [Jekyll.com](http://jekyllcn.com/)

�ο��ĵ���[using jekyll with pages](https://help.github.com/articles/using-jekyll-with-pages/) & [Upgrading from 2.x to 3.x](http://jekyllrb.com/docs/upgrading/2-to-3/)


## ��л

1. ���ģ���Ǵ����� [Hux](https://github.com/Huxpro/huxpro.github.io) fork ��, ��л������ߡ� 
2. ��л Jekyll��Github Pages �� Bootstrap!

## License

��ѭ MIT ���֤���й���ϸ,����� [LICENSE](https://github.com/lingyun0406/lingyun0406.github.io/blob/master/LICENSE)��
