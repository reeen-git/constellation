# constellation
[AppStore](https://apps.apple.com/jp/app/stargazers/id1636193581)

※下記にある通り、夜に使用することを前提にしているので、UIは暗めです。   
黒を基調とし、文字は赤くしました。赤色は暗順応した目に優しい為です。
  
---------------------------------------------
高校生の時に天文部に所属していました。  

当時早見表派などを見ても、当然周りは暗く、目を暗順応させるため、できるだけ懐中電灯(減光したもの)も使いたくありませんでした。  
結果として、方角が分からず星が見れない or 懐中電灯を使いすぎて目が暗順応できずなかなか星が見れない、ということがよくありました。  
そこで、なるべく暗いUIで、また星座の位置や形が分かるアプリがあれば、その問題は解決するだろうと考えこのアプリを作成しました。
  
アプリを立ち上げると、端末から位置情報と時刻を取得し、「星を見る人API」より、その座標・その時刻に見れる星座一覧が帰ってきます。  
tableViewCellに星座名とその方角が表示されます。  
後に、cellをタップすると、indexに合わせたDetailViewに飛び、様々な情報（方角・高度・星座の写真や由来）を表示します。  
さらに、端末の方角の情報もリアルタイムで取得しているので、端末の角度とそこに表示されている角度が一致すれば、スマホの指す方向に星座が見えます。  
(実機デバッグで確認済み。シュミレータでは角度は表示されません。)

使用技術: Swift / UIKit / Nuke
