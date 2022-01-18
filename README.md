# powershell
powershell　コマンド

パワーシェルで文字化けで日本が読めない
バージョンを2022年で最新　7.3.0をインストールした
文字コードがUTF-8になり　日本語表示　成功


コマンドラインで以下を入力して確認
$PSVersionTable　バージョンを確認
$OutputEncoding.EncodingName　　文字コードを確認



ウィンドウズのパワーシェルで以下のコマンドを入力
説明　PS C:\Users\name(ここはカレントディレクトリ)

PS C:\Users\name> $PSVersionTable

Name                           Value
----                           -----
PSVersion                      7.3.0-preview.1
PSEdition                      Core
GitCommitId                    7.3.0-preview.1
OS                             Microsoft Windows 

バージョン7．3.0　GITHUBでmsi形式のファイルをダウンロードしてウィンドウズで実行

文字コードを確認
PS C:\Users\name> $OutputEncoding.EncodingName

Unicode (UTF-8)

文字コードがUTF-8になっている。


PS C:\Users\name> get-content a.txt


あいうえお

かきくけこ



日本語が表示された



今までバージョン5.1では文字化けしていた

パワーシェル　PSVersion   5.1.　Edition            Desktop

PS C:\Users\name> $OutputEncoding.EncodingName

US-ASCII

PS C:\Users\name> get-content a.txt

縺ゅ＞縺・∴縺・縺九″縺上￠縺・

上記のように文字化け　US　ASCII　のため
