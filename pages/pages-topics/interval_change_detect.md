---
layout: equipment
show_meta: false
title: "インターバル計測を用いた環境変化の抽出"
subheadline: "NAIST Robotics Laboratory"
header:
   image_fullwidth: topics.jpg
permalink: "/Research/topics/interval_change_detect/"
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
日常生活の中でおきる環境の変化を観測することで，物の動かしやすさ，変化の規則性などの物に付随するセマンティクスを抽出することができる．また，環境の変化した部分のみを更新することで，日常生活における物の管理や，ロボットにおけるマップ更新の効率化も実現することができる．

本研究では，時間的に間隔をおいて計測された3次元データから，変化した部分を検出するのみでなく，どのような変化（出現・消失，もしくは単なる計測範囲の違い）がおこったのかを認識することができる．
## <span style="font-size: 100%">キーテクノロジー</span>
___
3次元センサは，対象物までの距離の情報を提示するのみならず，対象物までの間に障害物が存在しないこと，対象物の後ろは不可視領域であること，の計3つの情報を教えてくれる．
<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}key.jpg" alt="" style="width: 600px;" style="height: 350px;">
</div>
<br/>
<br/>
前回計測したデータにおいて，障害物が存在しない領域に計測データが現れた場合，それは新たに物体が出現したことがわかる．また前回計測したデータにおいて，不可視領域である領域に計測データが現れたとしても，それは単なる計測範囲の違いによる変化であることがわかる．


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
## <span style="font-size: 100%">工事現場で適用した例</span>
___

下図に示すように，工事の前後で草木が刈られた領域は正しく検出されていることはもちろんのこと，フェンスによって射影領域になった部分，および草木が刈られたことによって，奥が見えるようになったことなど，フェンスや草木が目隠しとしての効果を発揮することなどが理解できる可能性を示唆している．
 
<br/>
<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}result.jpg" alt="" style="width: 600px;" style="height: 350px;">
</div>
## <span style="font-size: 100%">メンバー</span>
___
- 田辺雅人

## <span style="font-size: 100%">主要関連論文</span>
___
- 田辺雅人, 竹村憲太郎, 吉川雅博, 高松淳, 小笠原司: 
"インターバル３次元計測からの環境変化の検出",
第14回計測自動制御学会システムインテグレーション部門講演会(SI2013), 2K3-4, Dec 18-20, 2013. 
- 田辺雅人, 吉川雅博, 竹村憲太郎, 高松淳, 小笠原司: 
"インターバル 3 次元形 状計測からの環境変化の識別",
ロボティクスメカトロニクス講演会 2014(ROBOMECH2014), 3P1-I02, 2014.

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
