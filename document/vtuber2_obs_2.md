# 透過PNG、透過GIFをOBSでキャプチャすると透過部分が黒くなる
---
OBSは背景が透過されたウィンドウを正しくキャプチャできないようです。「だれでもVtuber」をOBSと連携させたい場合は、画像背景を単色で塗りつぶしてください[^1]。
+ <ruby>GB<rp>（</rp><rt>グリーンバック</rt><rp>）</rp></ruby>や<ruby>BB<rp>（</rp><rt>ブルーバック</rt><rp>）</rp></ruby>をOBS上で透過する手順
    1. `ソース`一覧のキャプチャ項目を右クリックして`フィルタ`を選択します。
        <div style="text-align:center">
            <img src="images\vtuber2\OBS004.png">
        </div>
    1. 表示されたフィルタウィンドウの`エフェクトフィルタ`に`カラーキー`または`クロマキー`を追加してください。
        <div style="text-align:center">
            <img src="images\vtuber2\OBS005.png">
        </div>
    1. `カラーキー`を使用する場合は、`色キーの種類`で`カスタム色`を選択し、`キーの色`に背景色と同じ色をHTMLカラーコードで指定してください。
        <div style="text-align:center">
            <img src="images\vtuber2\OBS006.png">
        </div>
    1. `滑らかさ`のトラックバーを調節することで、ジャギーの発生を抑えることができます。
        <div style="text-align:center">
            <img src="images\vtuber2\OBS007.png">
        </div>

---
+ [だれでもVtuber QA 目次ページに戻る](index_vtuber2_qa.md)
+ [だれでもVtuber 目次ページに戻る](index_vtuber2.md)
+ [トップページに戻る](index_top.md#falhong-cha)

[^1]: <ruby>GB<rp>（</rp><rt>グリーンバック</rt><rp>）</rp></ruby>や<ruby>BB<rp>（</rp><rt>ブルーバック</rt><rp>）</rp></ruby>など