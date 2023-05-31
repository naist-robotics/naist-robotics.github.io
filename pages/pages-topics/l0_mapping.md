---
layout: equipment
show_meta: false
title: "動的環境におけるリアルタイム地図生成"
subheadline: "NAIST Robotics Laboratory"
header:
   image_fullwidth: topics.jpg
permalink: "/Research/topics/l0_mapping/"
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
これまでのロボットは，工場や実験室のような意図的に整えられた環境で働くことが求められていました．しかし，近年ではロボットを人がたくさんいるような日常生活環境下で働かせたいという要求が高まっています．そのような環境でロボットを働かせるためには，ロボット自身が周囲の環境を正しく認識することが必要になります．

本研究では，センサによる観測の対応付けの評価にL0ノルムを利用することで，動的な混雑環境下でも適用可能なSLAMを提案しました．また，近似最近傍探索アルゴリズムと重点的サンプリングを利用することで，処理のリアルタイム化を実現しました．

## <span style="font-size: 100%">L0ノルム最小化によるSLAM</span>
___
SLAMは未知環境を移動する際にセンサから得られるデータを用いて自己位置推定と地図生成を同時に行う手法です．本研究ではLIDARを用いて周囲の物体までの距離を計測し，フレーム間でのマッチングを行なって地図を作成します．

<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/0MibqgZ_eeo" frameborder="0" allowfullscreen></iframe>
</div>
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
## <span style="font-size: 100%">リアルタイムSLAM</span>
___
実際に人間が歩きまわる環境でロボットを走行させ，動的な混雑環境下での地図生成の性能を確認しています．




<br/>


## <span style="font-size: 100%">メンバー</span>
___

- 日永田 佑介
- 竹村 憲太郎

<br/>


## <span style="font-size: 100%">主要関連論文</span>
___
- 日永田 佑介, 末永 剛, 竹村 憲太郎, 高松 淳, 小笠原 司:
"L0ノルム最小化による動的環境下に適用可能なSLAM",
第11回計測自動制御学会システムインテグレーション部門講演会, pp.1648-1651, 2010.
- 日永田佑介, 末永剛, 竹村憲太郎, 高松淳, 小笠原司:
"L0ノルム最小化を利用した動的な混雑環境下に適用可能なリアルタイムSLAM",
画像の認識・理解シンポジウム(MIRU2011), IS3-56, 2011.
- Y. Hieida, T. Suenaga, K. Takemura, J. Takamatsu and T. Ogasawara: "Real-time Scan-Matching Using L0-norm Minimization Under Dynamic Crowded Environment", 4th IROS Workshop on Planning, Perception and Navigation for Intelligent Vehicles , 2012.
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
