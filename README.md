#OITVL Live Player
バーチャルライブ用の映像再生システム

++++++++

## Description
複数の映像を複数の出力先にそれぞれ同時に提示することができる，キュー出しプログラムです．
同じタイミングで複数のプロジェクターにそれぞれ別の映像を同時再生する場合に便利です．
TouchDesignerで動作しますが，無料版では1280x1280以上の映像を出力できません．
開発途中のためUIは雑です．

## Usage
再生するメディアソースを用意し，出力先ごとにフォルダ分けしてください．
バーチャルライブだと，透過スクリーンに投影する用のメイン映像と，左右に投影する用のサブ映像がそれぞれあるかもしれません．
キューリストにあるキュー名でファイルを認識するので，同時に流す映像はキュー名とファイル名を統一してください．


画面と機能の説明です．


①パフォーマンスモニタ
フレーム落ちしてないかなど確認できます．

②コントローラーパネル
▶CUE　キューリストで選択中のキューを開始します．
AUTO　現在のキューが終了すると自動で次のキューを開始します．
Source　再生時間の基準にするメディアソースを選択します．
（追加実装予定）シーク機能，一時停止/再生機能，リピート機能，スキップ機能，タイムコード出力機能

③サウンド設定
Source　音声の出力元（メディアソース）と出力先（出力デバイス）を選択できます．

④キューリスト
キューを追加したり編集したりできます．
キューをダブルクリックするとキュー名を編集でき，D&Dすると順番を入れ替えることができます．
Load　.datで書かれたキューリストを読み込めます．
Save　現在のキューリストを.datで保存します．保存先フォルダとファイル名を指定してください．

⑤メディアソース設定
再生するメディアソース群を管理できます．
メディアソースが保存されているフォルダを選択してください．
（改善予定）タイムラインの共有化，再生処理の最適化

⑥出力設定
出力先（プロジェクター，サブモニタなど）を設定します．
Output　出力先を指定してください．
Open　出力ウィンドウを表示します．
Close　出力ウィンドウを閉じます．
Shutter　一時的に出力を停止し黒画面にします．
Source　出力するメディアソースを選択します．
W/H　出力解像度を指定します．出力先の画面サイズに合わせると良いと想います．
L/R/B/T　メディアソースをクリッピングします．横長映像などを分割する用途を想定しています．左下が0です．
（追加実装予定）NDI出力，プロジェクションマッピング用設定，

## Author
[lksrtk](https://github.com/lksrtk)

## References
