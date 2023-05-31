---
layout: equipment
show_meta: false
title: "モーションキャプチャデータの多様化"
subheadline: "NAIST Robotics Laboratory"
header:
   image_fullwidth: topics.jpg
permalink: "/Research/topics/motionsynth/"
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
## <span style="font-size: 100%">運動学習プリミティブの演算による動作の多様化</span>
___
ロボットやCGキャラクタの動作生成のために，モーションキャプチャなどのシステムを利用する方法が普及しています． しかしながら，モーションキャプチャで取得した動作のみでは，決まりきった動作しか生成できません．

そこで，この研究では，「運動学習プリミティブ」という表現形を用いて動作を表現し，運動学習プリミティブに対する演算を定義することによって動作を多様化する手法を開発しました．
<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}1_FlowChart_short.jpg" alt="" style="width: 600px;" style="height: 350px;">
</div>

## <span style="font-size: 100%">運動学習プリミティブ</span>
___

運動学習プリミティブは，非線形の力学系を用いて動作を表現するものです．これにより，単に関節角の時系列データを保持する場合に比べて，

- パンチ動作の打点変更など，動作の到達位置（姿勢）や到達時間を自然に変更できる
- 任意の位置から動作を開始できる  
という利点があります．

## <span style="font-size: 100%">運動学習プリミティブの演算</span>
___
この研究では，運動学習プリミティブに対して以下のような演算を定義しました．

- ふたつの運動学習プリミティブを連結
- ひとつの運動学習プリミティブを任意の時間で分割
- ふたつの運動学習プリミティブを時間的に並列に合成



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
## <span style="font-size: 100%">適用例 </span>
___
以下のような動作をプリミティブとしてデータベース化しているとします．


<div class="flex-video">
        <iframe width="400" height="400" src="//www.youtube.com/embed/_Oga4XFHk4w" frameborder="0" allowfullscreen></iframe>
</div>
<div class="flex-video">
        <iframe width="400" height="400" src="//www.youtube.com/embed/3jQG5XoX-jM" frameborder="0" allowfullscreen></iframe>
</div>
<br/>
このとき，跳躍と膝蹴りを「合成」することによって，以下のようにとび膝蹴りが実現できます．

<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}5_hiknee_abs_SICE.jpg" alt="" style="width: 300px;" style="height: 250px;">
<div class="flex-video">
        <iframe width="400" height="400" src="//www.youtube.com/embed/J4JPjNgqE24" frameborder="0" allowfullscreen></iframe>
</div>
</div>
<br/>
次の例は，跳躍を屈伸部や着地部で分割し，時間調整することによって生成した，「スーパーハイジャンプ」です．

<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}5_shjump_abs_SICE.jpg" alt="" style="width: 300px;" style="height: 250px;">
<div class="flex-video">
        <iframe width="400" height="400" src="//www.youtube.com/embed/EQJ3je_J9eQ" frameborder="0" allowfullscreen></iframe>
</div>
</div>
## <span style="font-size: 100%">メンバー</span>
___
- 竹内 喜之
- 山口 明彦
<br/>


## <span style="font-size: 100%">主要関連論文</span>
___
- 竹内 喜之, 山口 明彦, 竹村 憲太郎, 高松 淳, 小笠原 司:
モーションキャプチャデータから多様な動作生成を可能にする運動学習プリミティブの合成,
第10回システムインテグレーション部門講演会(SI2009), 1M4_7, pp.824-827, 2009年12月.
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
