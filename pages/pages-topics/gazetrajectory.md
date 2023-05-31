---
layout: equipment
show_meta: false
title: "実環境における三次元注視軌跡の解析"
subheadline: "NAIST Robotics Laboratory"
header:
   image_fullwidth: topics.jpg
permalink: "/Research/topics/gazetrajectory/"
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
人は見るという行為から情報を取得し，高次認知処理によって行動を決定しています．そのため，認知心理学や人間工学，ヒューマンインタフェースの研究では視線行動を計測することによって，人の興味関心を解析します．

しかしながら，計測される注視点はディスプレイやカメラ画像などの特定平面上の二次元座標として取得されるため，視線情報と環境の三次元的な対応関係を解くことが困難となります.

この研究では，ViualSLAMや3D Feature Mapなどの手法により生成された環境の三次元地図を用いることで，三次元空間上での注視点計測を行っています.
## <span style="font-size: 100%">EyeTracking</span>
___
視線計測は視線計測装置ViewPoint EyeTrackerを頭部に装着し，人間の眼球運動と視野映像を二つのカメラを用いて同時に取得します．そして，人間が対象物に対して注視しているときの瞳孔中心と, 近赤外光が角膜表面で反射することよって生じるプルキニエ像との位置関係を利用することで，カメラ画像中の二次元注視点を算出します．

<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/0SVEnadVPPE" frameborder="0" allowfullscreen></iframe>
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

## <span style="font-size: 100%">ViualSLAM</span>
___
ViualSLAMは未知環境を移動する際に，カメラ画像を用いて自己位置推定と地図生成を同時におこなう手法である．具体的にはFAST特徴検出を用いて画像中に存在する自然特徴点の検出を行い，それをキーフレーム間の視差により三次元空間にマッピングします．そして，取得した特徴点の位置関係からカメラの位置・姿勢をトラッキングします．

本研究では広範囲な環境を想定しているのでカメラ位置をそのまま人間の頭部位置として扱っています.
<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/KuOTHiMsvEU" frameborder="0" allowfullscreen></iframe>
</div>
</div>
 
<br/>


## <span style="font-size: 100%">3D Feature Map</span>
___
3D Feature Mapは，色付き三次元点群と三次元位置が既知となったSIFT特徴量から構成されます．環境中に移動ロボットを走行させ，オドメトリ情報，垂直水平方向のスキャンデータ，さらに画像データを取得します．そして，オドメトリ情報と水平方向のスキャンデータを用いてSLAMを行い，移動ロボットの移動経路を推定します．さらに，推定された移動経路をもとに垂直方向のスキャンデータを積層して三次元点群データを生成します．また，垂直方向のスキャンデータを画像上に投影し，投影された位置の色情報を取得することで色情報が付加された三次元地図を生成します．
<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/hgcvzIOOUz0" frameborder="0" allowfullscreen></iframe>
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
## <span style="font-size: 100%">三次元注視点計測と可視化手法</span>
___
Visual SLAMにより取得した自然特徴点を用いて，画像平面上の視線情報と環境情報を関連付ます．三次元注視点が自然特徴点から構成される平面上に位置すると仮定し，自然特徴点と注視点の画像上での位置関係から注視点の三次元位置を求めることが可能となります．

そして，算出した三次元注視点をもとに，三次元的な注視点軌跡の計測及び注視頻度マップの生成を行います．軌跡に関しては，三次元注視点として推定された座標を記録して三次元軌跡を記述します．注視頻度に関しては，注視点を内包する自然特徴点で構成された三角形の各頂点に対して，一定の注視頻度を付与することで，画像ではなく環境に対する正確な注視頻度の記録を実現しました．また，他の観察者との視線を重ね合わせることによって，視認しながら比較することが可能となります.
<div style="text-align:center">
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/XQCS03XGHf0" frameborder="0" allowfullscreen></iframe>
</div>
</div>
 
<br/>


## <span style="font-size: 100%">メンバー</span>
___

- 竹村憲太郎
 
<br/>


## <span style="font-size: 100%">主要関連論文</span>
___
- Kentaro Takemura, Yuji Kohashi, Tsuyoshi Suenaga, Jun Takamatsu, and Tsukasa Ogasawara:
Estimating 3D Point-of-regard and Visualizing Gaze Trajectories under Natural Head Movement,
Proc. of ETRA2010 : ACM Symposium on Eye-Tracking Research & Applications, pp.157-160, 2010.
- 高橋健治, 竹村憲太郎, 末永剛, 高松淳, 小笠原司:
移動ロボットによるSIFTを用いた三次元特徴点地図の生成, 
第28回日本ロボット学会学術講演会予稿集, RSJ2010AC1Q3-2, 2010.
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
