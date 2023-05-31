---
layout: equipment
show_meta: false
title: "DCOB: 高自由度ロボットの運動学習ための行動空間"
subheadline: "NAIST Robotics Laboratory"
header:
   image_fullwidth: topics.jpg
permalink: "/Research/topics/RL-intro/"
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
強化学習手法は，報酬（目的）関数によって表現された目的のみから，ロボットが自律的に行動を獲得することを可能にします．しかしながら，ヒューマノイドのような高次元の制御入力空間への対処は，未解決問題のひとつです．

この研究のねらいは，ロボットが高速に高パフォーマンスな動作を学習できる，強化学習手法にとって最適な行動空間を開発することです．

私たちは，DCOBという離散行動集合を提案しました．DCOB は "an action Directed to the Center Of a Basis function"（基底関数の中心に向かう行動）を意味します．DCOB は価値関数を近似するために与えられた基底関数の集合から生成されます．DCOB は離散集合ですが，高いパフォーマンスの動作を獲得できます．

## <span style="font-size: 100%">跳躍の学習</span>
___
シミュレーション上のヒューマノイドロボットの跳躍タスクに DCOB を適用しました．強化学習手法としては，Peng の Q(λ)-learning を用いました．

学習の初期段階では，ロボットはランダムに振る舞います．これは，スクラッチ（事前知識を与えない）から学習したからです．

<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/aOf_Ia04GgE" frameborder="0" allowfullscreen></iframe>
</div>
</div>
<br/>
学習後，ロボットは跳躍を獲得できました

<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/KyhfYWQCf1g" frameborder="0" allowfullscreen></iframe>
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
## <span style="font-size: 100%">匍匐（ほふく）の学習</span>
___
学習前：
<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/zwTNJtiHVLU" frameborder="0" allowfullscreen></iframe>
</div>
</div>
 
<br/>
学習後：
<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/dUXJJ0cXhjI" frameborder="0" allowfullscreen></iframe>
</div>
</div>
## <span style="font-size: 100%">実ロボットの匍匐</span>
___
<a href="http://www.robotis.com/">ROBOTIS</a>社製のBioloidの匍匐学習に適用した例です．

この動画は学習段階です．ロボットは同様にスクラッチから学習します（シミュレーションなし）．


<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/VXiYhFK4TSY" frameborder="0" allowfullscreen></iframe>
</div>
</div>
 
<br/>
学習後，ロボットは匍匐の獲得に成功しました（約30分ほどです）．
<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/2Yoz-7OhJNs" frameborder="0" allowfullscreen></iframe>
</div>
</div>
 
<br/>
ほかの視点から：
<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/YzYLLhDS0tg" frameborder="0" allowfullscreen></iframe>
</div>
</div>

## <span style="font-size: 100%">メンバー</span>
___

- 山口明彦
 
<br/>


## <span style="font-size: 100%">主要関連論文</span>
___
- 山口 明彦, 高松 淳, 小笠原 司:
強化学習によるロボットの動作獲得のための基底関数に基づく行動空間生成手法,
日本ロボット学会誌, Vol.29, No.1, pp.55-66, 2011.
- 山口 明彦, 高松 淳, 小笠原司:
強化学習によるロボットの動作獲得のための基底関数に基づく行動空間生成手法DCOB ---実機多自由度ロボットの匍匐動作への適用---,
日本機械学会ロボティクス・メカトロニクス講演会2010(ROBOMEC2010), 2P1-G10, 旭川, 2010年6月.
- Akihiko Yamaguchi, Jun Takamatsu, and Tsukasa Ogasawara:
Constructing Action Set from Basis Functions for Reinforcement Learning of Robot Control,
in Proceedings of the 2009 IEEE International Conference on Robotics and Automation (ICRA2009), pp.2525-2532, Kobe, Japan, May, 2009.
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
