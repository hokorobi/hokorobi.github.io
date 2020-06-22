Vim plugins
===========

.. list-table:: plugin manager
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - Shougo/dein.vim
     - using
     - | プラグインマネージャ。高速。
       | 遅延読み込みが一番カスタマイズできる（はず）
       | 自動キャッシュ更新が無効にできるようになったので、最近は困ることがない。
     - 2020-02-22

.. list-table:: completion
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - prabirshrestha/asyncomplete.vim
     - using
     -
     -
   * - prabirshrestha/asyncomplete-buffer.vim
     - using
     -
     -
   * - prabirshrestha/asyncomplete-necosyntax.vim
     - using
     -
     -
   * - Shougo/neco-syntax
     - using
     -
     -
   * - prabirshrestha/asyncomplete-necovim.vim
     - using
     -
     -
   * - Shougo/neco-vim
     - using
     -
     -
   * - prabirshrestha/asyncomplete-neosnippet.vim
     - delete
     - neosnippet を asyncomplete で使う。
       日本語の後ろで補完候補がずらっと出てきてしまうので削除。 [2020-05-23]
     - 2020-05-23
   * - hokorobi/asyncomplete-neosnippet.vim
     - using
     - ``let l:kw = matchstr(l:typed, '\w\+$')`` の ``\w`` を ``\k`` に変更してみた。大丈夫そう？
     - 2020-05-23
   * - prabirshrestha/vim-lsp
     - using
     -
     -
   * - mattn/vim-lsp-settings
     - using
     - | vim-lsp の設定をよしなにやってくれる
       | install gopls:

         #. パスの通ったディレクトリに gopls が入っていたら削除
         #. set ft=go の状態で :LspInstallServer を実行して gopls をインストール

     - 2020-02-18
   * - prabirshrestha/asyncomplete-lsp.vim
     - using
     -
     -
   * - high-moctane/asyncomplete-nextword.vim
     - todo
     - 単語の補完
     - 2020-03-22
   * - thomasfaingnaert/vim-lsp-snippets
     - delete
     - LSP で snippet。動かせなかった。
     - 2020-01-19
   * - thomasfaingnaert/vim-lsp-neosnippet
     - delete
     - LSP で neosnippet。動かせなかった。
     - 2020-01-19
   * - Shougo/neosnippet.vim
     - using
     -
     -
   * - Shougo/neosnippet-snippets
     - using
     -
     -
   * - honza/vim-snippets
     - using
     -
     -
   * - coc.nvim
     - delete
     - 補完速度が比較的遅いので asyncomplete.vim に移行。
     -

.. list-table:: REPL?
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - thinca/vim-quickrun
     - using
     -
     -
   * - osyo-manga/shabadou.vim
     - using
     -
     -
   * - rhysd/reply.vim
     - using
     - REPL。ほとんど使っていない。
     - 2020-03-22

.. list-table:: Text Object
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - kana/vim-textobj-user
     - using
     -
     -
   * - mattn/vim-textobj-url
     - using
     -
     -
   * - machakann/vim-sandwich
     - using
     -
     -
   * - machakann/vim-textobj-delimited
     - delete
     - , 区切りの文字の textobj として使っていたけど、vim-swap で代用できることがわかったので削除。
     - 2020-05-17
   * - tommcdo/vim-exchange
     - using
     -
     -
   * - kana/vim-textobj-indent
     - using
     -
     -
   * - glts/vim-textobj-comment
     - using
     -
     -
   * - Julian/vim-textobj-variable-segment
     - using
     -
     -

.. list-table:: filetype
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - AndrewRadev/linediff.vim
     - using
     -
     -
   * - lambdalisue/vim-diffa
     - delete
     - diff を賢くする＋自動アップデートなど。
       Vim 本体だけでも diffopt+=algorithm:histogram,indent-heuristic で賢くなるらしい。
       自動アップデートは使っていないので削除。
     - 2020-03-31
   * - hdima/python-syntax
     - using
     -
     -
   * - hynek/vim-python-pep8-indent
     - using
     -
     -
   * - previm/previm
     - using
     -
     -
   * - plasticboy/vim-markdown
     - using
     -
     -
   * - hokorobi/vim-restructuredtext
     - using
     - marshallward/vim-restructuredtext を Fork。
       Syntax やコマンドを少し追加。
     - 2020-01-18
   * - hokorobi/riv.vim
     - delete
     - gu-fan/riv.vim を Fork。
       restructuredtext を書くのに使っていたけど、色々と気に入らないところがあったので vim-restructuredtext へ移行。
     - 2020-01-18
   * - lambdalisue/qfloc.vim
     - using
     - quickfix を少し便利にする。無効にしているマッピングもそれなりにある。
     - 2020-03-15
   * - romainl/vim-qf
     - todo
     - quickfix を便利に使えるようになるみたい。qfloc.vim より多機能？
     - 2020-03-15
   * - AndrewRadev/quickpeek.vim
     - using
     - Quickfix をポップアップウィンドウでプレビュー
     - 2020-03-22
   * - ronakg/quickr-preview.vim
     - todo
     - Quickfix を別ウィンドウでプレビュー
     - 2020-05-31
   * - vim-jp/syntax-vim-ex
     - using
     -
     -
   * - pangloss/vim-javascript
     - using
     -
     -
   * - PProvost/vim-ps1
     - using
     -
     -
   * - hokorobi/plantuml-syntax
     - using
     - | aklt/plantuml-syntax の fork。
       | 色々といじって PR を送っている。
     - 2020-05-23
   * - tsuyoshicho/plantuml-previewer.vim
     - using
     -
     -
   * - cespare/vim-toml
     - using
     -
     -
   * - osyo-manga/vim-precious
     -
     -
     -
   * - Shougo/context_filetype.vim
     -
     -
     -
   * - hnamikaw/vim-autohotkey
     -
     -
     -
   * - mechatroner/rainbow_csv
     -
     -
     -
   * - mattn/emmet-vim
     -
     -
     -
   * - hokorobi/vim-changelog-alt
     - delete
     - 本体同梱の changelog プラグインを自分好みにしようとしたけど、大して帰るところがなかったので削除。
     - 2020-05-11
   * - hokorobi/vim-howm-syntax-mini
     - using
     -
     -
.. list-table:: Colorscheme
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - rhysd/vim-color-spring-night
     - using
     - colorscheme. iceberg -> spring-night
       italic, bold は無効にしている。
     - 2020-05-11
   * - yasukotelin/shirotelin
     - delete
     - ネタとしては好きだけど、常用するにはちょっと辛く感じた。
     - 2019-11-30

.. list-table:: Look
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - itchyny/lightline.vim
     - using
     - statusline に色々表示。
       tabline は非表示にしている。
     - 2020-05-11
   * - taohexxx/lightline-buffer
     - delete
     - 必要な時だけ :. 相当の表示になるのが好みなので buftabline を使うように戻した。
     - 2019-10-26
   * - mengelbrecht/lightline-bufferline
     - delete
     - こちらも buftabline の方が好みだった。
     - 2019-10-24
   * - osyo-manga/vim-anzu
     - using
     - incremental search の現在のマッチ位置を表示。
     - 2020-05-11
   * - MattesGroeger/vim-bookmarks
     - using
     - ファイルの位置をブックマークしてくれる
       vim-signature へ移行。 [2019-08-04]
       やっぱり使い始めた。 [2020-05-31]
     - 2020-05-31
   * - hokorobi/vim-bookmarks
     - using
     - CtrlP でファイル名を表示できるように変更。 [2020-05-24]
     - 2020-05-24
   * - kshenoy/vim-signature
     - delete
     - | ファイルの位置を Vim の mark に追加してくれる
       | mark を使ってくれるのが良さそうに思えたので vim-bookmarks から移行。 [2019-08-04]
       | 使わないので削除。 [2020-02-18]
       | やはり使いたくなった。
       | :SignatureListGlobalMarks でマークの復元がうまくいかないみたい。
       | vim-bookmarks へ戻る。 [2020-05-24]
     - 2020-05-24
   * - itchyny/vim-cursorword
     - using
     -
     -
   * - andymass/vim-matchup
     - using
     -
     -
   * - t9md/vim-quickhl
     - using
     -
     -
   * - markonm/traces.vim
     - using
     -
     -
   * - liuchengxu/vista.vim
     - using
     -
     -

.. list-table:: Edit
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - cohama/lexima.vim
     - using
     -
     -
   * - machakann/vim-highlightedyank
     - using
     -
     -
   * - kana/vim-operator-replace
     - delete
     - 選択してペーストができるようになると思っていたけど、標準でもできていた。
       レジスタが変わらないのでドットリピートできるけど、そのような使い方はしないかな。
     - 2020-04-01
   * - uplus/vim-clurin
     - using
     -
     -
   * - tpope/vim-speeddating
     - using
     -
     -

.. list-table:: Motion
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - junegunn/vim-easy-align
     - using
     -
     -
   * - mbbill/undotree
     - using
     -
     -
   * - osyo-manga/vim-jplus
     - using
     -
     -
   * - hokorobi/yankround.vim
     - using
     - vim-submode を使って p, P を連続して押して次々過去のレジスタうから貼り付けできるようにしている。
     - 2020-04-02
   * - svermeulen/vim-yoink
     - todo
     - xmap では使えない？　試していないからわからないけれど yankroud.vim で満足している。
       yankround.vim + sub-mode で実現していることが単体でできそう。
     - 2020-04-02
   * - deris/vim-rengbang
     - using
     -
     -
   * - ntpeters/vim-better-whitespace
     - using
     - 末尾スペースを探すときに実行。
     - 2020-05-17
   * - thinca/vim-template
     - using
     -
     -
   * - mattn/vim-sonictemplate
     - using
     - ファイルの新規作成時にテンプレートを挿入。
       snippet のようにテンプレートを展開。
     - 
   * - deris/vim-pasta
     - using
     -
     -
   * - nocd5/ExpandSerialNumber.vim
     - using
     -
     -
   * - lambdalisue/vim-findent
     - using
     - 開いたファイルのインデントに従って Vim のインデントを設定する
     - 2020-04-18
   * - machakann/vim-swap
     - using
     - , 区切りの要素の入れ替え、ソート、textobj
     - 2020-05-17
   * - kana/vim-niceblock
     - using
     - 選択した行すべてに対して I, A を反映させる。
     - 2020-04-18
   * - da-x/name-assign.vim
     - todo
     - 選択した範囲を変数に変えて、その変数の定義を追加する。
     - 2020-05-23
   * - chrisbra/NrrwRgn
     - delete
     - 選択した範囲だけ編集対象とする。
       Vim だと標準で同じようなことができるのでいらなさそう。
       便利な場合もあるんだろうな。
     - 2020-04-18
   * - unblevable/quick-scope
     - delete
     - f, F, t, T でハイライトしてくれる。ルールがよくわからなくて、まともに使っていない。
     - 2020-02-20
   * - easymotion/vim-easymotion
     - using
     -
     -
   * - haya14busa/vim-edgemotion
     - using
     - 縦方向の端に移動
     - 2020-04-18
   * - tyru/columnskip.vim
     - delete
     - edgemotion に近いけど、空白に対してだけスキップ。
       インデントの途中なら、インデントの区切りの位置に移動するのかと思ったけど、違うみたい。
       Vim の設定のせい？
       これなら edgemotion の方が好み。
     - 2020-04-18
   * - machakann/vim-columnmove
     - using
     - f t F T ; , w b e ge W B E gE を縦方向に使える。
     - 2020-04-18
   * - pechorin/any-jump.vim
     - todo
     - 定義にジャンプできるらしい。
       Windows では動かない？　 **:AnyJump** でこんなエラーが出る。::

         function <SNR>17_Jump[35]..search#SearchUsages[4]..<SNR>144_RunRgUsagesSearch の処理中にエラーが検出されました:
         行   14:
         E484: ファイル "C:\Users\hokorobi\AppData\Local\Temp\VIo33AC.tmp" を開けません

     - 2020-04-07
   * - haya14busa/vim-asterisk
     - using
     -
     -
   * - osyo-manga/vim-milfeulle
     - using
     -
     -
   * - hokorobi/vim-smarthome
     - using
     -
     -
   * - osyo-manga/vim-operator-stay-cursor
     - using
     - yank でカーソル移動をさせない。
       ``nnoremap y y`>`` だと不十分なことがあったので。
     - 2020-04-14

.. list-table:: Buffer
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - mhinz/vim-sayonara
     - using
     - | いい感じにバッファを閉じてくれる。
       | filetype に応じた閉じるコマンドの指定もできる。
       | 直前のバッファも一緒に閉じる場合がある。自分の誤操作が原因か？
       | すべてのバッファを閉じると CtrlP で開いたバッファが vsplit される。CtrlP の問題か？
     - 2020-06-07
   * - tyru/capture.vim
     - using
     - コマンドの実行結果などをバッファに取り込んでくれる。
       [nvxstoilc]?map, scriptnames, messages には個別のコマンドを定義して使っている。
     -
   * - ap/vim-buftabline
     - using
     - tabline にバッファを羅列する。タブがある場合はタブを表示。
       同名のバッファがある場合は親ディレクトリも表示。
     - 2020-05-02
   * - mg979/vim-xtabline
     - delete
     - タブを扱えるのは良いけれど、それ以外は buftabline の方がよさそう。機能過剰。
     - 2019-12-02
   * - tyru/closesubwin.vim
     - using
     -
     -

.. list-table:: File
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - kana/vim-gf-user
     - using
     -
     -
   * - kana/vim-gf-diff
     - using
     -
     -
   * - justinmk/vim-dirvish
     - using
     -
     -
   * - lambdalisue/vim-protocol
     - using
     -
     -
   * - mattn/vim-findroot
     - using
     -
     -

.. list-table:: Selector
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - itchyny/vim-gof
     - delete
     - mattn/gof を呼び出してファイル表示など。
       tapi を使っていたので Windows では NG
     - 2020-02-05
   * - ctrlpvim/ctrlp.vim
     - using
     -
     -
   * - hokorobi/ctrlp-sessions
     - using
     -
     -
   * - mattn/ctrlp-launcher
     - using
     -
     -
   * - zeero/vim-ctrlp-help
     - using
     -
     -
   * - ivalkeen/vim-ctrlp-tjump
     - using
     -
     -
   * - ompugao/ctrlp-locate
     - using
     -
     -
   * - tacahiroy/ctrlp-funky
     - using
     -
     -
   * - printesoi/ctrlp-filetype.vim
     - using
     - CtrlP で filetype を指定
     - 2020-06-07
   * - christoomey/ctrlp-generic
     - using
     - 外部コマンドの結果を CtrlP で選択して入力する CtrlPCmdPaste を作成。使っていない…
     - 2020-06-07
   * - suy/vim-ctrlp-commandline
     - using
     - | コマンドラインの履歴を CtrlP で使う。
       | 直接実行だけでなく <C-t> でコマンドラインに表示することができるので、ちょっと変更して再実行も可能。
     - 2020-06-07
   * - mattn/vim-fz
     - delete
     - gof を呼び出してファイルを開く
       Gvim が固まることがあったので、ひとまず使うのをやめた。
     - 2020-04-16
   * - liuchengxu/vim-clap
     - delete
     - 更新すると、まだよく動かなくなることがあるので CtrlP へ戻った。
       CtrlP より若干起動が遅い。
     - 2020-01-03
   * - hokorobi/vim-clap-sessions
     - delete
     - vim-clap を削除したので一緒に削除。
     - 2020-01-03
   * - hokorobi/vim-clap-launcher
     - delete
     - vim-clap を削除したので一緒に削除。
     - 2020-01-03
   * - hokorobi/vim-clap-filelist
     - delete
     - vim-clap でファイル一覧を含んだファイルを候補に使用する provider。
       ``g:clap_provider_mru`` などを定義して source にファイルを読み込めばよいと分かったので使わなくなった。
     - 2019-11-13
   * - Yggdroot/LeaderF
     - todo
     - フィルタリングプラグイン。
       Python を使用しているため、 Windows では起動がちょっと遅そうでまだ試していない。
     - 2020-04-12
   * - prabirshrestha/quickpick.vim
     - todo
     - フィルタリングプラグイン。
       vim-lsp と連携するプラグイン prabirshrestha/quickpick-lsp.vim があるみたい。
     - 2020-05-24

.. list-table:: Utility
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - tyru/vim-altercmd
     - using
     -
     -
   * - kana/vim-altr
     - using
     -
     -
   * - thinca/vim-prettyprint
     - using
     -
     -
   * - tpope/vim-repeat
     - using
     -
     -
   * - mattn/webapi-vim
     - using
     -
     -
   * - ynkdir/vim-vimlparser
     - using
     -
     -
   * - kana/vim-operator-user
     - using
     -
     -
   * - tweekmonster/helpful.vim
     - using
     -
     -
   * - lilydjwg/colorizer
     - using
     -
     -
   * - tyru/open-browser.vim
     - using
     - URL を Web ブラウザで開く。
       'username/repogitory' を Github で開くコマンドを定義している。
     - 2020-02-09
   * - rhysd/wandbox-vim
     - delete
     - wandbox を Vim から使う。
       使うことがなかったので削除。
     - 2019-09-28
   * - tyru/open-browser-unicode.vim
     - using
     -
     -

.. list-table:: Web Service
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - lambdalisue/vim-gista
     - using
     -
     -
   * - mattn/qiita-vim
     - delete
     - Qiita に記事を書く。
       Qiita に書くことがほとんどなく、書く時も Web ブラウザを使うことが多いので削除。
     - 2019-09-28

.. list-table:: Others
   :header-rows: 1

   * - repogitory
     - status
     - comment
     - date
   * - fedorenchik/VimCalc3
     - using
     -
     -
   * - thinca/vim-submode
     - using
     -
     -
   * - lambdalisue/gina.vim
     - using
     -
     -
   * - iberianpig/tig-explorer.vim
     - delete
     - シェルスクリプトを実行するみたいなので Windows では使えなかった。
     - 2020-05-23
   * - vim-jp/vital.vim
     - delete
     -
     -
   * - lambdalisue/vital-Whisky
     - delete
     -
     -
   * - vim-jp/vimdoc-ja
     - using
     -
     -
   * - tyru/empty-prompt.vim
     - using
     -
     -
   * - LeafCage/vimhelpgenerator
     - todo
     - ヘルプのひな型を生成
     - 2020-02-08
   * - rbtnn/vim-mrw
     - todo
     - MRU の書き込み版。出来上がるファイルを vim-fz から開いてみたい。
     - 2020-02-08
   * - tamago324/LeaderF-filer
     - todo
     - CtrlP 的なもの
     - 2020-02-08
   * - dhruvasagar/vim-table-mode
     - delete
     - restructuredtext のテーブルが手軽に書けるはず。
       やはり list-table が便利なので使わなかった。
     - 2020-02-08
   * - vim-voom/VOoM
     - delete
     - restructuredtext のアウトライン表示に使っていた。
       hokorobi/vim-restructuredtext の fold で良さそうなので削除。
     - 2020-02-01
   * - w0rp/ale
     - delete
     - Linter として使っていたけど coc.nvim に移行。
     - 2019-12-08
   * - hokorobi/cmdlineplus.vim
     - delete
     - LeafCage/cmdlineplus.vim を Fork。
       バグ修正の PR がマージされなかったので Fork して使っていた。
       コマンドラインウィンドウを使うことにしたので削除。
     - 2019-12-08
   * - tsuyoshicho/vim-fg
     - delete
     - pt を使って grep を実行。
       grepprg に pt を設定した場合に比べての利点がわからないので一旦削除
     - 2020-02-11

