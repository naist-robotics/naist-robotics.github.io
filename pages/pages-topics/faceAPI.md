---
layout: equipment
show_meta: false
title: "アンドロイドロボットの表情生成"
subheadline: "NAIST Robotics Laboratory"
header:
   image_fullwidth: topics.jpg
permalink: "/Research/topics/faceAPI/"
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
人と人のインタラクションと同様に，人型ロボットが人間との対話を考えた時，人と同等の表情生成を行える事は必須事項です．豊かな表情を生成するため，私たちは顔に１３自由度を持つアンドロイドを用いています．

## <span style="font-size: 100%">ニューラルネットワークを用いた逆運動学</span>
___

アクトロイドの顔を制御するため、顔特徴点から人口ニューラルネットワークを用いて逆運動学を解きました。特徴点を口元と目の周りの二か所にグループ化し、独立に逆運動解放器を構成することによって実現しました。
<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}actIK.jpg" alt="" style="width: 600px;" style="height: 350px;">
</div>

## <span style="font-size: 100%">計算コストの削減</span>
___
先行研究では，顔特徴点の取得にはモーションキャプチャーが用いられていました．しかしモーションキャプチャーは計算コストが高く，このため人間の早い表情動作に追従できないでいました．そこで顔特徴点の抽出を計算ソフトに変更することによって，計算コストを削減しより早い表情動作に追従することを可能としました．

<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}faceAPI.jpg" alt="" style="width: 600px;" style="height: 350px;">
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
## <span style="font-size: 100%">アクチュエータ指令値の加工</span>
___
先行研究では，アクチュエータへの指令値とそれに対するポテンショ検出値を比較すると，変位が小さく振動しているような動作になっていました．そこで，変位と速度に注目して指令値を加工する事にしました．指令値をより大きく，変位の小さいアクチュエータを無視することによって人の表情動作に追従するような動作生成を可能としました．


<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/PGztcJYRTG4" frameborder="0" allowfullscreen></iframe>
</div>
</div>


## <span style="font-size: 100%">主要関連論文</span>
___
- Emarc Magtanong, Akihiko Yamaguchi, Kentaro Takemura, Jun Takamatsu, and Tsukasa Ogasawara: "Inverse Kinematics Solver for Android Faces with Elastic Skin", Latest Advances in Robot Kinematics, pp.181-188, 2012.
- 赤本 拓也, 山口 明彦, 高松 淳, 小笠原 司: "RGB-Dセンサから取得した特徴点座標によるアンドロイドのリアルタイム表情生成", 日本機械学会ロボティクスメカトロニクス講演会2013(ROBOMEC2013), 2P1-P23, May 22-25, 2013.
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
