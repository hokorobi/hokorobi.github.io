使用ソフトとその用途
====================

.. role:: strike

Update はソフトウェアがバージョンアップされた日ではなく、『私がそのバージョンのソフトウェアをインストールした日』です。

使用中
------


ファイル関係
~~~~~~~~~~~~

.. list-table:: ファイル関係諸々
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `fenrir <http://hp.vector.co.jp/authors/VA026310/>`_
     - 0.75c
     - | ディレクトリのインデックスを作成し、インクリメンタルサーチでディレクトリを開く。
       | 私には、DF の登録ディレクトリを使った移動で十分な気もする。
       | `起動までのライムラグのうちに、キーボードを叩き始めて、ファイラがアクティブになってしまったり、アプリケーションエラーで落ちたりするので使ってない。`:strike:
       | Paper Plane xUI でディレクトリの移動に使っている。
     - 2008-03-18
   * - `Paper Plane xUI <http://toro.d.dooo.jp/slppx.html>`_
     - 1.72 x64
     - DF 並に起動が速いけれど、カスタマイズが大変 (楽しい？) なファイラ。
     - 2020-03-22
   * - `Paper Plane xUI Window Module <http://toro.d.dooo.jp/slppx.html>`_
     - R7
     - 指定したウィンドウの最大化を交互におこなうコマンドと、指定したウィンドウ位置・大きさを別のウィンドウに合わせるコマンドが入った PPx Module。
     - 2016-09-03
   * - `Paper Plane xUI Script Module <http://toro.d.dooo.jp/slppx.html>`_
     - R18
     - スクリプトを使えるようにするモジュール。
       R17+1: ログが出力されるのでやめ
       `R17+2: リネーム用スクリプトで ESC を押すと環境依存文字が入力されるのでやめ`:strike: 本体側が原因 1.69+3 で修正
     - 2020-01-13
   * - `Paper Plane xUI Text Module <http://toro.d.dooo.jp/slppx.html>`_
     - R4
     - テキスト関係のコマンドを使えるようにするモジュール。
     - 2018-08-15
   * - `7zca.dll <http://toro.d.dooo.jp/slplugin.html>`_
     - 0.4
     - 7-Zipに入っている7z.dllを使った 7z等の書庫の展開ライブラリ。
       PPx で使用する定義は書いている。実際に使われているかは不明。
       7-Zip の 7z.dll を 7z64.dll にしてアーカイバDLLのフォルダへコピーしている。
     - 2020-01-13
   * - `bregonig.dll <http://homepage3.nifty.com/k-takata/>`_
     - 4.20 x64
     - Paper Plane xUI で正規表現を使えるようにする。
     - 2019-02-02
   * - `C/Migemo <http://www.kaoriya.net/software/cmigemo>`_
     - 20110227 x64
     - Paper Plane xUI で Migemo を使うため。
     - 2011-12-24
   * - `FastCopy <http://www.ipmsg.org/tools/fastcopy.html>`_
     - 3.86 x64
     - | 大量ファイルの削除時に使用。
       | 削除確認は PPx 側でダイアログを出して、実行時には /no_confirm_del を指定。
     - 2020-02-01
   * - `FreeFileSync <http://freefilesync.sourceforge.net/>`_
     - 10.15
     - ファイルのバックアップ。
     - 2019-09-08
   * - `FastHash <http://hp.vector.co.jp/authors/VA033110/>`_
     - 0.39β
     - | ファイルが同じものなのかどうか確認。
       | MD5 も計算できるのでネットで公表されているものと確認できる。
     - 不明
   * - `Avira AntiVir Personal - FREE <http://www.free-av.com/>`_
     - 随時
     - | アンチウィルスソフト。
       | BitDefender で手動チェックするだけでいいかな～と思っていたけれど、なんとなく常駐版もほしいかもと思い始めたので導入。
       | `http://www.avpusers.org/ug4win/config_guard.html を見て Scan Archive へチェックを付けて Web ブラウザからダウンロードするファイルの Scan もさせるようにした。`:strike:
       | 実行させたときに引っかかればいいやということで、やっぱやめ。
       | 他にも設定するべきところはあるだろうけど、とりあえずそのまま。
       | バージョンは手動でインストールしたときのもの。随時、バージョンアップ中。
       | 自動起動する avgnt のコマンドラインに /nosplash というオプションを追加。
     - 2016-07-10
   * - `WizTree <http://antibody-software.com/web/software/software/wiztree-finds-the-files-and-folders-using-the-most-disk-space-on-your-hard-drive/>`_
     - 3.28
     - ディスク領域を多く使っているディレクトリを一覧表示する。MFT を使っているので高速。
     - 2019-02-06
   * - `SpaceSniffer <http://www.uderzo.it/main_products/space_sniffer/index.html>`_
     - 1.1.3.1
     - WindowsPCのハードディスクの占有状況を高速に分析するツール。
     - 2011-05-19
   * - `Everything <http://www.voidtools.com/>`_
     - 1.4.1.935
     - | NTFS change Journal を使って高速ファイル検索。
       | こちらも管理者権限が必要なのは同様だが、ETP というプロトコルでの通信ができるので PPx から使っている。
       | Command-line interface の es もインストール。パスの通っている cmd へ。[2013-05-27]
       | Everything -install-service でサービスへ追加。これにより Everything は通常権限で起動させる。
       | そうしないと es からの検索も管理者権限が必要になるため。
       | `Everything の起動を hokorobi.ahk から bbKeys.rc へ移動。`:strike: hokorobi.ahk に起動ショートカットを登録（だいぶ前だけど）[2018-02-15]
       | PPx の現行のモジュールからは実行できなくなったので、そちらも使わないように変更。
     - 2019-02-18
   * - `es <http://www.voidtools.com/>`_
     - 1.1.0.10
     - | コマンドラインからの Everything 実行。
       | vim の ctrlp-locate から実行する。
     - 2018-08-16
   * - `NTFSlinksView <http://www.nirsoft.net>`_
     - 1.12
     - ジャンクション、シンボリックリンクなどを表示する。
     - 2013-06-08
   * - `ghq <https://github.com/motemen/ghq>`_
     - v1.0.0
     - | peco と連携して vim プラグイン、golang リポジトリを検索、移動
       | install: go get -u -ldflags -s github.com/motemen/ghq
     - 2020-01-05


.. list-table:: デフラグ
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `Smart Defrag <http://www.iobit.com/>`_
     - 6.2.0
     - | ブートタイムデフラグが出来ると言うことで使ってみたけど、あんまり良いようには思わない。
       | フォルダを指定してデフラグにも使う。
     - 2019-03-30
   * - `Ultra Defrag <http://ultradefrag.sourceforge.net/en/index.html>`_
     - 7.1.0
     - ブートタイムデフラグができるオープンソースデフラグソフト。
     - 2018-10-06


.. list-table:: アーカイバ
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `7-Zip <https://sourceforge.net/projects/sevenzip/files/>`_
     - 19.00 x64
     - 7-zip アーカイバ。
       shell extensionが追加されるので、7zFMを管理者権限で起動してツール - オプション - 7-Zip タブから該当箇所のチェックを外す。
     - 2019-03-08
   * - `Universal Extractor <http://www.legroom.net/modules.php?op=modload&amp;name=Open_Source&amp;file=index&amp;page=software&amp;app=uniextract>`_
     - 1.6.1
     - インストーラ形式のアーカイブからファイルを取り出す。
       色々とアーカイブ用のバイナリを同梱している。
       インストーラなしもあるので好感が持てる。
       DF.INI の [CMD] へはこげな感じで。

       .. code-block:: none

         UniExtract=C:\bin\UniExtract.exe $MF C:\Temp\$X$R

       innounp.exe http://innounp.sourceforge.net/ を 0.39 へ入れ替え。Monkey's Audio 4.12 のインストーラから抽出できなかったので。 [2013-08-13]
     - 2010-05-14
   * - `UNLHA32.DLL <http://www.csdinc.co.jp/archiver/lib/unlha32.html>`_
     - 3.00
     - LZH
     - 2017-05-17
   * - `CAB32.DLL <http://www.madobe.net/archiver/lib/cab32.html>`_
     - 0.98
     - CAB
     - 不明
   * - `TAR32.DLL <http://www.csdinc.co.jp/archiver/lib/tar32.html>`_
     - 2.42
     - tar, gz の展開。
     - 2012-09-30
   * - `TAR64.DLL <http://homepage1.nifty.com/Ayakawa/soft/index.html>`_
     - 2.42.00.02
     - PPx 64 bit で使う 64 bit アーカイバ DLL
     - 2017-02-09
   * - `7-zip64.dll <http://homepage1.nifty.com/Ayakawa/soft/index.html>`_
     - 9.22.00.01
     - PPx 64 bit で使う 64 bit アーカイバ DLL
     - 2014-06-29
   * - `unrar32.dll <http://www.jsdlab.co.jp/~kamei/>`_
     - 0.12 2009/6/24
     - rar
     - 2009-12-16
   * - `unrar.dll <http://www.diana.dti.ne.jp/~winrar/>`_
     - 3.80.100.259
     - rar
     - 2009-03-28
   * - `unrar.dll/unrar64.dll <http://www.rarlab.com/rar_add.htm>`_
     - 4.20
     - rar の展開。使ってる？
       リンク先のページの UnRAR.dll をダウンロード。
     - 2012-08-02
   * - `unrar64j.dll <https://github.com/rururutan/unrar32>`_
     - 0.17
     - rar の展開。64 bit。
     - 2015-07-13


.. list-table:: バージョン管理
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `Git for Windows <https://gitforwindows.org/>`_
     - 2.26.0
     - MSYS の Git は UNIX-like path を要求して https://github.com/rhysd/git-messenger.vim をうまく動かせなかったので MSYS からこちらに切り替えてみる。
       install

       #. .. image:: _image/git_01.png
       #. .. image:: _image/git_02.png
       #. .. image:: _image/git_03.png
       #. .. image:: _image/git_04.png
       #. .. image:: _image/git_05.png

     - 2020-04-12
   * - `Fork <https://git-fork.com/>`_
     - 1.47.0
     - Git の GUI クライアント
       hank の一部を選択すると、そこだけ stage できるのがとても便利。
     - 2020-03-28
   * - `TortoiseHg <https://bitbucket.org/tortoisehg/thg/downloads>`_
     - 4.9.1 x64
     - GUI の Workbench を使う。
       Vim で python27.dll が認識されて gista が動かなくなるのでインストール後にパスから外している。
       5.0.2 で hg-git が動かなかったので 4.9.1 へ戻した。
     - 2019-09-01


システム関係
~~~~~~~~~~~~

.. list-table:: システム関係諸々
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `EjctClse <http://home.att.ne.jp/delta/hrymkt/>`_
     - 1.400
     - CD-ROM ドライブ等の開け閉めを CraftLaunch から。
       FD は無理だった（当たり前）。
       `1.222 では CD-ROM ドライブを開いてくれなくなってしまったので、1.220 に戻す。`:strike: 1.232 で改善されたのかな？
     - 2012-01-28
   * - `ExitWndw <http://home.att.ne.jp/delta/hrymkt/>`_
     - 1.440
     - Windows の終了やログオフを CraftLaunch から。
       1.260 より後は動かない。1.260 は手違いで消してしまった。1.350 も動かなかった。
     - 2019-04-07
   * - `WhatInStartup <http://www.nirsoft.net/utils/what_run_in_startup.html>`_
     - 1.35 x64
     - スタートアップで実行されるプログラムを減らしたり増やしたり。
       StartupRun の後継ソフト。
     - 2013-06-26
   * - `Autoruns <http://technet.microsoft.com/ja-jp/sysinternals/bb963902(en-us).aspx>`_
     - 13.95
     - スタートアップで実行されるプログラムやライブラリを減らしたり増やしたり。
       通常は StartupRun を使ってゴミ掃除にこっちを使う。
     - 2019-06-15
   * - `ConEmu <http://code.google.com/p/conemu-maximus5/>`_
     - 190303
     - シェルラッパー
       Console2 だと外からタブを増やせなかったので、こちらを使っている。
     - 2019-03-03
   * - `startw <http://homepage3.nifty.com/k-takata/mysoft/startw.html>`_
     - 1.09
     - start の GUI 版。
       -wait -min なんかを使っている。
     - 2012-02-28
   * - `RapidEE <http://www.rapidee.com/en/about>`_
     - 9.2 build 937 x64
     - 環境変数を書き換えるソフト。
     - 2018-07-08
   * - `JoyToKey <http://www.vector.co.jp/soft/win95/util/se101657.html>`_
     - 6.3
     - ジョイパッドの操作をキーボードやマウスに割り当てる。
       動画を離れてみながら、操作するときに使っている。
       駄目人間化。
     - 2019-07-24
   * - `nyagos <https://github.com/zetamatta/nyagos/>`_
     - 4.4.5_4 64bit
     - コマンドラインシェル。UNC が扱えるので、Mercurial と一緒に使えないか試してみる。
       最近は PowerShell を使い始めた。 [2016-03-12]
       nyagos に戻ってきた。 [2016-09-08]
     - 2020-03-15
   * - `TaskSchedulerView <http://www.nirsoft.net/utils/task_scheduler_view.html>`_
     - 1.30
     - タスクスケジューラの一覧表示
       不要なタスクを探して無効にしたり。
     - 2017-05-09
   * - `ServiWin <http://www.nirsoft.net/utils/serviwin.html>`_
     - 1.66
     - サービスの一覧。設定変更の差分確認をする際に使用する。
     - 2016-05-01
   * - `RunKan <http://www2.osk.3web.ne.jp/~sm/besrk/besrk.html>`_
     - 1.21
     - コマンドプロンプトなどを管理者権限起動。
     - 2017-08-25
   * - `ClockPod <http://toro.d.dooo.jp/index.html>`_
     - 2.70
     - IME の状態を表示
     - 2018-08-05
   * - `sudo <https://github.com/mattn/sudo>`_
     - 0.0.1
     - sudo
     - 2019-05-23
   * - `フォントインストーラー SAKURA <http://tam.vni.jp/soft/sakura/sakura.html>`_
     - 2.77
     - フォントの情報を表示。Fontlink を設定するため名前を調べた。
     - 2019-06-08
   * - `GeekUninstaller <https://www.geekuninstaller.com/>`_
     - 1.4.7
     - AppStore アプリのアンインストール
     - 2019-09-21

ネットワーク関係
~~~~~~~~~~~~~~~~

.. list-table:: ネットワーク関係諸々
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `Vivaldi <https://vivaldi.com/?lang=ja_JP>`_
     - 2.11.1811.47 x64
     - Chromium 派生 Web ブラウザ。
       Cyberfox から移行してきた。
     - 2020-03-05
   * - `Firefox <http://mozilla.jp/firefox/>`_
     - 73.0
     - Web ブラウザ。
       サブブラウザを Firefox に戻した。 [2018-01-21]
     - 2020-02-12
   * - `WWWC <http://www.nakka.com/>`_
     - 1.1.2
     - Web ページの更新チェック。
     - 2018-10-27
   * - `utorrent <http://www.utorrent.com/>`_
     - 2.2.1.25249
     - 小さな bittorrent クライアント。
       実行すると、問答無用で ``C:\Program Files\uTorrent`` へインストールされていたが、インストール先は選べるようになった。(1.8)
     - 2011-05-06
   * - `FileZilla <http://filezilla.sourceforge.net/>`_
     - 3.44.2 x64
     - FTP クライアント。
       多重接続できるのが嬉しい。
     - 2019-06-29
   * - `twicli <http://www.geocities.co.jp/twicli/>`_
     - 随時
     - JS 製クライアント。
     - 随時
   * - `PuTTY <http://www.chiark.greenend.org.uk/~sgtatham/putty/>`_
     - 0.68
     - `coLinux の Ubuntu へのアクセスで使用。`:strike:
       `Mercurial で Bitbucket へアクセスする際に plink を使用。`:strike:
       Git で Github へアクセスする際に plink を使用。
     - 2017-02-22
   * - `CarotDAV <http://rei.to/carotdav.html>`_
     - 1.14.6
     - WebDAV その他のクライアント。
       SkyDrive へのアクセスに使ってみる。
       ブラウザで SkyDrive にアクセスして CID を取得して、 https://d.docs.live.net/CID を WebDAV の URL として使う。
       userid, password は SkyDrive のもの。
     - 2017-04-29
   * - `Pochitter! <http://www.vector.co.jp/soft/winnt/net/se478199.html>`_
     - 2.6.2
     - Twitter のフォロー状態の確認。あんまりやらない方がいいよな～。
     - 2014-01-25
   * - `Jane Style <http://janesoft.net/janestyle/>`_
     - 4.00
     - 5ch の閲覧
     - 2017-11-09
   * - `Slack <https://slack.com/intl/ja-jp/release-notes/windows>`_
     - 4.00
     - Slack
     - 2019-07-12

テキスト関係
~~~~~~~~~~~~

.. list-table:: テキスト関係諸々
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `CLISM excellent <http://toro.d.dooo.jp/slwin4.html>`_
     - 2.1
     - クリップボードの履歴とったり定型文を挿入したり。
     - 2018-09-29
   * - `CLCL <https://www.nakka.com/soft/clcl/>`_
     - 2.1.0
     - | クリップボードの履歴とったり定型文を挿入したり。
       | 画像も履歴が取れるのが良いところであり、履歴ファイルが膨れ上がるのが気になるところでもある。
     - 2019-12-15
   * - `Sumatra PDF <http://blog.kowalczyk.info/software/sumatrapdf/>`_
     - 3.1.2 x64
     - PDFリーダー。読んだ位置を記憶してくれる。
     - 2016-08-19
   * - `xdoc2txt <http://ebstudio.info/home/xdoc2txt.html>`_
     - 2.19.1 x64
     - 各種バイナリ文書からテキストを抽出する。
       WinMerge, Vim で使用中。
     - 2019-06-29
   * - `XpdfReadre <http://www.xpdfreader.com/>`_
     - 4.0.1
     - PDF からテキストを抽出する pdftotext を使用。
       Vim で使えるかと思ったけど工夫がいりそう。
     - 2019-03-04
   * - `pdfcpu <https://github.com/pdfcpu/pdfcpu>`_
     - 0.3.2
     - PDF の編集をするコマンドラインツール。
     - 2020-01-15
   * - `WinMerge <http://www.geocities.co.jp/SiliconValley-SanJose/8165/winmerge.html>`_
     - 2.16.6+-jp-1 x64
     - | ファイルの比較。
       | 差分内容によって綺麗に色分けしてくれる。
       | こちらは文字コードの自動判別もしてくれる。
       | インストーラを使った場合は、 ``**regsvr32 /u WinMerge\ShellExtension.dll**`` とやったりする。
       | 2.3.3.1-jp-1 からは、設定の「複数のインスタンスを起動しない」を選択することができるようになった。
       | MergePlugins から amb_xdocdiffPlugin.dll 以外を移動。プラグインが自動展開になっているので、色々と入っていると自動で動いてしまう。たまにエラーメッセージが出たりしていた。
       | MergePlugins の中身は移動せず xdocdiffPlugin.dll を追加する運用にしてみる。 [2019-11-02]
     - 2020-03-03
   * - `xdocdiff WinMerge Plugin 64bit <http://crus.mydns.jp/xdocdiffPlugin64/>`_
     - 1.0.6 64bit
     - Winmerge で Word, Excel, PowerPoint, pdf その他の比較が行えるようにするプラグイン。
       zlib.dll に 1.2.4 を使おうとすると xdoc2txt がエラーになるのはちょっと悲しい。
       `オリジナル xdocdiff WinMerge Plugin <http://freemind.s57.xrea.com/xdocdiffPlugin/>`_
     - 2018-10-16
   * - `nkf.exe <http://www.vector.co.jp/soft/win95/util/se295331.html>`_
     - 2.1.1
     - 文字コード変換と改行変換。
     - 2013-03-09
   * - `jj <https://github.com/tidwall/jj>`_
     - 1.2.2
     - JSON パーサ。
       jq より速いらしい。golang 製。
     - 2018-09-22
   * - `Platinum Searcher <https://github.com/monochromegane/the_platinum_searcher>`_
     - 2.1.6
     - 文字コードが色々なファイルをまとめて grep できるソフト。
       jvgrep よりも高速。
     - 2018-07-14
   * - `ripgrep <https://github.com/BurntSushi/ripgrep>`_
     - 11.0.2 x64 msvc
     - | Platinum Searcher よりも高速らしい。
       | 出力の文字コードがファイルの文字コードになるよう。指定できないものだろうか？ [2018-08-04]
       | 文字コードが色々なファイルをまとめて grep はできないので pt に戻った。 [2019-09-11]
     - 2019-08-09
   * - `Sphinx <http://www.sphinx-doc.org/ja/master/index.html>`_
     - 3.0.0
     - reStructuredText を HTML に変換
     - 2020-04-07
   * - `Pandoc <http://johnmacfarlane.net/pandoc/>`_
     - 2.7.3
     - | 文書の変換
       | Sphinx の singlehtml から docx への変換（仮） [2018-06-09]
     - 2019-07-10
   * - `Evernote <https://evernote.com/intl/jp/download>`_
     - 6.17.6.8292
     - Web だけで使っていたけれど一括編集、一括移動などが使えないようなのでアプリをインストール
     - 2019-01-27

.. list-table:: Vim 関係
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `Vim <https://github.com/vim/vim-win32-installer/releases>`_
     - 8.2.0539
     - | デフォルトエディタ。xyzzy から移行。
       | 7.3.1203はうまく動かなかった。Lingrが動かなかったのと、やっぱり色々と問題がありそう。
       | `8.0.0596-20170502 は gvim -c GrepWrap で <t_<fd>`> が入力されたので前のバージョンに戻した。 [2017-05-21]`:strike:
       | `gvim -c GrepWrap で <t_<fd>a> が入力されるが気にせず使っている。 [2017-11-30]`:strike: develop 8.0.1376 で改善されていた。 [2017-12-11]
       | 8.1.1234 から system() の結果がテンポラリファイルから取れない場合があるみたい。dein の自動リキャッシュ（？）時に発生 [2019-05-01]
       | この件 8.1.1350 でも解決しなかったので、自動リキャッシュが発生しないように dein に手を入れた。 [2019-05-19]
     - 2020-04-10
   * - `cmigemo <https://www.kaoriya.net/software/cmigemo/>`_
     - 2011-02-27
     - Vim の easymotion で使用する。
       Kaoriya 版をやめたので migemo.dll は使えなくなったため。
     - 2018-09-29
   * - `lua.dll <http://luabinaries.sourceforge.net/download.html>`_
     - 5.3.4 Win64
     - Vim の +lua を有効にする。
       パスの通った場所に lua53.dll を格納。
     - 2018-08-19

.. list-table:: フォント
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `Cica <https://github.com/miiton/Cica>`_
     - 5.0.1 with emoji
     - Conemu, Paper Plane xUI, Vim で使用。
     - 2019-06-27
   * - `MyricaM <https://myrica.estable.jp/>`_
     - 2.012.20180119
     - Conemu, Paper Plane xUI で使用。
       Cica へ変えてみている。 [2019-02-25]
     - 2018-09-08
   * - `BDF M+ <http://www1.kaoriya.net/>`_
     - 2.2.4p2
     - Paper Plane xUI の等幅フォントに使用。
       Bold, Italic も使えるから替えてみたけど使ってないぞ？
       Cica へ変えてみている。 [2019-02-25]
     - 2010-04-25
   * - `Takaoゴシック <https://launchpad.net/takao-fonts>`_
     - 2015-03-04
     - コマンドプロンプトで使用するフォント。
       2017-11-16 に MyricaM M に変更した。
     - 2015-06-28
   * - `kindlegen <https://www.amazon.com/gp/feature.html?ie=UTF8&docId=1000765211>`_
     - 2.9
     - epub から mobi への変換。
       Calibre も試したけどイマイチ。
     - 2019-04-20

音楽関係
~~~~~~~~

.. list-table:: 音楽関係諸々
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `m4acut <https://github.com/nu774/m4acut>`_
     - 0.1.2
     - M4A の編集。
       Youtube でダウンロードした動画から音声を抽出した後、不要部分を取り除く。
       Free Audio Dub が止まりすぎるので。
     - 2018-04-15
   * - `Audacity <http://audacity.sourceforge.net/>`_
     - 2.2.2
     - OGG Vorbis の編集。
       Lossless で保存できているはず。
     - 2018-04-15
   * - `Free Audio Dub <http://www.dvdvideosoft.com/jp/products/dvd/Free-Audio-Dub.htm>`_
     - 1.7.9.908
     - M4A の編集。
       Youtube でダウンロードした動画から音声を抽出した後、不要部分を取り除く。
     - 2013-01-12


.. list-table:: foobar2000 関係
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `foobar2000 <http://foobar2000.hydrogenaudio.org/>`_
     - 1.5.3
     - BGM として TAK, Ogg Vorbis, MP3, WMA などの再生をさせている。
       プレイリストが削除されることがある。最後の発生は 0.9.5.5。
     - 2020-04-04
   * - `foo_input_tak <http://www.foobar2000.org/components/view/foo_input_tak>`_
     - 0.4.8
     - TAK の再生。
     - 2018-03-01
   * - `Playback statistics <http://www.foobar2000.org/components/view/foo_playcount>`_
     - 3.02
     - 曲の演奏回数を保持する。
       最近演奏した一覧も表示してくれるので履歴の代わりに使っている。
     - 2011-09-28
   * - `Skip Track <http://www.foobar2000.org/components/view/foo_skip>`_
     - 1.9.10
     - 再生をスキップする条件を指定
       聴きたくない曲は rating を 2 にしているので、::

         %rating% IS 2

     - 2018-08-03
   * - `foo_podcatcher <http://www.unkempt.co.uk/fb2k/foo_podcatcher.html>`_
     - 0.25
     - Podcast を聞く。NHKラジオニュースを登録。
     - 2016-03-27


.. list-table:: 作成、編集
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `Exact Audio Copy <http://www.exactaudiocopy.de/>`_
     - 1.5
     - 音楽 CD からの wave 吸出し。
       CDImage を取り出して TAK へ。
       0.95 beta 4 だと TOC の取得はできなくなったんだっけ？
       CCCD などを使うときは前のバージョンを使おう。
     - 2020-02-25
   * - `TAK <http://www.thbeck.de/Tak/Tak.html>`_
     - 2.3.0
     - 圧縮率とエンコード、デコード時間がそこそこに良いロスレスコーデック。
       ロスレスはこれ一本にした。
     - 2013-06-30
   * - `FLAC <http://xiph.org/flac/index.html>`_
     - 1.3.0 RareWares
     - FLAC のエンコード、デコード。
       `FLAC RareWares <http://www.rarewares.org/lossless.php>`_
     - 2013-06-14
   * - `LAME <http://rarewares.org/>`_
     - 3.99.5 64bit Rarewares
     - MP3 でないと駄目なこともあるので。
     - 2012-03-02
   * - `MAC <http://www.monkeysaudio.com/>`_
     - 4.22
     - Monkey's Audio Console Front End.
     - 2017-03-13

画像関係
~~~~~~~~

.. list-table:: 画像関係諸々
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `PNGOUT <http://advsys.net/ken/utils.htm>`_
     - 2010-03-24
     - PNG のサイズを小さくする。
       たいてい OptiPNG よりも縮む。そのかわり時間もかかる。適当に比べてみたら -o7 の 5 倍くらい。
     - 2010-03-27
   * - `pingo <https://css-ig.net/pingo>`_
     - 0.99 RC2
     - PNG のサイズを小さくする。
       PNGOUT ほどは縮まないみたい。（s9 で比べると違うのかも）
       かなり縮むしかなり高速。
     - 2020-04-07
   * - `Graphviz <http://www.graphviz.org/>`_
     - 2.38
     - | グラフ構造の整形、描画、編集システム。
       | 依存関係のある何かを図示するのに使ったり。
       | 2.30 を msi でインストールしたらシステムの PATH にパスが追加されたので削除した。
       | zip を展開しただけだと dot.exe の実行で以下のエラーが表示された。

       .. code-block:: none

         (dot.exe:3928): Pango-WARNING **: `/target/lib/pango/1.6.0/modules/pango-basic-win32.dll': 指定されたモジュールが見つかりません。

     - 2019-08-05
   * - `AzPainter <http://hp.vector.co.jp/authors/VA033749/>`_
     - 2.09
     - シンプルで使いやすいような気がするペイントソフト。
     - 2010-06-20
   * - `buff <http://www.geocities.co.jp/SiliconValley/1367/>`_
     - 1.08
     - JPEG の無劣化トリミング。
     - 2011-01-11
   * - `Jcropper <http://www.vieas.com/>`_
     - 1.2.50
     - JPEG の無劣化トリミング。
     - 2015-04-23
   * - `jpegcrop <http://sylvana.net/jpegcrop/>`_
     - 2012
     - JPEG の無劣化トリミング、回転他。
     - 2012-05-12
   * - `azure <http://www.geocities.co.jp/SiliconValley/1367/>`_
     - 1.16
     - JPEG の無劣化回転。
       ファイルによっては「ストリームが読み込めません」と出るので JPEG Lossless Rotator も使う。
     - 2011-01-11
   * - `JPEG Lossless Rotator <http://annystudio.com/software/jpeglosslessrotator/>`_
     - 9.1
     - JPEG の無劣化回転。
       azure で回転できなかったファイルが回転できた。
       Ver 9.1 64 bit は起動しなかった。
     - 2013-05-03
   * - `jpegoptim <http://sourceforge.net/projects/jpegoptim/>`_
     - 1.30
     - メタデータ削除。carmine よりも少しだけ縮むみたい。
     - 2014-04-27
   * - `carmine <http://www.geocities.co.jp/SiliconValley/1367/>`_
     - 1.05
     - JPEG のハフマンテーブル最適化、exif データ削除。
     - 2012-01-28
   * - `Ralpha <http://nilposoft.info/ralpha/>`_
     - 140329
     - 画像の一括リサイズに使用。比較的高速なようなので。
     - 2014-04-04
   * - `Imagemagick <http://www.imagemagick.org/script/index.php>`_
     - 7.0.7-11-portable-Q16-x64
     - | 画像の変換や切り出し。
       | 001.png の x=206, y=0 の位置から幅 1508 ピクセル、高さ 1080 ピクセルを切り出して crop/001.png へ保存。

       .. code-block:: none

         convert.exe -crop 1508x1080+206+0 001.png crop/001.png

       | カレントディレクトリ内の png を x=206, y=0 の位置から幅 1508 ピクセル、高さ 1080 ピクセルを切り出して上書き保存。

       .. code-block:: none

         mogrify.exe -crop 1508x1080+206+0 *.png

       | 6.8.8-4-Q16-x64-dll などだと dll も必要だったが、static なら不要みたい。
       | `cmd へ convert.exe, mogrify.exe だけを格納。`:strike:
       | 7.0.7-11 では magic.xml が必要だと怒られたので普通にパスを通した。
     - 2017-12-01
   * - `WinShot <http://www.woodybells.com/winshot.html>`_
     - 1.53a
     - スクリーンショットを画像ファイルとして保存。
       Lightscreen を使ってみたけど、保存するまでに時間がかかる気がするのでやめ。
     - 2016-04-17


.. list-table:: 表示
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `MassiGra <http://www.vector.co.jp/soft/win95/art/se400675.html>`_
     - 0.45
     - マンガミーヤは公開中止されてしまったので、別のを探さないとなぁということで見つけた。
       zip ファイルを扱うために `axzipx.spi <http://www.geocities.jp/gis2lel/sw/index.html>`_ をインストール。
     - 2013-12-21
   * - `IrfanView <http://www.irfanview.com/>`_
     - 4.54 64bit
     - 軽いグラフィックビューア。
       プラグインで色々なファイル形式に対応。
       `NKV よりもマシだけれど縮小が綺麗じゃない。`:strike: バージョン 4.00 で View - Display options (window mode) - Use "Resample" for fitting (better quality) を選択すると綺麗になった。前のバージョンでも設定していれば綺麗になったのかな？。
       `日本語モジュール <http://park15.wakwak.com/~yu-ki/>`_ 、 `日本語版 <http://www8.plala.or.jp/kusutaku/>`_
       最近は MassiGra しか使っていないけれど、サブとして入れている。
     - 2019-12-25
   * - `PlantUML <http://ja.plantuml.com/>`_
     - 1.2020.6
     - シーケンス図とかを描く。
     - 2020-04-06


.. list-table:: Susie Plug-in
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `ifgif.spi m0.1 <http://mij4x.datacompression.jp/text/ifgif_cmp.html>`_
     - ifgif.spi m0.1
     - 標準の ifgif.spi よりも高速で、ちゃんと画像を表示してくれるみたいなので変更。
     - 2005-04-17
   * - `JPEG-turbo Susie Plug-in <http://toro.d.dooo.jp/slplugin.html#ifjpegt>`_
     - 1.05
     - PPx で JPEG を表示。
       WIC を使うように変更 [2013-03-30]
       これを使うように変更。輪郭がくっきりしたイラストっぽい画像だと ifjpegt が圧倒的に早く、1Mbyte超のデジカメ画像だと iftwic がすこし早い傾向 [2017-09-02]
     - 2018-11-15
   * - `WIC Susie Plug-in <http://toro.d.dooo.jp/slplugin.html#iftwic>`_
     - 1.7
     - PPx で GIF 以外を表示。
     - 2018-03-04
   * - `spibench <http://hp.vector.co.jp/authors/VA010446/toolbox2/index.html#spibench>`_
     - 2004-10-15
     - Susie Plug-in のベンチマーク。
     - 2004-10-15

動画関係
~~~~~~~~

.. list-table:: 動画関係諸々
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `HugFlash <http://www.paw.hi-ho.ne.jp/milbesos/>`_
     - 2.9
     - フラッシュファイルからデータを抽出する。
       swf よりも flv に使うことが多い。
     - 2013-05-20
   * - `Nautilus <http://blog.x-row.net/?p=4997>`_
     - 0.0.1.0
     - デスクトップキャプチャ
     - 2014-07-30
   * - `LosslessCut <https://github.com/mifi/lossless-cut>`_
     - 3.0.1
     - Youtube の動画の不要部分を無劣化で取り除く。
       シンプルなので Avidemux から移行。
     - 2020-02-17
   * - `ffmpeg <https://ffmpeg.zeranoe.com/builds/>`_
     - 4.2
     - 音声の抜き出しとか。
       `バイナリ配布先1 <http://oss.netfarm.it/mplayer-win32.php>`_

       - 動画から音声の抜き出し: ``ffmpeg -i input.mkv -acodec copy output.???`` 音声の拡張子は ``ffmpeg -i input.mkv`` の結果から判断する。
       - 音声の修正？: ``ffmpeg -i input.ogg -acodec copy output.ogg``

     - 2019-08-09


.. list-table:: 動画再生
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `Media Player Classic <http://sourceforge.net/projects/guliverkli>`_
     - Home Cinema x64 1.7.10 / x86 1.6.5.6366
     - 各種コーデックを入れて動画を再生。
       RealMedia, QuickTime，Flash なんかも再生できる。
       URL を入れても大丈夫。
       日本語のタグを見られるように、極力日本語版を入れようと思う。
       `Media Player Classic - Home Cinema <http://mpc-hc.sourceforge.net/>`_ ,
       `henry <http://henry.fushizen.eu/>`_ ,
       `ロシア <http://www.xvidvideo.ru/>`_ ,
       Home Cinema x64 1.5.3.3704 henry は再生が遅くなったりしたので使うのやめ。
     - 2016-05-07 / 2012-12-17
   * - `mpv <https://sourceforge.net/projects/mpv-player-windows/files/>`_
     - 0.32.0+ (77a74d9)
     - | 動画再生。mplayer から切り替え。
       | 2016-11-20 は WMV の再生がおかしかった。映像が出ない。 [2016-12-04]
       | バイナリ取得サイトを変更 http://mpv.srsfckn.biz/ -> https://sourceforge.net/projects/mpv-player-windows/files/ [2018-07-24]
     - 2020-02-07
   * - `youtube-dl <https://rg3.github.io/youtube-dl/>`_
     - 2020.03.24
     - youtube を mpv で再生。
       youtube の動画を DL。
       Microsoft Visual C++ 2010 Redistributable Package (x86) （not x64）が必要。
     - 2020-04-12
   * - `MPC-BE <https://sourceforge.net/projects/mpcbe/>`_
     - 1.5.1 x64
     - MPCHC の改訂版。
     - 2017-10-14
   * - `VLC media player <http://www.videolan.org/>`_
     - 2.1.0
     - | DVD とか色々と再生できるプレイヤ。
       | `0.9.2 Advanced Option を使うと、終了時にエラーが出て、設定の保存が出来ない様子。`:strike: 0.9.4 で改善された様子。
       | `MPEG-TSの字幕表示に対応 <https://skydrive.live.com/?cid=2DAB0D8D07FA4EBF&id=2DAB0D8D07FA4EBF%21473>`_
     - 2013-09-26
   * - `ffdshow <http://sourceforge.net/projects/ffdshow/>`_
     - rev4531_20140628_x64
     - DivX や Xvid を軽快に再生。
       `ffdshow tryouts <http://ffdshow-tryout.sourceforge.net/>`_

       - AC3 の音声がやけに小さいというのはバグ（？）らしい。Mixer をオンにすると解消されるとか。
       - DeBand をオンにしてグラデーションの縞々を綺麗に表示。
       - ffdshow-2546-gcc4.0.3-sse2-x264.nl は mkv 再生時にエラーが出たので sse を使っていた。

     - 2014-06-30

プログラミング
~~~~~~~~~~~~~~

.. list-table:: プログラミング諸々
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `Python <http://www.python.org/>`_
     - 64 bit 3.8.1
     - | メインの LL。
       | `Vim プラグインの Gista は 2.7 が入っていないと保存時にエラーになる。なぜだ？ [2017-05-14]`:strike:
       | TortoiseHg の python27.dll が Python 2.7 として認識されていた。TortoiseHg のパスをはずした。 [2018-02-03]
       | neovim が pynvim になって Windows の 3.7 でも使えるようになったので 3.6 は削除。 [2019-02-23]
       | 会社の PC が 64 bit になったので 32 bit は削除。 [2019-04-21]
     - 2020-02-01
   * - `go <http://golang.org/>`_
     - 1.14.2 64bit
     - go
     - 2020-04-09
   * - `goimports <https://github.com/golang/tools/tree/master/cmd/goimports>`_
     - 2019-12-17 621d4eef
     - Fast gofmt
       Install: go get -u -ldflags -s -v golang.org/x/tools/cmd/goimports
     - 2020-01-03
   * - `gopls <https://github.com/golang/tools/tree/master/gopls>`_
     - v0.1.7
     - | Vim + coc.nvim から呼び出して使用。
       | Install: GO111MODULE=on go get -ldflags -s golang.org/x/tools/gopls@latest
       | v0.2* はうまく動かなかった。 [2019-12-08]
     - 2019-12-08
   * - `Node.js <https://nodejs.org/ja/>`_
     - 10.15.3 LTS
     - textlint や plantuml-syntax-test で使用。
     - 2019-04-27
   * - `universal ctags <https://github.com/universal-ctags/ctags-win32>`_
     - 2019-12-12/f42b573f
     - tags ファイルを作成して Vim で使用
     - 2019-12-13
   * - `efm-langserver <https://github.com/mattn/efm-langserver>`_
     - 2020-03-11 90adbf
     - Vim で vint を実行
     - 2020-03-15


辞書
~~~~

.. list-table:: 辞書
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `PDIC/Unicode <http://homepage3.nifty.com/TaN/>`_
     - 5.10.70
     - `英辞郎2 <http://www.amazon.co.jp/dp/4757408382/>`_ を使って英語辞書として使っている。
       PDIC/Unicode の発音記号フォントは、 `Doulos SIL Font Home <http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&amp;item_id=DoulosSILfont>`_ を使う。
     - 2020-01-03
   * - `EBWin <http://www31.ocn.ne.jp/~h_ishida/EBPocket.html>`_
     - 4.7.7 64bit / 3.06 Unicode
     - EPWING などの辞書データから辞書引きできるソフト。
       今は広辞苑のために使っている。
     - 2020-03-04 / 2012-05-18
   * - `Lingoes <http://www.lingoes.net/en/>`_
     - 2.9.1
     - ポップアップ辞書。
       英辞郎とか明鏡とか、まずいんじゃないかと思うデータも無料で手に入る。
     - 2013-06-08

kobo
~~~~~~

.. list-table:: その他
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `AozoraEpub3 <http://www18.atwiki.jp/hmdev/pages/21.html>`_
     - 1.1.0b46
     - 青空文庫形式を ePub3 へ変換。kobo 用。
     - 2016-11-23
   * - `ChainLP <http://no722.cocolog-nifty.com/blog/>`_
     - 0.40-17
     - 画像 zip を変換。kobo 用。
     - 2013-02-05


その他
~~~~~~

.. list-table:: その他
   :header-rows: 1
   :widths: 15 10 60 10

   * - Name
     - Version
     - Comment
     - Update
   * - `USBDeview <http://www.nirsoft.net/utils/usb_devices_view.html>`_
     - 2.71 x64
     - 接続している USB デバイスを表示する（他機能もあり）ソフト。
       コマンドラインでシリアルナンバーを指定して、デバイスの取り外しなどを行うために使っている。
       USBDeview.exe /stop_by_serial hoge
     - 2017-06-08
   * - `USBremove <http://home.att.ne.jp/delta/hrymkt/USBremove.html>`_
     - 1.120
     - 接続している USB デバイスを取り外せるようにする。
     - 2013-06-15
   * - `CraftLaunch <http://sites.google.com/site/craftware/>`_
     - 2.08
     - ソフトの起動や操作。
     -
   * - `KeePassXC <https://keepassxc.org/>`_
     - 2.5.3 64bit Portable
     - オープンソースでクロスプラットフォームのパスワード管理ソフト。
       KeePass のバージョン 2 への移行をしていなかったけど、こちらにしてみた。
     - 2020-01-07
   * - `家計簿，出納簿ひかる <http://www.kensoft.co.jp/>`_
     - 9.60
     - 家計簿。
       たまにグラフ表示をして生活を振り返ってみる。
     - 2017-12-13
   * - `JRE <http://www.oracle.com/technetwork/java/javase/downloads/index.html>`_
     - 1.8.0.241 32bit, 64bit
     - Java のランタイム。
       インストール後に、コントロールパネルから Java を開いて、「アップデート」-「アップデートを自動的にチェック」のチェックを外す。
       ``HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Run`` に追加される ``"C:\Program Files\Java\jre6\bin\jusched.exe"`` を削除。
     - 2020-02-01
   * - `Freeplane <http://sourceforge.net/apps/mantisbt/freeplane/my_view_page.php>`_
     - 1.8.1 pre06
     - マインドマップを書くためのツール。
       FreeMind の改造版。
       いくつか嬉しい機能がある。
     - 2020-03-22
   * - `conim <http://site-clue.statice.jp/>`_
     - 3.00
     - 16 進表記の色を作成したり、画面から取ってきたり。
     - 2006-02-19
   * - `Stud_PE <http://www.cgsoftlabs.ro/studpe.html>`_
     - 2.6.1.0
     - 実行ファイルの中身を覗いてみる。
     - 2013-10-04
   * - `Process Monitor <http://technet.microsoft.com/ja-jp/sysinternals/bb896645(en-us).aspx>`_
     - 3.50
     - ファイルシステム、レジストリ、プロセス（スレッド）のモニタリングソフト
     - 2018-02-18
   * - `Process Explorer <http://technet.microsoft.com/ja-jp/sysinternals/bb896653(en-us).aspx>`_
     - 16.30
     - プロセスの詳細な情報を表示することができるタスクマネージャ。
       メニューの Find → Find Handle or DLL でプロセスが掴んでいる DLL を探すようなことができる。
     - 2019-09-07
   * - `LibreOffice <http://www.libreoffice.org/>`_
     - 6.2.2 64bit
     - オープンソースのオフィススイート。
       OOo からフォーク。
     - 2019-03-24
   * - `ImgBurn <http://www.imgburn.com/>`_
     - 2.5.8.0
     - CD/DVD 作成。
       `日本語ランゲージファイル <http://www.nihongoka.com/jpatch_main/imgburn>`_
     - 2013-06-18
   * - `less <http://www.vesta.dti.ne.jp/~tsato/software.html#less>`_
     - 458 ckw対策済み x64
     - 日本語も表示できる less。
       UNICODE は駄目かな？
       -> `RuRuRu さんバージョン <http://www.vesta.dti.ne.jp/~tsato/software.html#less>`_ なら set LESSCHARSET=utf-8 で表示できた。
       hg で使うなら、日本語での設定ははやめないといけないな。hg 本体の表示が shift-jis になるから、こちらが文字化けしてしまう。
     - 2014-11-23
   * - `VirtualBox <http://www.virtualbox.org/>`_
     - 5.2.8
     - 仮想環境を提供するアプリケーション。
       Ubuntu を GUI で使って、たまに遊ぶ程度。
       1.6.0 からは Windows XP 以上でないとインストールできなくなった。
       回避方法もあるけれど、正常動作するかは未検証。
       旧バージョンをアンインストールしてからインストールしないとエラーになることが多い。
       Docker Toolbox と一緒にインストール。
     - 2018-05-20
   * - `CrystalDiskMark <http://crystalmark.info/>`_
     - 3.0.1
     - HDD の S.M.A.R.T の情報などを表示してくれる。
     - 2010-12-27
   * - `OpenedFilesView <http://www.nirsoft.net/>`_
     - 1.45
     - プロセスが開いているファイルのリストを表示する。
     - 2009-09-24
   * - `ShellExView <http://www.nirsoft.net/>`_
     - 2.00
     - Shell Extension の一覧を表示したり、削除したり。
     - 2019-03-08
   * - `TkSQLite <http://reddog.s35.xrea.com/wiki/TkSQLite.html>`_
     - 0.5.7
     - SQLite の GUI ツール。
     - 2008-12-07
   * - `Disk Usage <http://technet.microsoft.com/ja-jp/sysinternals/bb896651(en-us).aspx>`_
     - 1.33
     - ディスク使用量の一覧表示。
     - 2008-12-11
   * - `WinDirStat <http://windirstat.info/>`_
     - 1.1.2.80
     - ディスク使用量をグラフィカルに表示。
       比較対象を忘れてしまったけれど、比較的高速に感じた。
     - 2009-11-01
   * - `FullEventLogView <http://www.nirsoft.net/>`_
     - 1.32 x64
     - イベントビューア代替。
     - 2019-01-27
   * - `MultiPyAlarm <https://bitbucket.org/hokorobi/multipyalarm>`_
     - 3c190e2
     - 複数のタイマーを登録したくなったので自作。
       コマンドラインオプションで時間が設定できるのが嬉しい。
       bktimer から変更。
     - 2019-01-07
   * - `Scriptac <http://home.att.ne.jp/delta/hrymkt/>`_
     - 1.050
     - スタートアップの実行に使用。
     - 2011-03-07
   * - `AutoHotkey <http://www.autohotkey.net/~Lexikos/AutoHotkey_L/>`_
     - 1.1.31.0 x64
     - キーの入れ替えに使用。

       管理者権限で実行されるプログラム（主に Everything）でも使えるように、AutoHotkey も管理者権限で実行する。
       タスクスケジューラに AutoHotkey のタスクを登録。

       * 「全般 - セキュリティオプション - 最上位の特権で実行する」にチェック
       * 「トリガー」は無し
       * 「操作 - 設定 - プログラム/スクリプト」に AutoHotkey のパス
       * 「操作 - 設定 - 引数の追加」に実行したいスクリプトファイル
       * 「設定 - タスクを停止するまでの時間」からチェックを外す。常駐させるため。

       このままだと優先度が低くなっているので、エクスポートして Priority を 6 に変更。
       その後、インポート。
       効果は不明。

       PC 起動時に実行::

         schtasks.exe /Run /TN AutoHotkey

       | 1.1.21 系に変更してみた。大丈夫かな？ [2015-04-23]
       | 1.1.27.00 はやたらと落ちるので 1.1.26.01 に戻した。Windows Update が原因の可能性もあるので様子見。[2017-12-27]
       | 1.1.27.02 でマシになったみたい [2018-01-07]
     - 2019-10-22
   * - `Stickies <http://www.zhornsoftware.co.uk/stickies/>`_
     - 7.1e
     - 思いついたことを書き込んで画面に貼り付ける付箋。
     - 2012-11-16
   * - `EasyMCC <http://bluesky23.yu-nagi.com/EasyMCChtml>`_
     - 132
     - モニタのハードボタンで行う設定をソフトで変更できる。
       輝度、コントラスト、青ゲインを下げたり（ブルーライトカット）
     - 2016-05-01
   * - `Tascher <http://www16.atpages.jp/rayna/index.html>`_
     - 1.62
     - タスクの切り替え。インクリメンタルサーチと絞込が一件になったら自動切り替えしてくれる機能が素晴らしい。
       Migemo 対応！ 1.5.6
     - 2017-03-27
   * - `MSYS2 <https://msys2.github.io/>`_
     - msys2-i686-20150512.exe
     - | Git とか unix ツールとか
       | ``ssh -p portNumber username@hostname``
       | ``pacman -Syu``
       | Git for Windows だけで満足できるか試してみる [2020-04-12]
     - 2015-07-13
   * - `peco <https://github.com/peco/peco>`_
     - 0.5.7
     - PPx のタブ切り替えのために 使用。
       Install: go get -u -ldflags -s github.com/peco/peco/cmd/peco [2018-03-18]
       Defender の例外にも登録。
     - 2020-01-11
   * - `Docker Toolbox <https://www.docker.com/products/docker-toolbox>`_
     - 17.03.1-ce
     - Docker
     - 2017-04-08
   * - `RelaxTools Addin <https://software.opensquare.net/relaxtools/>`_
     - 4.25.2
     - Excel の操作を便利にしてくれるアドイン
     - 2017-04-20

削除済み
--------

.. list-table:: 未分類
   :header-rows: 1
   :widths: 15 10 30 30 10

   * - Name
     - Version
     - Comment
     - Delete reason
     - Update
   * - `PyQt <http://www.riverbankcomputing.co.uk/>`_
     - 5.0.1
     - Python で GUI
     - WxPython が Python3 で使えるようになったので Qt はやめ。
     - 2013-08-31
   * - `XnView <http://www.xnview.com/en/index.html>`_
     - 2.12
     - 多機能なグラフィックビューア。
       nConvert で PDF を画像にしてクリップボードへ送って、それを PPv から参照。
     - PDF のプレビューはそんなにいらない。
     - 2013-11-29
   * - `GIMP <http://www.gimp.org/index.html>`_
     - 2.6.11
     - GIMP is the GNU image manipulation program.
       Photoshop の操作感に似せた `GIMPshop <http://www.gimpshop.com/>`_ もある。
       `Windows バイナリ (sourceforge.net) <https://sourceforge.net/projects/gimp-win/>`_ , `gimp-win <http://gimp-win.sourceforge.net/>`_ 。
     - 使いこなせなかった。
     - 2010-10-09
   * - `Inkscape <http://www.inkscape.org/>`_
     - 0.48.4-1
     - SVG エディタ。
     - 使いこなせなかった。
     - 2012-12-20
   * - `ロック音MT <http://hp.vector.co.jp/authors/VA014492/>`_
     - 1.15
     - | ラジオやミニコンポからの録音に使っている。
       | 予約録音を重宝している。
       | 録音後に mono_resample.bat "%a" というコマンドを実行するように設定している。
       | mono_resample.bat では、waveflt2 でモノラル化、24 bit 化、DC オフセット補正、50 Hz ~ 15 kHz のバンドパスフィルタ処理をした後に、r8brain で 32 kHz にリサンプリングしている。

       .. code-block:: bat

         @echo off
         if "%1" == "" (goto USAGE)
         :ENC
         if not exist "%1" (goto SHIFT)
         D:\OLS\Music\waveflt2\waveflt2.exe -autoofs 3060 -mix 1.0 -fir_bpf 50 15000^
          -bit24 "%1" "%~dpn1_a%~x1"
         D:\OLS\Music\r8brain\r8b_console.exe "%~dpn1_a%~x1" "%~dpn1_b%~x1" 32000 32000^
          24 4
         :SHIFT
         shift /1
         if "%1" == "" (goto EOF) else (goto ENC)
         :USAGE
         echo USAGE: %0 files
         :EOF

     - ラジオを録音することがなくなった
     - 2010-10-26
   * - `WAVEFLT2 <http://hp.vector.co.jp/authors/VA014492/>`_
     - 1.16
     - ラジオドラマのモノラル化、24 bit 化、DC オフセット補正、50 Hz ~ 15 kHz のバンドパスフィルタをかけるのに使用している。
     - ラジオを録音することがなくなった
     - 2007-11-16
   * - `r8brain <http://www.voxengo.com/product/r8brain/>`_
     - 1.9
     - Wave のサンプリング周波数を変換する。
       FM ラジオは 32 kHz で十分だよねということで変換したりする。

       .. code-block:: none

         r8b_console.exe hoge.wav fuga.wav 32000 32000 24 4

       適当に b2e ファイルを作った。（mono_resample.bat を使うようになったので、こちらは使っていない）

       .. code-block:: none

         load:
          (name D:\OLS\Music\r8brain\r8b_console.exe)
          (type wav 24bit_32kHz_wav)

         encode1:
          (cmd (list) (arc_24b32k.wav) 32000 32000 24 4)

     - ラジオを録音することがなくなった
     - 2010-10-26
   * - `WaveGain <http://www.rarewares.org/others.html>`_
     - 1.2.8
     - wave ファイルのリプレイゲインを計算。
       `DC Offset なんかも検出してくれるので、SoundEngine で DC 成分調整を忘れていることがわかったりする。`:strike: 今は mono_resample.bat を使うようになったので DC Offset は気にしていない。
       1.2.7 も出たけれど、自分には必要のない機能追加みたいな。
     - ラジオを録音することがなくなった
     - 2009-04-26
   * - `STEP <http://www22.atpages.jp/~haseta2003/cgi-bin/index.cgi>`_
     - 1.03b7
     - MP3, Ogg Vorbis のタグ編集。
       SuperTagEditor 改造版からファイルタイプ特有の機能をプラグイン化したモノ。
       `STEP_M <http://mimumimu.net/software/#STEP_M>`_
     - 最近は foobaro2000 のタグ編集で十分
     - 2010-09-26
   * - `oggdropXPd <http://www.rarewares.org/ogg.html>`_
     - 1.9.0 aoTuV b5.5 P4
     - ファイルをドロップすることで Ogg Vorbis へ簡単エンコード。
       ラジオドラマの wave を ogg へ変換するために使用している。
     - venc へ移行。
     - 2008-04-22
   * - `oggenc2 <http://www.rarewares.org/ogg-oggenc.php>`_
     - Rarewares 2.87 using aoTuVb6.03 (Lancer Builds) SSE3 x64
     - Ogg Vorbis へのエンコード。
       ファイル名を oggenc.exe に変更して foobar2000 の Convert で使用。
       2013-06-16 Lancer を見付けたので戻ってきた。
     - venc へ移行。
     - 2013-06-16
   * - `venc <http://www.geocities.jp/aoyoume/aotuv/>`_
     - aoTuV b6.03
     - Ogg Vorbis のエンコード。
       oggenc.exe とは別物。
     - 2013-06-16 oggenc へ。
     - 2011-04-27
   * - `OggVorbis Packet Tool's <http://hp.vector.co.jp/authors/VA027311/>`_
     - 06/11/18-R5
     - OggVorbis を劣化無しで編集するソフト集。
       ラジオドラマのサンプリングレートを変更して、ゲインを調節して、エンコードしたけれど、頭とお尻を切り忘れて、かつソースも削除してしまったので使った。
     - 最近、OggVorbis の編集はしない
     - 2007-06-27
   * - `Nero Digital Audio Reference MPEG-4 & 3GPP Audio Encoder <http://www.nero.com/ena/downloads-nerodigital-nero-aac-codec.php>`_ ,
       `他の DL サイト <http://ftp6.nero.com/tools/>`_
     - 1.3.3.0
     - 私的利用目的ならフリーの AAC エンコーダ。

       .. code-block:: none

         neroAacEnc.exe -q 0.4 -if input.wav -of output.m4a

     - AAC を使わない。
     - 2008-09-24
   * - `PMPlib (EasyPMP) <http://pmplib.sourceforge.net/>`_
     - 0.12 alpha
     - 純正の無駄な重さが好きになれないので、iRiver H10Jr. のデータベース更新に使っている。
       ただファームウェアのアップデートは iRiver Plus 2 を使ってしまう。
       使い方はこんな感じで。

       .. code-block:: none

        D:\OLS\Music\easypmp\easypmp_cui.exe -c H:\
     - Ogg を使わない
     - 2006-08-01

   * - Mp3Tag
     - 2.50
     - 音楽ファイルのタグ打ち。ちょっとタグを見たいときに。
       `日本語化ファイル <http://www.nihongoka.com/jpatch_main/mp3tag/>`_
     - foobar2000 で十分
     - 2012-03-14
   * - `UniteTTC <http://yozvox.web.infoseek.co.jp/>`_
     - 2008-06-08
     - 複数の TTF を TTC にまとめたり、TTC を複数の TTF にばらしたり。
     - 使う機会がなくなった。
     - 2008-07-04
   * - `WinFontsView <http://www.nirsoft.net>`_
     - 1.05
     - 任意の文字列でフォントを表示する。
     - 使う機会がなくなった。
     - 2009-08-23
   * - `Y.OzFont TTF JIS X 0213:2004 (YOzR04N) <http://yozvox.web.infoseek.co.jp/>`_
     - 12.14
     - smoopy で小説を読む際に使用。
     - 使う機会がなくなった。
     - 2011-01-04
   * - `SH G30 <http://osakattf.hp.infoseek.co.jp/>`_
     - 不明
     - 可読性に優れたフォント。
       ライセンスは不明。
     - 使う機会がなくなった。
     - 2010-10-26
   * - `Andale Mono <http://sourceforge.net/project/showfiles.php?group_id=34153&amp;package_id=56408>`_
     - 不明
     - 0 と O、I と l と 1 が判読しやすいフォント。
     - 使う機会がなくなった。
     - 2010-10-26
   * - `P4Merge <http://www.perforce.com/perforce/downloads/index.html>`_
     - 2010.1.26.5509
     - | diff, merge ツール。
       | diff は個別ファイルでしか使えないので、merge に特化して使うのが良さそう。
       | msysgit での設定

       .. code-block:: none

         git config --global merge.tool p4merge
         git config --global mergetool.p4merge.cmd 'p4merge.exe \"$BASE\" \"$LOCAL\" \"$REMOTE\" \"$MERGED\"'

     - WinMerge を使っている。
     - 2010-10-09
   * - `KDiff3 <http://kdiff3.sourceforge.net/>`_
     - 0.9.96a
     - diff, merge ツール。
       TortoiseHg 同梱の kdiff3 を使うようにした。
       レジストリ ``HKEY_CURRENT_USER\Software\KDiff3`` には存在しないパスが指定されているけれど、ちゃんと TortoiseHg 同梱の kdiff3 が起動するな。
       どうなっているんだろう？
     - WinMerge を使っている。
     - 2012-11-19
   * - `ffphrase <http://www4.atwiki.jp/shouhmisc/>`_
     - 1.4
     - マクロを使える定型文をメニューから貼り付け
     - 使う機会がなくなった。
     - 2013-03-09
   * - `PDFsam <http://www.pdfsam.org/>`_
     - 2.2.2
     - PDF の分割・結合
     - 使う機会がなくなった。
     - 2012-12-08
   * - `TxtMiru <https://sites.google.com/site/gearsns/>`_
     - 2.0.3.3
     - 小説読むのに。文字のアウトライン補正が良いかも。
     - 使う機会がなくなった。
     - 2012-06-12
   * - `smoopy <http://site-clue.statice.jp/>`_
     - 1.62
     - 小説読むのに。文字のアウトライン補正が良い。
       UPX 圧縮のせいで BitDefender Version: 7.11972 で Generic.Malware と誤認されるみたい。（UPX を元に戻したら大丈夫だった）
     - 使う機会がなくなった。
     - 2007-03-21
   * - `ArisuViewer <http://www.vector.co.jp/soft/win95/util/se433856.html>`_
     - 1.2.0.0
     - 小説読むのに。
       最初の設定に戸惑った。
       悪くはないけれど smoopy とどちらがよいかな？　甲乙つけ難い。
     - 使う機会がなくなった。
     - 2007-12-03
   * - `oedit <http://www.hi-ho.ne.jp/a_ogawa/oedit/>`_
     - 7.5.2.4
     - msysgit のコミットを UTF8 で入力するために指定。
     - 使う機会がなくなった。
     - 2012-11-03
   * - `GetASFStream <http://tetora.orz.ne.jp/>`_
     - 2.3.0.0c
     - ストリーミングデータのダウンロード。
     - 2009-09-15
     - 使う機会がなくなった。
   * - `htmllint <http://htmllint.itc.keio.ac.jp/htmllint/htmllint.html>`_
     - htmllint.pm 3.36
     - HTML の構文チェックに。
       xyzzy (2004-07-09) から実行。
     - 使う機会がなくなった。
     - 2006-04-07
   * - `Privoxy <http://www.privoxy.org/>`_
     - 3.0.24
     - Web ページの広告を削除したり，ポップアップを抑止したり。
     - 使う機会がなくなった。
     - 2016-02-27
   * - `MyDefrag <http://www.mydefrag.com/>`_
     - 4.3.1
     - JkDefrag の後継。
       スクリプトを記述できる。
     - SSD になったので使わなくなった。
     - 2010-11-14
   * - `Ultimate defrag <http://www.disktrix.com/UDFree.htm>`_
     - 1.72
     - デフラグ。
     - SSD になったので使わなくなった。
     - 2012-07-04
   * - `Fire File Copy <http://www.k3.dion.ne.jp/~kitt/pc/sw/ffc/>`_
     - 4.9.1 u
     - HDD をガリガリ言わせずにでっかいファイルをコピー。
     - FastCopy を使う。といってもほどんと使わない。
     - 2009-08-01
   * - `Miranda-IM <http://www.miranda-im.org/>`_
     - 0.8.27 unicode
     - MSN メッセンジャー，Yahoo メッセンジャーなどとメッセージをやりとり。
     - 使う機会がなくなった。
     - 2010-07-02
   * - `Atomic <http://addons.miranda-im.org/details.php?id=194>`_
     - 0.6.0.0
     - SNTP サーバから時間を取得。
       ntp.nict.jp
       `NTPサーバのリスト <http://yotaro.bird.to/feedback/misc/NTP_list.html>`_ から tracert.exe で適当に選んで。
       ntp1.jst.mfeed.ad.jp (210.173.160.27)
       ntp2.jst.mfeed.ad.jp (210.173.160.57)
       ntp3.jst.mfeed.ad.jp (210.173.160.87)
     - 使う機会がなくなった。
     - 2004-12-04
   * - `NewXstatusNotify YM (Unicode) <http://addons.miranda-im.org/details.php?id=4341>`_
     - 1.4.0.3
     - NewStatusNotify に機能追加したもの。
     - 使う機会がなくなった。
     - 2010-10-27
   * - `NewEventNotify <http://addons.miranda-im.org/details.php?id=3637>`_
     - 0.2.2.3
     -
     - 使う機会がなくなった。
     - 2009-07-02
   * - `YAPP <http://addons.miranda-im.org/details.php?id=2759>`_
     - 0.5.0.9
     - ポップアップで情報表示。
       アニメーションが格好良かったので換えてみた……でも、切ってしまった。
       高負荷時のポップアップ表示が PopUp よりもすんなりできている。
       0.5.0.4 の新しいバージョンでは、ポップアップが表示されないようになってしまったので、バージョンアップしなかった。
     - 使う機会がなくなった。
     - 2010-12-13
   * - `Message Export mod (Unicode) <http://addons.miranda-im.org/details.php?id=3973>`_
     - 3.1.0.3
     - メッセージをデータベースからテキストファイルに保存。
     - 使う機会がなくなった。
     - 2009-01-29
   * - `Miranda IM Database Tool <http://addons.miranda-im.org/details.php?id=73>`_
     -
     - データベースからいらない情報を削除したり，データベースのサイズを小さくしたり。
     - 使う機会がなくなった。
     -
   * - `realreconnect <http://addons.miranda-im.org/details.php?id=1783>`_
     - 0.0.1.1
     - ネットワークの接続に失敗したときに再接続を試みる。
       サイズも小さいし、使っている DLL も少ないようだったので使ってみる。
       とりあえず問題はないみたい。
     - 使う機会がなくなった。
     - 2005-12-27
   * - `Message Notify <http://addons.miranda-im.org/details.php?id=2415>`_
     - 0.3.0.2
     - メッセージが届いたときにポップアップを表示するプラグイン。
       メッセージウィンドウが最前面になっていないときにポップアップを表示するようにしている。
     - 使う機会がなくなった。
     - 2007-07-18
   * - `Gmail Multiple Notifier (UNICODE) <http://addons.miranda-im.org/details.php?id=3677>`_
     - 0.4.0.10
     - Gmail の新着チェックをする。
       0.4.0.9 はステータスが Unknown にしかならなかった。0.4.0.10 で修正。
     - 使う機会がなくなった。
     - 2008-12-22
   * - `History++ (2in1) <http://addons.miranda-im.org/details.php?id=2995>`_
     - 1.5.1.4
     - メッセージの履歴を便利に検索することができたりする
     - 使う機会がなくなった。
     - 2010-02-27
   * - `History Sweeper+ Unicode <http://addons.miranda-im.org/details.php?id=4132>`_
     - 0.2.0.1
     - 履歴削除。
     - 使う機会がなくなった。
     - 2009-08-31
   * - `Proxomitron <http://www.proxomitron.org/>`_
     - 4.5june+shift_jis誤爆回避日本語化パッチ+RWIN32768回避+バイパス赤アイコン+有難屋さんgoodjob!
     - Web ページの広告を削除したり，ポップアップを抑止したり。
       `Proxomitron-J <http://www.pluto.dti.ne.jp/~tengu/proxomitron/index.html>`_ ,
       `Proxomitorn 等に関する Wiki <http://abc.s65.xrea.com/prox/wiki/>`_
     - 使う機会がなくなった。
     - 2004-12-12
   * - `OperaCacheView <http://www.nirsoft.net/utils/opera_cache_view.html>`_
     - 1.36
     - Opera のキャッシュに存在するファイルを一覧する。
       Web マンガを読んでいて、URL で検索して画像を一括で保存といったことに使った。
     - 使う機会がなくなった。
     - 2010-03-06
   * - `MPlayer <http://www.mplayerhq.hu/>`_
     - corei7-r37653+g674cc26 (Gianluigi Tiesi)
     - マルチメディアプレイヤ。
       `Gianluigi Tiesi <http://oss.netfarm.it/mplayer-win32.php>`_
       使い方いくつか

       - DVD の再生（数字やデバイスは適宜変更）: mplayer dvd://1 -aid 128 -dvd-device k: -vf filmdint=io=2997:2997
       - 音量変更: -af volume=17:1
       - ストリーミングデータのダウンロード: mplayer mms://somewhere/hoge.asf -dumpstream -dumpfile hoge.asf
       - 音声のデコード: mplayer hoge.rm -ao pcm:file=hoge.wav
       - input.conf で vo_ontop を指定しているために ontop のトグルがうまいこと動いていないようなので、コメントアウト
       - mplayer/codes.conf を用意して `windows codes <http://www2.mplayerhq.hu/MPlayer/releases/codecs/windows-essential-20071007.zip>`_ を codecs へ展開する
       - 再生時間などを表示するために、mplayer/config へ osdlevel=3 を記述する
       - `PL_fonts-ISO8859-2_and_WINDOWS-1250.tgz <ftp://ftp.mplayerhq.hu/MPlayer/contrib/fonts/windows-1250/PL_fonts-ISO8859-2_and_WINDOWS-1250.tgz>`_ を font あたりに展開して、mplayer/config の font で font.desc をフルパス指定する
       - vo=gl とする

         - geometry=100%:100% がちゃんと右隅に行くようになる。vo=directx だと画面からはみ出してしまう
         - フルスクリーンにしても、再生時間表示が設定したサイズで表示できる (noscaled-osd)。vo=directx だと倍率に合わせて拡大縮小されてしまう
         - フルスクリーンにしたときに、再生時間表示がちゃんと左隅に表示される。vo=directx だと拡大縮小の結果、上下に黒帯が発生しても、黒帯部分には再生時間表示をしてくれない
         - 最前面オプションを有効にして動画を再生した直後に Alt + Tab でフォーカスを移動すると、ちゃんとそのウィンドウが前面にくる。
           vo=directx だと何回かフォーカスを移動させないと駄目
         - 負荷が比較的高い

       - 最小化/最大化して元に戻したときにウィンドウのサイズが変になる
       - 再生失敗ビルド

         - p4-svn-33489
         - corei7-r36541+g43f9255

       - i7-r35910 あたりから初回起動時に ``C:\Users\hokorobi\AppData\Local\fontconfig`` にフォントのキャッシュを作るようになった。
         フォントキャッシュを作らないようにする設定はわからない。nofontconfig ではないみたい。

     - mpv へ移行。
     - 2016-02-11
   * - `Clink <http://mridgers.github.io/clink/>`_
     - 0.4.4
     - ConEmu で bash ライクな色々を提供してくれる。
       履歴と C-r のインクリメンタルサーチでしかほとんど使えていないけれど。
     - nyagos を使うようになったので、とりあえずインストールしていない
     - 2015-02-28
   * - `CubePDF <http://wwwcube-softjp/cubepdf/>`_
     - 1.0.0 RC7
     - 印刷をPDFへ保存。
     - Windows10 にしたら PDF 出力が OS にあったので削除
     - 2014-11-28
   * - `akinosign <http://www.vector.co.jp/soft/winnt/writing/se495848.html>`_
     - 2.02
     - IME の状態をテキストフィールドの色を変えて表示。
       .NET Framework 製なのでメモリ消費量は多い。
       色を見る前に入力を始めてしまうので意味が無い……。慣れたら違うのかな？
     - やっぱり慣れなかった。
     - 2014-05-31
   * - `FreeMind <http://freemind.sourceforge.net/wiki/index.php/Main_Page>`_
     - 1.0.0 beta2
     - マインドマップを書くためのツール。
       その名の通りフリー。
     - Freeplane へ。
     - 2012-04-21
   * - `True Crypt <http://www.truecrypt.org/>`_
     - 6.3a
     - USB メモリの暗号化。
     - USB メモリを使うことがなくなったし、True Crypt は死んだので使っていない。
     - 2009-11-25
   * - `BitDefender <http://www.bitdefender.com/index.php>`_
     - 8.0 Free
     - DL したファイルのチェックに使っている。

       - コマンドラインから使うだけなので、インストール時には Custom を選んで削れる物はすべて削る。
       - サービスのBitDefender Scan Server、BitDefender Communicator を停止して無効にする。
       - BDMCon と BDNewsAgent を自動起動しないようにレジストリをいじる。
       - `BitDefender (コマンドライン版) <http://lets-go.hp.infoseek.co.jp/bitdefender.html>`_ で提供されている bdcscan.bat を使っている。
       - 定義ファイルのアップデートは bdcupdate.vbs を使っている。

     - 個別にチェックはしなくなった Avira しか使っていない。
     - 2005-08-10
   * - `PageDefrag <http://technet.microsoft.com/ja-jp/sysinternals/bb897426(en-us).aspx>`_
     - 2.32
     - ページファイルやレジストリの断片化を解消。
       Windows7 64bit Home Premium では使えないみたい。
     - SSD になったのでデフラグは使わなくなった。
     - 2005-07-13
   * - `Auslogic Registry Defrag <http://www.auslogics.com/en/software/registry-defrag/>`_
     - 7.3.1.0
     - レジストリのデフラグ。
     - Eusing Software の方がデフラグ対象が多いみたいなので、こちらは削除。
     - 2013-10-17
   * - `Eusing Free Registry Defrag <http://www.eusing.com/free_registry_defrag/registry_defrag.htm>`_
     - 2.2
     - レジストリのデフラグ。
     - Windows10 には対応していないみたい。
     - 2013-10-15
   * - `md5sum <http://www.hakusan.tsg.ne.jp/tjkawa/software/paranoia/sha1sum/index.jsp>`_
     - 0.0.2
     - ファイルが同じものなのかどうか確認。
       ファイル一覧からハッシュ一覧を作成。
       md5sum -l hoge &gt; hoge.md5
       ハッシュ一覧とカレントディレクトリのファイルを比較
       md5sum -c hoge.md5
     - 使う機会がなくなった。
     - 未インストール
   * - `UnDup <http://hp.vector.co.jp/authors/VA032597/>`_
     - 1.5g
     - 重複ファイルの削除。
     - 使う機会がなくなった。
     - 未インストール
   * - `Unlocker <http://ccollomb.free.fr/unlocker/index.htm>`_
     - 1.9.1
     - ロックされて削除のできないファイルをアンロックしてくれる。
     - 使う機会がなくなった。
     - 未インストール
   * - `Recuva <http://www.piriform.com/>`_
     - 1.53
     - ゴミ箱からも削除してしまったファイルを復元。
     - 使う機会がなくなった。
     - 2016-06-12
   * - `ResourceHacker <http://www.angusj.com/resourcehacker/>`_
     - 3.5.2
     - アプリケーションの邪魔なダイアログを削ったり，フォントを変えたり。
     - 使う機会がなくなった。
     - 2011-11-23
   * - `Comodo Internet Security <http://www.personalfirewall.comodo.com/>`_
     - 6.3.297838.2953 64bit
     - COMODO Personal Firewall から変更。
       AntiVirus 機能を正式に謳うようになって名称も変更されたみたい。
       `Comodo Firewall Pro @ まとめ <http://www4.atwiki.jp/comodopf/>`_ ,
       `公式フォーラム <https://forums.comodo.com/>`_
     - Windows10 以降とともに削除
     - 2013-11-04
   * - `WinSCP <http://winscp.net/>`_
     - 5.1
     - FTP クライアント。
       いつの間にか多重接続できるようになっていたみたい。
       キューはちゃんと動くかな？
     - 使っていないので削除。
     - 2012-09-25
   * - `QMAIL3 <http://q3.snak.org/ja/>`_
     - 3.0.9
     - メーラ。
       Gmail の受信後の処理でエラーが出るようになったので Sylpheed へ乗り換え。
       インポートは、 ``C:\Users\hokorobi\AppData\Roaming\QMAIL3\accounts\GMail_tada\msg`` のファイルを ``*.eml`` へ変更してインポート。
     - 使っていないので削除。
     - 2010-11-25
   * - `Sylpheed <http://sylpheed.sraoss.jp/ja/>`_
     - 3.5
     - メーラ
     - Gmail だけでしかメールを使わないので削除。
     - 2016-01-27
   * - `Opera <http://www.opera.com/>`_
     - 12.17 32bit / 27
     - 窓の杜からもらったので使う。
       `ftp win <http://ftp.opera.com/pub/opera/win/>`_
       11.60 は読み込みが途中で切れたり、よく落ちたりするので 11.52 に戻した。
       11.61 は読み込みが途中で切れる現象がまだ起こるので 11.52 に戻した。少し試した限りでは落ちることはほとんどなかった。
       11.60 以降の読み込みが途中で切れる件は、opera:config#Performance|EnablePipelining を使わないように設定することで改善されたみたい。
     - Cyberfox へ移行した。
     - 2014-04-12 / 2015-01-27
   * - `Notepad++ <http://notepad-plus-plus.org/>`_
     - 6.3.2
     - Mercurial のコミットメッセージ入力用
     - 使っていない。
     - 2013-04-06
   * - `Foxit Reader <http://www.foxitsoftware.com/>`_
     - 5.3.1.0606
     - 以前はフォントが気に入らなくて削除してしまったけれど、だいぶマシになったように感じる。それでも Acrobat Reader の方が好みではある。
       ページめくりで PDF-XChange Viewer のようにちらつかないのは良い。
       ページめくりの速度も上々。
     - Sumatra PDF へ。
     - 2012-08-26
   * - `PDF-XChange Viewer <http://www.docu-track.com/>`_
     - 2.00407 Portable
     - ページめくりのちらつきが嫌。
       編集機能が付いているので気にはなるのだけれど……。
     - 背景色が白以外だったりすると耐えられない。
     - 2008-11-27
   * - `Paper Plane xUI Everything Search Module <http://toro.d.dooo.jp/slppx.html#ppxets>`_
     - R5
     - Everything を使って検索機能を追加。
     - インクリメンタルサーチが便利なので Everything を呼び出して使うようにした。
     - 2013-12-22
   * - `Direct Show Filter Tool <http://hp.vector.co.jp/authors/VA032094/DFTool.html>`_
     - 1.04
     - メリット値を変更して優先させるフィルタを変更。
     - 使う機会がなくなった。
     - 2004-08-17
   * - `xyzzy with 2ch-mode <http://www7a.biglobe.ne.jp/~hat/xyzzy/2ch-mode.html>`_
     - 0.0.1.2
     - 2ch を xyzzy で読む。
       なかなか使いこなせないけどインクリメンタルサーチが便利。
     - 使う機会がなくなった。
     - 2010-10-26
   * - `xyzzy <http://www.jsdlab.co.jp/~kamei/>`_
     - 0.2.2.249
     - メモを書いたり、2ch 見たり、コード書いたり。
       - `xyzzy 0.2.2 <http://xyzzy-022.github.com/>`_
     - 使う機会がなくなった。
     - 2013-04-29
   * - `Bazaar <http://bazaar.canonical.com/en/>`_
     - 2.5.1-1 standalone
     - 日本語ファイルのバージョン管理に。
     - 使う機会がなくなった。
     - 2012-07-05
   * - `msysgit <http://code.google.com/p/msysgit/>`_
     - 1.9.4-preview20140929
     - | Linus 原作のバージョン管理システム。
       | git log を実行すると、このようなメッセージが表示される

       .. code-block:: none

         WARNING: terminal is not fully functional

       | 付属の less.exe を less.exe.bak などのようにして、 RuRuRu さんの less を実行するようにしている。
       | 文字化けが発生するので設定変更

       .. code-block:: none

         git config --global core.pager "LESSCHARSET=utf-8 less"

     - 2016-02-27 アンイストール。MSYS2 の Git に移行済み。
     - 2014-11-23
   * - `dgcac.exe <http://www.emit.jp/>`_
     - 1.09
     - DGCA 書庫操作用コンソールアプリケーション。
     - 使う機会がなくなった。
     - 2006-02-27
   * - `UnGCA32.DLL <http://www6.plala.or.jp/amasoft/index.html>`_
     - 0.11b
     - GCA 書庫操作用 DLL。
     - 使う機会がなくなった。
     - 2005-03-15
   * - `GitKraken <https://www.gitkraken.com/>`_
     - 2.31
     - Git の GUI クライアント
     - コミットにフォーカスを移したときに、差分が表示されてほしいので SourceTree へ移行
     - 2017-04-07
   * - `ERUNT, NTREGOPT <http://www.larshederer.homepage.t-online.de/erunt/index.htm>`_
     - 1.1j
     - ERUNT でレジストリのバックアップ（使ったこと無い）。
       NTREGOPT でレジストリの最適化。
     - Windows10 で使えるか確認できないので削除 [2017-05-17]
     - 2005-10-20
   * - `最前面でポーズ <http://so-zou.jp/software/pause/>`_
     - 1.03
     - Amazon ビデオを IE で見る際に最前面に表示。
     - autohotkey で作れたのでお蔵入り [2017-11-19]
     - 2016-12-27
   * - `FileSeeker3 <http://mokuzu.sakura.ne.jp/wiki/?FileSeeker3>`_
     - 3.1.1 beta
     - NTFS change Journal を使って高速ファイル検索。
     - 管理者権限にならないといけないので使いにくい。
     - 2010-08-21
   * - `DAEMON Tools Lite <http://www.daemon-tools.cc/dtcc/announcements.php>`_
     - 4.35.6
     - イメージファイルをマウントして普通のドライブのように使う。
       secure mode のチェックを外さないと、コマンド実行しても確認ダイアログが表示される。
       CraftLaunch から以下のようにして使っている。

       .. code-block:: none

         cmd daemon
         -L C:\bin\daemon.exe
         -A -mount 0, "%arg"
         -F C:\bin
         ^L C:\bin\daemon.exe
         ^A -unmount 0
         ^F C:\bin

     - 使おうとしたらエラーメッセージが出るようになったのでアンインストール。
       Virtual Clone Drive へ変更。
     - 2010-12-06
   * - `Revo Uninstall <http://www.revouninstaller.com/revo_uninstaller_free_download.html>`_
     - 1.9.4 portable
     - 「アプリケーションの追加と削除」よりも色々と消してくれるアンインストーラ。
     - 使う機会がなくなった。
     - 2012-05-16
   * - `Extensible Performance Counter List <http://www.microsoft.com/windows2000/techinfo/reskit/tools/existing/exctrlst-o.asp>`_
     - 不明
     - パフォーマンスカウンタを取るか否かの選択ができる。
       ftp://ftp.microsoft.com/reskit/win2000/ からもダウンロードできる。
     - 使う機会がなくなった。
     - 2005-09-17
   * - `RegDllView <http://www.nirsoft.net/utils/registered_dll_view.html>`_
     - 1.36
     - COM に登録されている DLL, OCX, EXE を一覧表示する。
       登録されているけれど使っていないというものを幾つか見つけて削除することができた。
     - 使う機会がなくなった。
     - 2009-09-02
   * - `Javara <http://raproducts.org/>`_
     - 1.14
     - Java のランタイム削除。
     - 使う機会がなくなった。
     - 2009-05-29
   * - `bbLean <http://bb4win.sourceforge.net/bblean/>`_
     - bbLean 1.17.1 64bit
     - 軽いという代替シェル。
       特に軽いという風にも思わなかったけど Explorer の変わりに Shell にしている。
     - Win7 から使っていない。
     - 2010-10-26
   * - `nyaos <http://www.nyaos.org/index.cgi?p=FrontPage.ja>`_
     - 3.3.6_1
     - シェル
     - nyagos へ。
     - 2013-03-20
   * - `ckw-mod <https://github.com/hokorobi/ckw-mod>`_
     - 0.9.0-d2 x64
     - シェルラッパー？
     - ConEmu へ。
     - 2012-01-19
   * - `Console2 <http://sourceforge.net/projects/console/>`_
     - 2.00b147 64bit + IME 20110527
     - シェルラッパー
       日本語入力ができるように cmd にかぶせて使っている。
     - ConEmu へ。
     - 2012-08-26
   * - `Calibrize <http://www.calibrize.com/>`_
     - 3.5.0
     - 色味の調整をするソフト。
       `テテのつぶやき: CalibrizeをWindows 7で使用する方法 <http://tete009.seesaa.net/article/208363148.html>`_ を見て再設定。
       「Windows のディスプレイ調整を使用」はチェックボックスはオフになっていた。
       msconfig から 「Intel(R) Common User Interface」のスタートアップ対象からはずした。
       Calibrizeが作成したICCプロファイルが（既定）になっていなかったので変更してみた。
       タスクスケジューラに Calibrize Gamma Loader を登録しているけれど、レジストリの User Run に登録されているから不要だったりしないのかな？
     - とりあえず設定していない。
     - 2017-07-29
   * - `NanJoy <http://crimson.onmitsu.jp/>`_
     - 2.33
     - ジョイパッドの操作をキーボードやマウスに割り当てる。
     - JoyToKey へ。
     - 2010-10-05
   * - `かざぐるマウス <http://www.staticflower.net/software/kazaguru.html>`_
     - 1.65
     - マウスジェスチャ。
     - 使う機会がなくなった。
     - 2013-06-09
   * - `RegScanner <http://www.nirsoft.net/>`_
     - 2.00
     - レジストリから文字列を検索して一覧表示。
       一覧から regedit.exe で該当する箇所を表示。
     - 使う機会がなくなった。
     - 2013-07-14
   * - `Tera Term <http://sourceforge.jp/projects/ttssh2/>`_
     - 4.65
     - Cygwin へのアクセスに使用する Cygterm のため。
     - 使う機会がなくなった。
     - 2010-05-02
   * - `radiro <http://radiro.tcraft.biz/>`_
     - 1.0.9.1
     - radiko ブラウザ。
     - 使う機会がなくなった。
     - 2012-12-16
   * - `MuRadiko <http://www.muraodos.com/muradiko.html>`_
     - 2.66
     - radiko.jp(ラジコ) ・らじる★らじる・サイマルラジオ（“CSRA.fm”・“JCBA”）
     - 使う機会がなくなった。
     - 2013-03-31
   * - `Wireshark <http://www.wireshark.org/>`_
     - 1.8.5 64bit
     - パケットキャプチャ。
       Winpcap サービスを OS 起動時に実行しない場合、Wireshark を管理者権限で実行しないと Winpcap のサービスが起動できずにエラーとなる。
       `参考 <http://typea.info/tips/wiki.cgi?page=Wireshark+Windows7+%A4%C7+NPF%A5%C9%A5%E9%A5%A4%A5%D0%A5%A8%A5%E9%A1%BC>`_
       Wireshark.exe のプロパティから管理者で実行するように設定。
     - 使う機会がなくなった。
     - 2013-01-30
   * - `WinPcap <http://www.winpcap.org/>`_
     - 4.1.2
     - Wireshark で必要。
     - 使う機会がなくなった。
     - 2011-12-24
   * - `TCP Monitor Plus <http://hp.vector.co.jp/authors/VA032928/>`_
     - 2.59
     - 通信状況表示
     - 使う機会がなくなった。
     - 2012-01-19
   * - `UltraVNC <http://www.uvnc.com/>`_
     - 1.0.8.2
     - VNC
     - 使う機会がなくなった。
     - 2011-05-14
   * - `TrueRemote <http://blog.x-row.net/?p=47>`_
     - 1.2.6
     - リモートデスクトップ。
     - 使う機会がなくなった。
     - 2012-04-10
   * - `Brynhildr <http://brynhildr.x-row.net/>`_
     - 1.0.0.2
     - リモートデスクトップ。TrueRemote の方が速い。
     - 使う機会がなくなった。
     - 2013-10-15
   * - `Mirror-DTC <http://homepage2.nifty.com/t_ishii/mc/>`_
     - 1.2.3
     - リモートデスクトップ。TrueRemote より速いかも
     - 使う機会がなくなった。
     - 2013-04-07
   * - `Cyberfox <https://cyberfox.8pecxstudios.com/>`_
     - 52.6.1
     - Opera がきな臭くなってきたので移行先として試している。
       メインブラウザは Vivaldi へ移行した。
       サブのブラウザを Firefox にしていたが 57 から使えなくて不便になる拡張があったので Cyberfox をサブにした。 [2017-11-15]
     - Firefox をサブにした。 [2018-01-21]
     - 2018-01-21
   * - `SRWare Iron <http://www.srware.net/forum/viewforum.php?f=18>`_
     - 61
     - Chromium 派生 Web ブラウザ。
       28.0.15500.0 は twicli でツイートやリツイートに反応しないことがある。
       Opera15 と同じ現象だから、どうも Blink がまずいみたい。
     - Vivaldi へ。
     - 2017-09-26
   * - `jq.exe <http://stedolan.github.io/jq/>`_
     - 1.2
     - JSON パーサ。 `紹介 <http://beatsync.net/main/log20130428.html>`_
     - jj へ。
     - 2013-04-30
   * - `jvgrep <https://github.com/mattn/jvgrep/downloads>`_
     - 4.2 amd64 go 1.5.1
     - 文字コード混在のファイルを grep できるソフト。
       go をインストールしてビルドした。 http://d.hatena.ne.jp/hokorobi/20130615/1371285263
       go get -u -ldflags -s github.com/mattn/jvgrep
     - Platinum Searcher の方が速いようなので移行できないか試している。
     - 2015-10-24
   * - `PngOptimizer <http://psydk.org/PngOptimizer.php>`_
     - 2.0 x64
     - PNG のサイズを小さくする。
       PNGOUT よりは大きくなる。でも速い。
     - pingo へ。
     - 2011-09-24
   * - `SmillaEnlarger <http://sourceforge.net/projects/imageenlarger/>`_
     - 0.9.0
     - 画像を綺麗に拡大。
     - 使う機会がなくなった。
     - 2010-09-07
   * - `JDK <http://www.oracle.com/technetwork/java/javase/downloads/index.html>`_
     - 1.8.0.73 x64
     - JDK。とりあえず削除した。
       また入れた。
     - 使う機会がなくなった。
     - 2016-02-22
   * - `contig <http://technet.microsoft.com/ja-jp/sysinternals/bb897428(en-us).aspx>`_
     - 1.7
     - ファイルを個別にデフラグしてくれる。
       動画などを再生していて HDD の音が大きいときなんかに試す。
     - SSD になったので使わなくなった。
     - 2012-11-20
   * - `WinContig <http://wincontig.mdtzone.it/en/index.htm>`_
     - 2.1.0.0
     - ファイルやフォルダを指定してデフラグ
     - SSD になったので使わなくなった。
     - 2017-02-19
   * - `Defraggler <http://www.piriform.com/defraggler>`_
     - 2.19
     - デフラグツール。
       Analyze 後にファイルサイズが大きい物だけデフラグとか。
     - SSD になったので使わなくなった。
     - 2015-03-14
   * - `Auslogic Disk Defrag <http://www.auslogics.com/en/software/disk-defrag/>`_
     - 5.2.0
     - デフラグ
     - SSD になったので使わなくなった。
     - 2015-01-30
   * - `Noah <http://www.kmonos.net/>`_
     - 3.199
     - アーカイバ DLL を使って様々なファイルの圧縮解凍。
       b2e ファイルを書くことで更なる拡張も可能。
       `Noah+ もあるよ。`:strike: ゴタゴタがあってなくなったみたい。
       Noah.ini へ NoExt=1 を指定すると aaa.bbb.ccc を圧縮したときの書庫名を aaa.lzh ではなく aaa.bbb.ccc.lzh としてくれる。
     - 使う機会がなくなった。
     - 2010-11-26
   * - `7za.exe <http://sourceforge.net/projects/sevenzip/>`_
     - 9.22 beta
     - `yc 氏の 7z.b2e <http://b2efile.at.infoseek.co.jp/0-b.html#sevenzip>`_ をもらってきて Noah から 7z 展開用に使用している。
       DF の登録コマンドから直接、7z 圧縮用に使用している。
     - 使う機会がなくなった。
     - 2011-04-19
   * - `rar.exe, unrar.exe <http://www.rarsoft.com/>`_
     - 4.1.1
     - Noah から RAR 書庫を作成する。
     - 使う機会がなくなった。
     - 2012-04-29
   * - `偽UnZip32.DLL <http://www31.ocn.ne.jp/~heropa/>`_
     - 5.5.2.0 (4)
     - 7-zip32.dll を使って UnZip32.DLL のふりをさせる DLL。
       DF から zip を扱う場合に使用している `……まず使う場面はないけれど。`:strike: 結構使うようになった。
     - 使う機会がなくなった。
     - 2009-08-14
   * - `7-zip32.dll <http://akky.cjb.net/>`_
     - 9.22.00.02
     - 偽UnZip32.DLL を併用して DF から zip を扱う場合に使用している `……まず使う場面はないけれど。`:strike: 結構使うようになった。
     - Noah 経由でも 7za を使用するようになった。
     - 2017-02-17
   * - `WinExChange <http://www.55555.to/>`_
     - 7.09
     - ファイルの拡張子を中身から推測。
     - 使う機会がなくなった。
     - 2010-08-25
   * - `DF (ファイラ) <http://homepage1.nifty.com/bee/df/>`_
     - Ver.198
     - Windows を使ってるときはたいてい動かしているファイラ。
       えらく軽い。
       ほとんどないのだけれど要望を控えておく。

       - lzh, zip 以外のアーカイバ（cab, tar, bga, 7z, rar）にも対応してほしい。
       - テキストビュアで UFT-8 の表示も可能にしてほしい。
       - 同じくテキストビュアで文字コードの判別精度を上げてほしい。
       - ビューアを表示したまま、ファイラから次のファイルを表示するといった機能をつけてほしい。

     - PPx へ。
     - 2011-08-07
   * - `CCleaner <http://www.ccleaner.com/>`_
     - 5.32
     - 不要なレジストリキーの削除。
       テンポラリファイル他などのファイルも削除。
     - 使う機会がなくなった。
     - 2017-07-15
   * - `Easter <http://hp.vector.co.jp/authors/VA035038/download/easter/index.html>`_
     - 0.92
     - 取り外し状態になった USB 機器を再接続。
       SD カード取り出しのために、SD カードリーダを取り外し状態にしたときなんかに使っている。
     - XP 時代の話なので 7 では、まだ使ったことがない。
     - 2011-03-07
   * - `AutoIt <http://www.autoitscript.com/site/autoit/>`_
     - 3.3.8.1
     - スクリプトによる Windows の操作。
     - 使う機会がなくなった。
     - 2012-01-31
   * - `UWSC <http://www.uwsc.info/>`_
     - 4.8e Free
     - スクリプトによる Windows の操作。
     - 使う機会がなくなった。
     - 2013-04-03
   * - `bktimer <http://www14.ocn.ne.jp/~bkclass/bktimer.html>`_
     - 0.13.0-1
     - タイマーで色々と使用。
       コマンドラインオプションで時間が設定できるのが嬉しい。
       `AAタイマー <http://hp.vector.co.jp/authors/VA011136/aatm.html>`_ から変更。
     - 自作タイマーを使うようになった。
     - 2012-02-09
   * - `KeyHoleTV <http://www.v2p.jp/video/>`_
     - 3.14
     - テレビの視聴。ほとんど使えない。
     - 使う機会がなくなった。
     - 2010-05-02
   * - `SQLiteStudio <http://sqlitestudio.one.pl/index.rvt>`_
     - 1.1.3
     - SQLite を GUI で操作。
     - 使う機会がなくなった。
     - 2010-04-29
   * - `SQLite <http://www.sqlite.org/>`_
     - 3.6.23.1
     - 小さな SQL データベースエンジン。
     - 使う機会がなくなった。
     - 2010-04-29
   * - `WhosIP <http://www.nirsoft.net/utils/whosip.html>`_
     - 1.03
     - PFW の設定などで IP を範囲指定するときなどに使ったりする。
       以前は `ANSI Whois Gateway <http://whois.ansi.co.jp/>`_ を使っていた。
     - 使う機会がなくなった。
     - 2008-12-11
   * - `Cygwin <http://cygwin.com/>`_
     - 1.7.4-1
     - | Windows で Linux ライクの環境を。
       | MinGW でビルドできなかったソフトをこちらではどうか試すくらい。
       | インストールするのは

       - Base
       - Devel/gcc
       - Devel/gettext
       - Devel/gdb
       - Devel/make

       | cygwin.bat に環境変数を設定

       .. code-block:: bat

         set CYGWIN=ntsec
         set HOME=/home/hokorobi
         set MAKE_MODE=UNIX
         set SHELL=/bin/bash
         set LANG = ja_JP.SJIS
         set TZ = JST-9

       | ~/.bash_profile へ色々設定。改行コードはインストール時の指定に合わせる。
       | ~/.bashrc は読み込んでくれなかった。きっと私がまずいことしてる。

       .. code-block:: bash

         export LESS=MrXE
         export LC_MESSAGES=c
         export PS1='\[\e[33m\]\w\[\e[0m\]\n\$ '
         alias ls='ls --show-control-chars --color=auto'

       | `UTF-8 Cygwin <http://www.okisoft.co.jp/esc/cygwin-20.html>`_ というのもある。
     - 最近は使っていない。
     - 2010-04-10
   * - `Eclipse <http://www.eclipse.org/>`_
     - 3.7.1 Eclipse IDE for Java Developers
     - IDE
     - 使う機会がなくなった。
     - 2011-12-28
   * - `groovy <http://groovy.codehaus.org/>`_
     - 2.1
     - groovy `groovy <http://groovy.codehaus.org/>`_
     - 使う機会がなくなった。
     - 2013-01-26
   * - `Virtual Clone Drive <http://www.elby.ch/>`_
     - 5.4.7.0
     - イメージファイルをマウントして普通のドライブのように使う。

       .. code-block:: none

         cmd vcd
         -L C:\Program Files (x86)\Elaborate Bytes\VirtualCloneDrive\VCDMount.exe
         -A
         -F C:\Program Files (x86)\Elaborate Bytes\VirtualCloneDrive
         ^L C:\Program Files (x86)\Elaborate Bytes\VirtualCloneDrive\VCDMount.exe
         ^A /u
         ^F C:\Program Files (x86)\Elaborate Bytes\VirtualCloneDrive

     - Win10 の機能で十分。
     - 2014-05-20
   * - `UNBYPASS <http://toro.d.dooo.jp/slplugin.html#unbypass>`_
     - 1.7
     - 32 bit Susie Plugin を 64 bit Paper Plane で使う。
     - 本体同梱なので削除 [2018-08-15]
     - 2015-03-14
   * - `LAV Filters <http://forum.doom9.org/showthread.php?t=156191>`_
     - 0.55.3 Splitter
     - | DirectShow Media Splitter and Decoders
       | 管理者権限でコマンドプロンプトを起動して、install_splitter.bat を実行してインストール。
       | 0.55.3 から exe でインストール。 ``C:\Program Files (x86)\LAV Filters``
     - 使う機会がなくなった。
     - 2013-03-17
   * - `PowerDVD <http://jp.cyberlink.com/products/powerdvd/overview_ja_JP.html>`_
     - 12
     - | MPCHC で H264 の再生に使ってみる。
       | Uniextract で展開して、Data1.7z の ``MediaEspresso\subsys\Video\filter\H264`` のファイルを適当なところにコピー。
       | 外部フィルタとして cl264dec.ax を指定。 Prefer に指定。
       | ダブルクリックで DXVA を使うように設定。
     - 使う機会がなくなった。
     - 2012-02-02
   * - `Kobito <http://kobito.qiita.com/win>`_
     - 2.0.2
     - Qiita への投稿。
     - 使えなくなった。
     - 2016-09-06
   * - `Avidemux <http://fixounet.free.fr/avidemux/>`_
     - 2.6.15
     - Youtube の動画の不要部分を無劣化で取り除く。
     - LosslessCut に移行。
     - 2016-12-04
   * - `GanttProject <http://www.ganttproject.biz/>`_
     - 2.6.1
     - MS Project みたいなの
     - 使う機会がなくなった。
     - 2013-02-08
   * - `PsKill <http://technet.microsoft.com/ja-jp/sysinternals/bb896683.aspx>`_
     - 1.15
     - プロセスの停止。
       Mercurial 拡張 statdaemon で常駐する hg.exe を停止させる。
     - 使う機会がなくなった。
     - 2012-10-28
   * - `USB Oblivion <http://code.google.com/p/usboblivion/>`_
     - 1.9.0.0
     - USB の接続情報を削除する。
     - 使う機会がなくなった。
     - 2012-11-15
   * - `milkode <http://milkode.ongaeshi.me/>`_
     - 0.29
     - rroonga を使って全文検索。
     - 使う機会がなくなった。
     - 2011-12-26
   * - `私本管理Plus <http://homepage1.nifty.com/EKAKIN/>`_
     - 6.1.0
     - 蔵書管理ソフト。
       3.4.29 から (多分) ISBN を元にした書籍データの取得が速くなった。素敵。
       5.6.13 は Ctrl や Shift を押すとエラーダイアログが表示される場合があったのでやめた。
     - `ブクログ <https://booklog.jp/>`_ に移行。 [2016-09-19]
     - 2016-04-08
   * - `Ruby <http://rubyinstaller.org/>`_
     - 1.8.7 p352
     - いまさらだけど触ってみようかなと。
       `readline.dll 4.3.2 <http://jarp.does.notwork.org/win32/>`_

       DevKit をインストールすると色々と make が通るようになる。
       $ ruby dk.rb init
       config.yml の末尾に - ``M:\OLS\Program\Ruby187`` などを追加。
       $ ruby dk.rb install

       mswin32 版は make でなく nmake を使おうとするので DevKit では使えない（使い方があるのかもしれないが知らん）
     - 使う機会がなくなった。
     - 2011-12-26
   * - `MKVToolnix <http://www.bunkus.org/videotools/mkvtoolnix/>`_
     - 5.0.1
     - MKV や MKA を作製するためのツール群。
     - 使う機会がなくなった。
     - 2011-10-10
   * - `x264 <http://developers.videolan.org/x264.html>`_
     - revision 1120 bob0r
     - H.264/AVC をエンコードするためのライブラリらしい。
       `bob0r <http://x264.nl/>`_ , http://komisar.gin.by/ , `猫科研究所 <http://www.up-cat.net/FrontPage.html>`_ : changelog 和訳
     - 使う機会がなくなった。
     - 2009-03-05
   * - `Avisynth <http://sourceforge.net/projects/avisynth2/>`_
     - 2.5.8
     - 久方ぶりに WavSource を使ってみたらエラーが発生するようになった。原因不明 (2.5.7, 2.5.8 RC4 and RC4a)
     - 使う機会がなくなった。
     - 2009-01-03
   * - `avs2wav <http://www.avisynth.info/?avs2wav>`_
     - 2007-10-08
     - AVS ファイルから WAV ファイルを出力する。
     - 使う機会がなくなった。
     - 2007-11-28
   * - `DGMPGDec <http://neuron2.net/dgmpgdec/dgmpgdec.html>`_
     - 1.5.8
     - DVD のデータを Avisynth へ渡すためのデータを作成する。
       Frame Rate が 29.970 で、Video Type の欄が FILM n% (n &gt;= 95)、または FILMとなっていた場合は、Field Operation を Forced FILM にする。
     - 使う機会がなくなった。
     - 2010-12-05
   * - `VirtualDub <http://sourceforge.net/projects/virtualdub/>`_
     - 1.9.10
     - Desktop video processing and capture application (Win32).
     - 使う機会がなくなった。
     - 2010-09-07
   * - `AvsP <http://avisynth.org/qwerpoi/>`_
     - 2.2.0 mod
     - Avisynth 用のテキストエディタ。動画のフレームプレビューも可能。再生はできないみたい。
       `AvsPmod <http://forum.doom9.org/showthread.php?t=153248>`_
     - 使う機会がなくなった。
     - 2011-07-01
   * - `MP4Box <http://kurtnoise.free.fr/mp4tools/>`_
     - 0.4.5
     - MPEG-4 コンバータ。
       MPEG-4 video (DivX/XviD/3ivx/ffmpeg) と audio ストリームを mp4 コンテナにインポートするもの。
       出力結果は ISO 適合の MPEG-4 ストリーム。この他に、srt などの字幕形式をインポートして MPEG-4 Timed Text ストリームを生成可能。
       x264 で作製した .264 を .mp4 とする。
       MP4BOX GUI `YAMB <http://yamb.unite-video.com/>`_

       - FPS 指定 (119.880 は適宜 23.975026, 29.970030 などへ): mp4box -fps 119.880 -add hoge.264 -new hoge.mp4
       - mp4 ファイルからの取り出し: mp4box -raw tracknumber mp4file
       - TimeScale の確認: mp4box -info mp4file
       - mp4 ファイルの連結（新規）: mp4box -add mp4file1 -cat mp4file2 -cat mp4file3 -new mp4outputfile
       - mp4 ファイルの連結（既存）: mp4box -cat mp4addfile mp4existfile

     - 使う機会がなくなった。
     - 2009-09-04
   * - `SIMD Enhanced JPEG Plug-in <http://cetus.sakura.ne.jp/softlab/>`_
     - 0.21
     - JPEG を表示。
       `バージョンアップするたびに遅くなっているような気がする。`:strike:
       0.14B で速くなった。
     - JPEG-turbo Susie Plug-in へ。
     - 2006-01-07
   * - `Susie32 PNG Plug-in <http://cetus.sakura.ne.jp/softlab/>`_
     - 0.25
     - PNG を表示。
       0.21 までは ifPNG.spi より明らかに遅かったけれど、0.22 で 0.21 より 1.5 倍ほど高速になったため導入。

       .. code-block:: none

         spibench -t 30 IFPNG024.spi ScreenShot.png

       の結果が 2.2 秒くらい。
     - 使う機会がなくなった。
     - 2007-05-31
   * - `Google 日本語入力 <https://www.google.co.jp/ime/>`_
     - stable
     - 日本語入力。
     - MS-IME がそれなりに使える気がするので新PCでは使っていない。
     - 2013-12-14
   * - `CrystalDiskInfo <http://crystalmark.info/>`_
     - 7.7.0
     - | 操作感の引っ掛かりをなくす。
       | 機能 - 上級者向け機能 - AAM/APM 設定 から対象のディスクを選択してパフォーマンス最高で有効にする。
     - SSD のみの新 PC では必要なくなったっぽい。
     - 2018-09-24
   * - `Process Hacker <http://processhacker.sourceforge.net>`_
     - 2.33
     - プロセスの詳細な情報を表示することができるタスクマネージャ。
     - `Process Explorer に対しては、プロセスが使用中のファイルを探せる機能があるので試している。`:strike: Process Explorer でも探せることが分かったので使わない。
     - 2013-12-29
   * - `IME Cursor <https://shirouzu.jp/tech/IMECursor.htm>`_
     - 1.00
     - マウスカーソルに IME のオン状態を表示。
     - Vivaldi での状態表示がうまくいかない
     - 2019-06-27
   * - `PowerToys <https://github.com/microsoft/PowerToys>`_
     - 0.11.0
     - FancyZones: 画面分割の利用
     - 使わない。
     - 2019-09-07
   * - `lazygit <https://github.com/jesseduffield/lazygit>`_
     - 0.8.1
     - Git の TUI クライアント
     - 表示がくずれるので使わない。
     - 2019-06-27
   * - `SourceTree <https://www.sourcetreeapp.com/>`_
     - 3.1.3
     - Git の GUI クライアント
     - Fork に移行
     - 2019-05-26
   * - `KeePass <http://keepass.sourceforge.net/>`_
     - 1.37
     - オープンソースのパスワード管理ソフト。
       パスワードやユーザ名をコピーして使うには不便なインタフェースだと思っていたけれど、ショートカットキーが使えるのでそうでもなかった。
       Ctrl + V でユーザ ID、パスワードの貼り付けができるが、うまく動かないこともあるため使わないように設定する（ユーザ ID をコピーする Ctrl + B とたまに間違えることがあるので）
       Tools - Options - Advanced - Auto-Type - Enable auto-type features のチェックを外す。
     - KeePassXC へ移行。
     - 2019-01-03

