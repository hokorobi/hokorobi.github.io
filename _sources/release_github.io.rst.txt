Sphinx で生成した html を github.io へ公開
==============================================

こんなんで。

.. code-block:: bash

    $ sphinx-quickstart.exe
    # githubpages: create .nojekyll file to publish the document on GitHub pages (y/n) [n]: には y で回答
    $ make html
    $ cd _build/html
    $ git init
    $ git checkout -b gh-pages
    $ git add *
    $ git add .nojekyll
    $ git commit -m init
    # gh-pages リポジトリを github に作っておく。
    $ git remote add origin https://github.com/hokorobi/gh-pages.git
    $ git push -u origin gh-pages
    # ソースも別のリポジトリに入れておく。
    $ cd ../..
    $ git init
    $ echo _build > .gitignore
    $ git add *
    $ git add .gitignore
    $ git commit -m init
    # github.io.src リポジトリを github に作っておく。
    $ git remote add origin https://github.com/hokorobi/github.io.src.git
    $ git push -u origin master

* ``hokorobi.github.io`` リポジトリだと master ブランチしか公開ができないみたい。
  そして .nojekyll があっても _static の css は公開してくれない様子。
  それ以外のリポジトリでも master で Github pages へ公開すると ``.nojekyll`` があってもダメ。
* ``git submodule`` は使わなかったけど、使ったら嬉しいことあるのかな？
* 参考: `github のプロジェクトにSphinxドキュメントを良さげな感じにおきたい 其の一 - Study08.net 対シンバシ殲滅用人型機動兵器 <http://tell-k.hatenablog.com/entry/2012/01/18/224126>`_

