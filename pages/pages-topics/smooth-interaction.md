---
layout: equipment
show_meta: false
title: "インタラクション動作の生成"
subheadline: "NAIST Robotics Laboratory"
header:
   image_fullwidth: topics.jpg
permalink: "/Research/topics/smooth-interaction/"
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
人と人のインタラクションと同様に，人・ロボット間のインタラクションを考慮した際に，対話の実現は不可欠です．人型ロボットの場合，聴覚情報である音声対話の生成に加え，視覚情報であるボディジェスチャの生成も非常に重要になってきます．特に私たちは安全性などの面からロボットに人間に似た見た目を持つアンドロイドを用いています．このため，他のロボットと違い，さらに人間らしい動作生成が要求されます．

このボディジェスチャ生成に対して，私たちはこれまでに人間の動作データベースとオンラインプランニングを組み合わせた再構成可能な動作データベースを用いた動作生成手法を提案してきました．この手法には大きく分けて2つの特徴があります．

## <span style="font-size: 100%">応答性の高い動作生成</span>
___
オフラインの動作生成と違い，人との対話で必要となるジェスチャ動作の生成は高い応答性が必要となります．さらに，アクトロイドは人間らしい見た目を持つため動作においても人間らしい振る舞いが要求されます．

<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}smooth-interaction.jpg" alt="" style="width: 600px;" style="height: 350px;">
</div>
<br/>
<br/>
そこで，私たちはモーションキャプチャによって撮影された人間の動作をあらかじめ再構成可能な形でデータベース化し，それらをロボットの自己干渉なくスムーズに繋ぎあわせる手法を提案しました．これによりリアルタイム性と人間らしい動作生成を両立し，応答性の高いインタラクションを可能としました．

<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/_IfuhmEpJiI" frameborder="0" allowfullscreen></iframe>
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
## <span style="font-size: 100%">パラメータ合成による動作の最適化</span>
___
真正面の話者に対して特定された対話を行うと仮定すると，各ボディジェスチャはそれぞれ一つの固定された動作シーケンスを再生するだけで済みます．しかし，実世界ではそういった仮定は成り立ちません．話者は移動し，対象物（指さしたい物体など）は環境によって異なります．そこで，動作データベース中にある類似動作を，話者の立ち位置や対象物の指示方向などをパラメータとして合成することでこの問題を解決します.

<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}multi-person_hri.jpg" alt="" style="width: 600px;" style="height: 350px;">
</div>

<br/>
奈良先端科学技術大学院大学の情報科学研究科は，平城遷都1300年祭の会場で2010年10月2日〜15日にかけて各研究室が研究成果の展示を行いました（<a href="http://www.naist.jp/event/1300_j.html" rel="nofollow">http://www.naist.jp/event/1300_j.html</a>）． その中で，私たちロボティクス講座は多人数との対話を実現するインタラクションシステムのデモを行いました．このデモで得られた知見から，人間に与えるロボットの印象や滞留時間を向上させることが確認できました．

<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/xiJaDb7oeGE" frameborder="0" allowfullscreen></iframe>
</div>
</div>



## <span style="font-size: 100%">主要関連論文</span>
___
- 近藤 豊, 竹村 憲太郎, 高松 淳, 小笠原 司: データベースとオンラインプランニングを統合した高速応答可能なジェスチャ生成, 日本ロボット学会誌, Vol. 30, No. 9, pp. 899-906, 2012.
- Yutaka Kondo, Kentaro Takemura, Jun Takamatsu, and Tsukasa Ogasawara, “A Gesture-Centric Android System for Multi-Party Human-Robot Interaction,” Journal of Human-Robot Interaction, Vol. 2, No. 1, pp. 133-151, 2013.
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
