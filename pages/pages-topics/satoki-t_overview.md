---
layout: equipment
show_meta: false
title: "視覚と行動計画を伴うヒューマノイドロボットのサービス提供"
subheadline: "NAIST Robotics Laboratory"
header:
   image_fullwidth: topics.jpg
permalink: "/Research/topics/satoki-t_overview/"
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
人間を助けるためのロボットサービスの実装に向けて，私たちはヒューマノイドロボットにおける実時間での家事動作生成を試みています． 家事には，コップなどの操作する物体の認識や，テーブルなどの環境と干渉しないための動作計画が必要です． さらに，サービスに対する人間の満足度を得るためには，これらの認識と行動計画の上に実時間で動作を生成することが求められます．

<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}satoki-t_overview.jpg" alt="" style="width: 600px;" style="height: 350px;">
</div>

<br/>
<br/>

環境の認識のために，人間の動作を基に生成された3Dポイントクラウドマップであるセマンティックマップを用い， 操作する物体の認識のために，マーカを用いた<a href="http://www.hitl.washington.edu/artoolkit/">ARToolKit</a>を用いて，動作生成に必要な情報を得ます． これらに基づいて，ヒューマノイドロボット全身の逆運動学を計算することで動作を生成し，ロボットを制御します．

本研究を適用するロボットとして，本研究室で所有している<a href="{{ site.url }}{{ site.baseurl }}/Research/equipment/HRP-4/">HRP-4</a>を用いて実験しています．
## <span style="font-size: 100%">ヒューマノイドロボットにおける給仕動作</span>
___
人間の生活環境でのロボットの給仕動作に向けて，人間が用いる電気ポットとコップを使ってHRP-4にお湯を注ぐ動作を実装しました． 腕を使って物体を操作する動作において，双腕での協調制御を実装することで実時間性を高めています．


<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/15SX5kmmEiY" frameborder="0" allowfullscreen></iframe>
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
## <span style="font-size: 100%">視覚に基づく上半身動作生成</span>
___
上記の給仕動作で得られた動作に，各関節の動かしやすさを等価に考えるヤコビアンを用いて動作生成を行った結果，腰を反る動作が生成されてしまいます． 通常のヤコビアンを逆運動学に適用する際に各関節の重みを考慮することで，自然で安定な双腕動作を生成しました．

また，実際の操作物体の位置変化に対応するために，HRP-4の頭部のUSBカメラを通じて，マーカの位置を計測しました． カメラ座標系で得られたマーカをロボット座標系に変換して，HRP-4の双腕をマーカの位置に制御しました．

<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/f0-7qnF5NM4" frameborder="0" allowfullscreen></iframe>
</div>
</div>

## <span style="font-size: 100%">メンバー</span>
___
- 築地原 里樹
 
<br/>


## <span style="font-size: 100%">主要関連論文</span>
___
- 築地原 里樹, 山口 明彦, 吉川 雅博, 高松 淳, 小笠原 司:
ヒューマノイドロボットにおける重み付きヤコビアンを用いた視覚に基づく上半身動作の生成,
第20回ロボティクスシンポジア, 2C2, 2015年3月15-16日.
- 築地原 里樹, 山口 明彦, 吉川 雅博, 高松 淳, 小笠原 司:
等身大ヒューマノイドロボットによる給仕動作の実現と実行時間に対する考察,
第32回日本ロボット学会学術講演会, 1C3-02, 2014年9月4-6日.
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
