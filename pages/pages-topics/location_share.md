---
layout: equipment
show_meta: false
title: "人と共存可能な移動ロボットシステム"
subheadline: "NAIST Robotics Laboratory"
header:
   image_fullwidth: topics.jpg
permalink: "/Research/topics/location_share/"
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
ロボット技術の進歩に伴い，単一ロボットだけでは提供が困難なサービスに対し，複数のロボットが協調してサービスを提供する枠組みに関する研究が盛んに行われています．しかしながら，複数のロボットの仕様を共通化することは難しく，センサの種類や位置が異なる異種ロボット間では，地図情報や位置情報を共有することが困難となる問題が存在します．また，ロボットが公共の場でサービスを提供するためには，個々のロボットが正確に自己位置推定を行うことが重要となります．

本研究では，各ロボットが自己位置推定を行っている座標系を統一することで位置情報共有の問題について解決する手法の提案を行いました．また，従来までノイズとして扱われていた周囲の人間の情報を積極的に利用し，人間の位置情報と共有したロボットの位置情報をもとに相互位置推定を行うことにより，人間が存在する環境での自己位置推定精度の向上を実現しました.


## <span style="font-size: 100%">汎用三次元環境地図を用いた位置情報共有</span>
___
ロボットに搭載されているセンサが異なると，それによって必要となる地図の種類が異なるため，各ロボットが自己位置推定を行う座標系に座標軸やスケールの違いが発生する．全方位カメラとLIDARの計測データから作成した汎用三次元環境地図を用いてこの問題を解消している．汎用三次元環境地図を変換して各ロボットが使用する位置推定手法に合わせた様々な地図を作成することで，お互いの位置情報を共有している．

<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}location_share.jpg" alt="" style="width: 600px;" style="height: 350px;">
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
## <span style="font-size: 100%">相互位置推定</span>
___
各ロボットが搭載しているセンサを用いて自己位置推定を行い，同時に人間を検出して相互位置推定を行うことで動的な環境下での相互位置推定の性能を確認する．青い三角がロボット1，赤い三角がロボット2を表す．


<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/LsEepAongc8" frameborder="0" allowfullscreen></iframe>
</div>
</div>
 
<br/>


## <span style="font-size: 100%">メンバー</span>
___

- 桑原 潤一郎
- 竹村 憲太郎
 
<br/>


## <span style="font-size: 100%">主要関連論文</span>
___
- 桑原 潤一郎, 伊藤 晃大, 日永田 佑介, 竹村 憲太郎, 末永 剛, 高松 淳, 小笠原 司:
RTミドルウェアを利用した異種ロボット間での位置情報共有,
ロボティクス・メカトロニクス講演会2010, 2A2-C05, 2010.
- 桑原 潤一郎, 竹村 憲太郎, 末永 剛, 高松 淳, 小笠原 司:
ユニバーサルマップを利用した異種ロボットにおける位置情報共有,
第28回日本ロボット学会学術講演会, RSJ2010AC1Q1-5, 2010.
- 桑原 潤一郎, 竹村 憲太郎, 末永 剛, 高松 淳, 小笠原 司:
移動ロボットのネットワーク化と制御用RTコンポーネント,
第11回計測自動制御学会システムインテグレーション部門講演会, pp.1068-1069, 2010.
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
