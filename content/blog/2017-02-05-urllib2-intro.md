---
author: David
categories:
- 技術簡介
- 雜七雜八
- Python
comments: true
date: "2017-02-05T00:00:00Z"
modified: "2017-02-05"
published: true
tags:
- python2
- python
- urllib
- urllib2
- wget
- curl
title: Python套件urllib2簡介
---
這裡就像哈利波特裡的儲思盆<br />
趁著我在當兵前還沒完全放空的時候<br />
把這些東西倒出來<br />
<br />
還以為我會很緊張要當兵了<br />
沒想到居然心如止水 來講講一個小套件<br />
<br />
今天講Python的一個小小小小套件 , urllib2<br />
<br />
基本上不需要額外安裝任何新的module就可以使用，所以用來救急很方便<br />
<br />
當有時候需要使用程式對某一網頁做POST或GET並獲得response時<br />
使用urllib2就非常方便<br />
<br />
簡單的幾行程式碼就可以搞定<br />
<br />
範例程式如下：<br />
我們對google首頁做GET<br />
<br />
# /usr/bin/env python<br />
# encoding: utf-8<br />
<br />
import urllib2<br />
<br />
request = urllib2.Request("http://www.google.com.tw/")<br />
response = urllib2.urlopen(request)<br />
html = response.read()<br />
print html<br />
<br />
<br />
去執行python 程式名稱就可以看到GET網頁的內容了<br />
非常簡單且快速<br />
用來撈取資料或做POST、GET都很方便<br />
<br />
<br />
當然，你也可以使用linux環境下的wget、curl等套件來達成。<br />
<br />
因為腦袋放太空不適合一次寫太多東西<br />
就先這樣好了<br />
<br />
<br />
<br />
<br />
<br />
<br />
<div style="text-align: right;">
2017-02-05 12:46 , Davin in Taipei</div>
<div style="text-align: right;">
<br /></div>

