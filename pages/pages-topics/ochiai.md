---
layout: equipment
show_meta: false
title: "タッチインターフェースを利用した移動ロボットの遠隔操作"
subheadline: "NAIST Robotics Laboratory"
header:
   image_fullwidth: topics.jpg
permalink: "/Research/topics/ochiai/"
---

<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**<a href="{{ site.url }}{{ site.baseurl }}/Research/">研究</a>**

{: #toc }
*  <a href="{{ site.url }}{{ site.baseurl }}/Research/equipment/">研究設備</a>  
*  <a href="{{ site.url }}{{ site.baseurl }}/Research/topics/">研究紹介</a>  
*  <a href="{{ site.url }}{{ site.baseurl }}/Research/publication/">業績リスト</a>  
*  <a href="{{ site.url }}{{ site.baseurl }}/Research/press/">マスメディア報道</a>  

{:toc}
</div>
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">
これまでの遠隔操作ロボットは，ジョイスティックなどで操作することが多かった．しかし，このような方式では操縦者が操縦に習熟するまでに時間がかかったり，1人で1台しか操作できないといった問題がありました．

本研究では，タブレット端末を用いることで素人でも操作しやすく，かつ1人で複数台のロボットを操作できるシステムを提案しました．タブレット端末を通じて，ユーザーが経由地や目標地点の情報を入力し，RRT (Rapidly-exploring Random Tree)による経路計画を行い，指示経路付近を重点的に探索することでユーザの意図に沿った探索を実現しています

<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/1qU7W_YFcVI" frameborder="0" allowfullscreen></iframe>
</div>
</div>

## <span style="font-size: 100%">タッチパネルインタフェースによる経路指定</span>
___
タブレット端末にはロボットがその時点で推定した地図と自己位置が表示されます．ユーザは，まだ地図ができていない領域も含めてタッチ操作によってマーカーを配置することができます．ロボットは，このマーカーを目印にして探索を行います．また，ロボットを複数台操作する場合は，この端末上で指示対象のロボットを切り替えることが可能です．

<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}tablet.jpg" alt="" style="width: 600px;" style="height: 350px;">
</div>

</div>
</div><!-- /.row -->

<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**<a href="{{ site.url }}{{ site.baseurl }}/Research/">研究</a>**

{: #toc }
*  <a href="{{ site.url }}{{ site.baseurl }}/Research/equipment/">研究設備</a>  
*  <a href="{{ site.url }}{{ site.baseurl }}/Research/topics/">研究紹介</a>  
*  <a href="{{ site.url }}{{ site.baseurl }}/Research/publication/">業績リスト</a>  
*  <a href="{{ site.url }}{{ site.baseurl }}/Research/press/">マスメディア報道</a>  

{:toc}
</div>
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">
## <span style="font-size: 100%">指示経路を利用した未知環境の経路計画</span>
___
経路計画はRRT(Rapidly-exploring Random Tree)を用いて行います．しかし，従来手法ではユーザの意図に沿わない経路を計画することがあります．そこで，RRTの探索木の成長時に指示経路付近を重点的に探索することで，ユーザの意図に近い移動を行えるようになりました．


<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}map2.jpg" alt="" style="width: 600px;" style="height: 350px;">
</div>
 
<br/>


## <span style="font-size: 100%">メンバー</span>
___

- 落合 佑哉
 
<br/>


## <span style="font-size: 100%">主要関連論文</span>
___
- Yuya Ochiai, Kentaro Takemura, Atsutoshi Ikeda, Jun Takamatsu, and Tsukasa Ogasawara, “Remote Control System for Multiple Mobile Robots using Touch Panel Interface and Autonomous Mobility”, in Proc. of IEEE/RSJ Int. Conf. on Intelligent Robots and Systems, pp. 3272-3277, 2014.
</div> 
</div><!-- /.row -->



 [1]: http://kramdown.gettalong.org/converter/html.html#toc
 [2]: {{ site.url }}/blog/
 [3]: http://srobbin.com/jquery-plugins/backstretch/
 [4]: #
 [5]: #
 [6]: #
 [7]: #
 [8]: #
 [9]: #
 [10]: #
