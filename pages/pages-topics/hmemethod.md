---
layout: equipment
show_meta: false
title: "筋電センサによる手の動作認識"
subheadline: "NAIST Robotics Laboratory"
header:
   image_fullwidth: topics.jpg
permalink: "/Research/topics/hmemethod/"
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
<div style="text-align:center">
<img class="t50" src="{{ site.urlimg }}hmemethod.jpg" alt="" style="width: 600px;" style="height: 350px;">
</div>
脳の運動指令が筋肉に伝わり，筋肉が収縮する際，筋上に電気的な信号=筋電位が発生します．この筋電位は，皮膚表面から容易に計測可能です．この筋電位を利用して手の動作意図を推定する動作認識法を開発しています．本手法は，サポートベクターマシン（SVM）に基づいて構築しています．筋電義手やロボットハンドの制御を目的としています．

<div class="flex-video">
        <iframe width="400" height="400" src="//www.youtube.com/embed/gUChcd9xeHU" frameborder="0" allowfullscreen></iframe>
</div>
<br/>
<br/>

はじめに操作者の筋電位を60秒間計測し，そのデータを元に使用者の筋電パターンを学習します．学習自体は30秒程度で終わります．学習が完了すると，手関節掌屈，手関節背屈，手を閉じる，手を開く，前腕回内，前腕回外，中立位の7動作を認識し，ロボットハンドの操作が可能になります
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

## <span style="font-size: 100%">メンバー</span>
___
- 吉川 雅博
<br/>


## <span style="font-size: 100%">主要関連論文</span>
___
- Masahiro Yoshikawa, Masahiko Mikawa, Kazuyo Tanaka, "A Myoelectric Interface for Robotic Hand Control Using Support Vector Machine, "IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS2007), San Diego, America, pp.2723-2728, Oct, 2007.
- 吉川雅博, 三河正彦, 田中和世, "筋電位を利用したサポートベクターマシンによる手のリアルタイム動作識別, "電子情報通信学会論文誌D, vol.J92-D, no.1, pp.93-103, 2009.
- 吉川雅博, 三田友記, 三河正彦, 田中和世, "前腕切断者を対象とした筋電位信号に基づく手の動作識別法に関する基礎的研究, "人間工学, vol.46, no.3, pp.197-207, 2010.
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
