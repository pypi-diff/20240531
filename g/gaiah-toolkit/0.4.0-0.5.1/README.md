# Comparing `tmp/gaiah_toolkit-0.4.0.tar.gz` & `tmp/gaiah_toolkit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaiah_toolkit-0.4.0.tar", last modified: Sun May 19 08:03:54 2024, max compression
+gzip compressed data, was "gaiah_toolkit-0.5.1.tar", last modified: Fri May 31 15:39:42 2024, max compression
```

## Comparing `gaiah_toolkit-0.4.0.tar` & `gaiah_toolkit-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:03:54.038873 gaiah_toolkit-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-19 08:03:54.038873 gaiah_toolkit-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:03:54.034873 gaiah_toolkit-0.4.0/gaiah/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/gaiah.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/gaiah_commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/gaiah_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/gaiah_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/gaiah/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:03:54.034873 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-19 08:03:54.000000 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-19 08:03:54.000000 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:03:54.000000 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-19 08:03:54.000000 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 08:03:54.000000 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 08:03:54.000000 gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:03:54.038873 gaiah_toolkit-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:03:54.034873 gaiah_toolkit-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-19 08:03:49.000000 gaiah_toolkit-0.4.0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:39:42.460800 gaiah_toolkit-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-05-31 15:39:42.460800 gaiah_toolkit-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:39:42.460800 gaiah_toolkit-0.5.1/gaiah/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/gaiah/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/gaiah/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/gaiah/gaiah.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/gaiah/gaiah_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/gaiah/gaiah_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/gaiah/gaiah_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:39:42.460800 gaiah_toolkit-0.5.1/gaiah/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/gaiah/template/DEMO_README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/gaiah/template/llm_commit_messages.md
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/gaiah/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:39:42.460800 gaiah_toolkit-0.5.1/gaiah_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-05-31 15:39:42.000000 gaiah_toolkit-0.5.1/gaiah_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-31 15:39:42.000000 gaiah_toolkit-0.5.1/gaiah_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:39:42.000000 gaiah_toolkit-0.5.1/gaiah_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 15:39:42.000000 gaiah_toolkit-0.5.1/gaiah_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 15:39:42.000000 gaiah_toolkit-0.5.1/gaiah_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 15:39:42.000000 gaiah_toolkit-0.5.1/gaiah_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:39:42.460800 gaiah_toolkit-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:39:42.460800 gaiah_toolkit-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-31 15:39:38.000000 gaiah_toolkit-0.5.1/tests/test_main.py
```

### Comparing `gaiah_toolkit-0.4.0/LICENSE` & `gaiah_toolkit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gaiah_toolkit-0.4.0/PKG-INFO` & `gaiah_toolkit-0.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiah_toolkit
-Version: 0.4.0
+Version: 0.5.1
 Home-page: https://github.com/your_username/gaiah
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gitpython
@@ -48,121 +48,137 @@
 </p>
 
 >[!IMPORTANT]
 >このリポジトリは[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage)を活用しており、リリースノートやREADME、コミットメッセージの9割は[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ＋ [claude.ai](https://claude.ai/)で生成しています。
 
 ## 🌟 はじめに
 
-Gaiahは、直感的でAIにやさしいメソッドを使用してGit操作を簡素化する革新的なPythonライブラリです。Gitリポジトリを制御するための高レベルなインターフェースを提供し、AIシステムがバージョン管理とシームレスに連携することを容易にします。新機能としてMarkdownから直接コミットを生成する機能が追加され、文書化されたコミットメッセージの管理がさらに効率的に行えます。
+Gaiahは、初心者でも簡単に使えるPythonのライブラリです。Gitを使ってファイルの管理をするのを助けてくれます。新しいバージョンのGaiahでは、Markdownでコミットメッセージをかけるようになりました。
 
-## 🚀 主な特徴
+## 🚀 Gaiahの特徴
 
-- 🤖 **AIフレンドリー**: AI主導の開発プロセスの独自の要件に対応するメソッドとユーティリティを提供し、AIを念頭に置いて設計されています。
-- 🌐 **リモートリポジトリのサポート**: リモートリポジトリとのシームレスな連携を可能にし、GitHubやその他のGitホスティングプラットフォームにリポジトリを作成、クローン、プッシュできるようにします。 
-- 📂 **リポジトリ管理**: 新しいリポジトリの初期化、ファイルの追加、コミットの作成、ブランチの管理をシンプルなPythonコードを介して簡単に行うことができます。
-- 🔧 **カスタマイズ**: 柔軟性とカスタマイズオプションを提供し、特定のニーズと設定に合わせてGitワークフローを調整できます。
-- 📘 **Markdownからのコミット生成**: Markdown形式のドキュメントから直接コミットを生成する機能を追加し、文書化されたコミットメッセージの効率的な管理を可能にします。
+- 🤖 **AIにやさしい**: AIを使った開発に合わせて作られています。
+- 🌐 **リモートリポジトリ**: GitHubなどのサービスとつながります。
+- 📂 **リポジトリ管理**: 新しいリポジトリを作ったり、ファイルを追加したり、コミットしたり、ブランチを管理したりできます。
+- 🔧 **カスタマイズ**: 自分の好みに合わせてGitの使い方を変えられます。
+- 📘 **Markdownでコミット**: Markdownで書いたファイルからコミットメッセージを作れます。
 
-## 📦 インストール
+## 📦 インストールの仕方
 
-Gaiahの使用を開始するには、次の手順に従ってください:
+Gaiahを使うには、次のコマンドを実行してください:
 
-1. 新しいconda環境を作成します:
    ```
-   conda create -n gaiah python=3.11
-   ```
-2. conda環境をアクティベートします:
-   ```
-   conda activate gaiah
-   ```
-3. 必要な依存関係をインストールします:
-   ```
-   pip install gitpython python-dotenv PyGithub termcolor art
+   pip install gaiah-toolkit
    ```
 
-## 🎉 使用方法
+## 🎉 使い方
 
-### CLI
+### コマンドライン
 
-GaiahのCLI機能により、コマンドラインから直接Git操作を行うことができます。例えば、以下のコマンドを使用してリポジトリにコミットを追加することができます:
+Gaiahはコマンドラインから使えます。例えば、こんなふうにコミットできます:
 ```bash
 gaiah
 ```
 
-### 応用的な使い方
-
-特定のプロジェクトディレクトリでGaiahを使用する場合、以下のようにリポジトリの場所やコミットメッセージのファイルパスを指定できます:
-
+もっと細かく指定することもできます:
 ```bash
 gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
 ```
 
-### リポジトリの初期化
+### 新しいリポジトリを作る
 
 ```bash
 gaiah --create_repo --repo_name Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
 ```
 
-## 処理フロー
+### .Gaiah.mdのコミットメッセージを一括送信
+
+Gaiahでは、.Gaiah.mdファイルにMarkdown形式でコミットメッセージをまとめて書いておくことができます。そして、次のコマンドを実行すると、.Gaiah.mdに書かれたコミットメッセージが一括でリポジトリに送信されます:
+
+```bash
+gaiah --process_commits
+```
+
+このコマンドを使えば、たくさんのコミットメッセージを一度に処理できるので、とても便利です。
+
+## Gaiahの中身
+
+Gaiahの処理の流れは、次の図のようになっています:
 
 ```mermaid
 
 graph TD
-   A[ユーザーがCLIを実行] --> B{コマンドライン引数を解析}
-   B --> C{Gaiahオブジェクトを作成}
-   C --> D{--create_repoオプションが指定されている?}
-   D -->|Yes| E[新しいリポジトリをGitHub上に作成]
-   E --> E1[.envファイルから環境変数を読み込む]
-   E1 --> E2[環境変数からアクセストークンを取得]
-   E2 --> E3[GitHubオブジェクトを作成]
-   E3 --> E4[リポジトリ名とパラメータを指定]
-   E4 --> E5[GitHub上に新しいリポジトリを作成]
-   E5 --> E6[リポジトリ作成完了のメッセージを表示]
-   E6 --> Q[処理完了]
-   D -->|No| F{--process_commitsオプションが指定されている?}
-   F -->|Yes| G[コミットメッセージファイルからコミットを処理]
-   G --> H[すべてのファイルをアンステージ]
-   H --> I{コミットセクションごとに処理}
+   A[ユーザーがコマンドを実行] --> B{コマンドを読み取る}
+   B --> C{Gaiahを準備}
+   C --> D{新しいリポジトリを作る?}
+   D -->|Yes| E[GitHubに新しいリポジトリを作る]
+   E --> E1[.envファイルから情報を読む]
+   E1 --> E2[トークンを取得]
+   E2 --> E3[GitHubとつなぐ]
+   E3 --> E4[リポジトリ名などを設定]
+   E4 --> E5[リポジトリを作る]
+   E5 --> E6[完了メッセージを出す]
+   E6 --> Q[おしまい]
+   D -->|No| F{コミットする?}
+   F -->|Yes| G[Markdownファイルからコミットを作る]
+   G --> H[全部のファイルをアンステージ]
+   H --> I{コミットを1つずつ処理}
    I --> J{ファイル名とコミットメッセージを取得}
    J --> K{ファイルを処理}
    K --> L{ファイルをステージ}
    L --> M{変更をコミット}
-   M --> N{次のコミットセクションがある?}
+   M --> N{次のコミットある?}
    N -->|Yes| I
-   N -->|No| O[リモートリポジトリにプッシュ]
-   O --> P[処理完了]
-   F -->|No| Q[処理完了]
+   N -->|No| O[リモートにプッシュ]
+   O --> P[おしまい]
+   F -->|No| Q[おしまい]
 
 ```
 
-## 開発用
+## 開発者向け
 
+1. 新しいconda環境を作ります:
+   ```
+   conda create -n gaiah python=3.11
+   ```
+2. conda環境に入ります:
+   ```
+   conda activate gaiah
+   ```
+3. 必要なものをインストールします:
+   ```
+   pip install gitpython python-dotenv PyGithub termcolor art
+   ```
+
+便利なコマンド:
 ```bash
-gaiah --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits
+script\activate-gaiah.bat
 ```
 
+```bash
+gaiah --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits
+gaiah --create_repo --repo_name AIRA --description "AIRA: AI-Integrated Repository for Accelerated Development" --init_repo --repo_dir C:\Prj\AIRA --process_commits --commit_msg_path .Gaiah.md
+```
 
+## 🤝 みんなでGaiahを良くしよう
 
-
-## 🤝 貢献
-
-Gaiahをさらに良くするために、コミュニティからの貢献を歓迎します。アイデア、提案、バグ報告がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/Gaiah)で issue を開くか、プルリクエストを送信してください。
+Gaiahをもっと良くするアイデアや、バグを見つけたら、[GitHubのページ](https://github.com/Sunwood-ai-labs/Gaiah)で教えてください。
 
 ## 📄 ライセンス
 
-Gaiahは、[MITライセンス](https://opensource.org/licenses/MIT)の下でリリースされており、ライブラリの自由かつオープンソースでの使用、変更、配布が可能です。
+GaiahはMITライセンスで公開されているので、自由に使ったり、変えたり、配ったりできます。
 
-## 🙏 謝辞
+## 🙏 感謝
 
-Gaiahは、以下のライブラリの優れた機能に基づいて構築されています:
+Gaiahは、次のようなすばらしいライブラリのおかげで作ることができました:
 
 - [GitPython](https://github.com/gitpython-developers/GitPython)
 - [python-dotenv](https://github.com/theskumar/python-dotenv)
 - [PyGithub](https://github.com/PyGithub/PyGithub)
 - [termcolor](https://pypi.org/project/termcolor/)
 - [art](https://pypi.org/project/art/)
 
-これらのプロジェクトの開発者とコントリビューターの皆様が、オープンソースコミュニティに貴重な貢献をしてくださったことに感謝します。
+これらを作ってくれた人たちに感謝します。
 
 ---
 
-Gaiahを使用してGitワークフローの自動化を開始し、AI主導の開発の力を解き放ちましょう! 🚀✨
+さあ、Gaiahを使ってGitを楽しく使いこなしましょう! 🚀✨
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gaiah_toolkit Version: 0.4.0 Home-page: https://
+Metadata-Version: 2.1 Name: gaiah_toolkit Version: 0.5.1 Home-page: https://
 github.com/your_username/gaiah Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Version Control Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: gitpython Requires-Dist: python-dotenv Requires-
 Dist: PyGithub Requires-Dist: termcolor Requires-Dist: art
        [https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/
                                Gaiah_icon1.png]
@@ -25,71 +25,69 @@
    llaabbss//GGaaiiaahh??ccoolloorr==oorraannggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//GGaaiiaahh)) **********
    _[[_?ð_?_?_?_ _WW_ee_bb_ss_ii_tt_ee_]] â¢ _[[_?ð_?_?_?±_ _GG_ii_tt_HH_uu_bb_]] _[[_?ð_?_?_?¦_ _TT_ww_ii_tt_tt_ee_rr_]] â¢ _[_ð____ _O_f_f_i_c_i_a_l_ _B_l_o_g_]
 >[!IMPORTANT] >ãã®ãªãã¸ããªã¯[SourceSage](https://github.com/Sunwood-
 ai-labs/
 SourceSage)ãæ´»ç¨ãã¦ããããªãªã¼ã¹ãã¼ããREADMEãã³ãããã¡ãã»ã¼ã¸ã®9å²ã¯
 [SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ï¼ [claude.ai]
 (https://claude.ai/)ã§çæãã¦ãã¾ãã ## ð ã¯ããã«
-Gaiahã¯ãç´æçã§AIã«ããããã¡ã½ãããä½¿ç¨ãã¦Gitæä½ãç°¡ç´ åããé©æ°çãªPythonã©ã¤ãã©ãªã§ããGitãªãã¸ããªãå¶å¾¡ããããã®é«ã¬ãã«ãªã¤ã³ã¿ã¼ãã§ã¼ã¹ãæä¾ããAIã·ã¹ãã ããã¼ã¸ã§ã³ç®¡çã¨ã·ã¼ã ã¬ã¹ã«é£æºãããã¨ãå®¹æã«ãã¾ããæ°æ©è½ã¨ãã¦Markdownããç´æ¥ã³ããããçæããæ©è½ãè¿½å ãããææ¸åãããã³ãããã¡ãã»ã¼ã¸ã®ç®¡çãããã«å¹ççã«è¡ãã¾ãã
-## ð ä¸»ãªç¹å¾´ - ð¤ **AIãã¬ã³ããªã¼**:
-AIä¸»å°ã®éçºãã­ã»ã¹ã®ç¬èªã®è¦ä»¶ã«å¯¾å¿ããã¡ã½ããã¨ã¦ã¼ãã£ãªãã£ãæä¾ããAIãå¿µé ­ã«ç½®ãã¦è¨­è¨ããã¦ãã¾ãã
-- ð **ãªã¢ã¼ããªãã¸ããªã®ãµãã¼ã**:
-ãªã¢ã¼ããªãã¸ããªã¨ã®ã·ã¼ã ã¬ã¹ãªé£æºãå¯è½ã«ããGitHubããã®ä»ã®Gitãã¹ãã£ã³ã°ãã©ãããã©ã¼ã ã«ãªãã¸ããªãä½æãã¯ã­ã¼ã³ãããã·ã¥ã§ããããã«ãã¾ãã
-- ð **ãªãã¸ããªç®¡ç**:
-æ°ãããªãã¸ããªã®åæåããã¡ã¤ã«ã®è¿½å ãã³ãããã®ä½æããã©ã³ãã®ç®¡çãã·ã³ãã«ãªPythonã³ã¼ããä»ãã¦ç°¡åã«è¡ããã¨ãã§ãã¾ãã
+Gaiahã¯ãåå¿èã§ãç°¡åã«ä½¿ããPythonã®ã©ã¤ãã©ãªã§ããGitãä½¿ã£ã¦ãã¡ã¤ã«ã®ç®¡çãããã®ãå©ãã¦ããã¾ããæ°ãããã¼ã¸ã§ã³ã®Gaiahã§ã¯ãMarkdownã§ã³ãããã¡ãã»ã¼ã¸ããããããã«ãªãã¾ããã
+## ð Gaiahã®ç¹å¾´ - ð¤ **AIã«ãããã**:
+AIãä½¿ã£ãéçºã«åããã¦ä½ããã¦ãã¾ãã - ð
+**ãªã¢ã¼ããªãã¸ããª**:
+GitHubãªã©ã®ãµã¼ãã¹ã¨ã¤ãªããã¾ãã - ð
+**ãªãã¸ããªç®¡ç**:
+æ°ãããªãã¸ããªãä½ã£ããããã¡ã¤ã«ãè¿½å ããããã³ããããããããã©ã³ããç®¡çãããã§ãã¾ãã
 - ð§ **ã«ã¹ã¿ãã¤ãº**:
-æè»æ§ã¨ã«ã¹ã¿ãã¤ãºãªãã·ã§ã³ãæä¾ããç¹å®ã®ãã¼ãºã¨è¨­å®ã«åããã¦Gitã¯ã¼ã¯ãã­ã¼ãèª¿æ´ã§ãã¾ãã
-- ð **Markdownããã®ã³ãããçæ**:
-Markdownå½¢å¼ã®ãã­ã¥ã¡ã³ãããç´æ¥ã³ããããçæããæ©è½ãè¿½å ããææ¸åãããã³ãããã¡ãã»ã¼ã¸ã®å¹ççãªç®¡çãå¯è½ã«ãã¾ãã
-## ð¦ ã¤ã³ã¹ãã¼ã«
-Gaiahã®ä½¿ç¨ãéå§ããã«ã¯ãæ¬¡ã®æé ã«å¾ã£ã¦ãã ãã: 1.
-æ°ããcondaç°å¢ãä½æãã¾ã: ``` conda create -n gaiah python=3.11
-``` 2. condaç°å¢ãã¢ã¯ãã£ãã¼ããã¾ã: ``` conda activate gaiah
-``` 3. å¿è¦ãªä¾å­é¢ä¿ãã¤ã³ã¹ãã¼ã«ãã¾ã: ``` pip install
-gitpython python-dotenv PyGithub termcolor art ``` ## ð ä½¿ç¨æ¹æ³ ### CLI
-Gaiahã®CLIæ©è½ã«ãããã³ãã³ãã©ã¤ã³ããç´æ¥Gitæä½ãè¡ããã¨ãã§ãã¾ããä¾ãã°ãä»¥ä¸ã®ã³ãã³ããä½¿ç¨ãã¦ãªãã¸ããªã«ã³ããããè¿½å ãããã¨ãã§ãã¾ã:
-```bash gaiah ``` ### å¿ç¨çãªä½¿ãæ¹
-ç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§Gaiahãä½¿ç¨ããå ´åãä»¥ä¸ã®ããã«ãªãã¸ããªã®å ´æãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãæå®ã§ãã¾ã:
-```bash gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-``` ### ãªãã¸ããªã®åæå ```bash gaiah --create_repo --repo_name
+èªåã®å¥½ã¿ã«åããã¦Gitã®ä½¿ãæ¹ãå¤ãããã¾ãã - ð
+**Markdownã§ã³ããã**:
+Markdownã§æ¸ãããã¡ã¤ã«ããã³ãããã¡ãã»ã¼ã¸ãä½ãã¾ãã
+## ð¦ ã¤ã³ã¹ãã¼ã«ã®ä»æ¹
+Gaiahãä½¿ãã«ã¯ãæ¬¡ã®ã³ãã³ããå®è¡ãã¦ãã ãã: ``` pip
+install gaiah-toolkit ``` ## ð ä½¿ãæ¹ ### ã³ãã³ãã©ã¤ã³
+Gaiahã¯ã³ãã³ãã©ã¤ã³ããä½¿ãã¾ããä¾ãã°ããããªãµãã«ã³ãããã§ãã¾ã:
+```bash gaiah ``` ãã£ã¨ç´°ããæå®ãããã¨ãã§ãã¾ã: ```bash
+gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md ``` ###
+æ°ãããªãã¸ããªãä½ã ```bash gaiah --create_repo --repo_name
 Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:
 \Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
-``` ## å¦çãã­ã¼ ```mermaid graph TD A[ã¦ã¼ã¶ã¼ãCLIãå®è¡] --> B
-{ã³ãã³ãã©ã¤ã³å¼æ°ãè§£æ} B --> C
-{Gaiahãªãã¸ã§ã¯ããä½æ} C --> D{--
-create_repoãªãã·ã§ã³ãæå®ããã¦ãã?} D -->|Yes| E
-[æ°ãããªãã¸ããªãGitHubä¸ã«ä½æ] E --> E1
-[.envãã¡ã¤ã«ããç°å¢å¤æ°ãèª­ã¿è¾¼ã] E1 --> E2
-[ç°å¢å¤æ°ããã¢ã¯ã»ã¹ãã¼ã¯ã³ãåå¾] E2 --> E3
-[GitHubãªãã¸ã§ã¯ããä½æ] E3 --> E4
-[ãªãã¸ããªåã¨ãã©ã¡ã¼ã¿ãæå®] E4 --> E5
-[GitHubä¸ã«æ°ãããªãã¸ããªãä½æ] E5 --> E6
-[ãªãã¸ããªä½æå®äºã®ã¡ãã»ã¼ã¸ãè¡¨ç¤º] E6 --> Q[å¦çå®äº]
-D -->|No| F{--process_commitsãªãã·ã§ã³ãæå®ããã¦ãã?} F --
->|Yes| G[ã³ãããã¡ãã»ã¼ã¸ãã¡ã¤ã«ããã³ããããå¦ç] G
---> H[ãã¹ã¦ã®ãã¡ã¤ã«ãã¢ã³ã¹ãã¼ã¸] H --> I
-{ã³ãããã»ã¯ã·ã§ã³ãã¨ã«å¦ç} I --> J
+``` ### .Gaiah.mdã®ã³ãããã¡ãã»ã¼ã¸ãä¸æ¬éä¿¡
+Gaiahã§ã¯ã.Gaiah.mdãã¡ã¤ã«ã«Markdownå½¢å¼ã§ã³ãããã¡ãã»ã¼ã¸ãã¾ã¨ãã¦æ¸ãã¦ãããã¨ãã§ãã¾ããããã¦ãæ¬¡ã®ã³ãã³ããå®è¡ããã¨ã.Gaiah.mdã«æ¸ãããã³ãããã¡ãã»ã¼ã¸ãä¸æ¬ã§ãªãã¸ããªã«éä¿¡ããã¾ã:
+```bash gaiah --process_commits ```
+ãã®ã³ãã³ããä½¿ãã°ãããããã®ã³ãããã¡ãã»ã¼ã¸ãä¸åº¦ã«å¦çã§ããã®ã§ãã¨ã¦ãä¾¿å©ã§ãã
+## Gaiahã®ä¸­èº«
+Gaiahã®å¦çã®æµãã¯ãæ¬¡ã®å³ã®ããã«ãªã£ã¦ãã¾ã:
+```mermaid graph TD A[ã¦ã¼ã¶ã¼ãã³ãã³ããå®è¡] --> B
+{ã³ãã³ããèª­ã¿åã} B --> C{Gaiahãæºå} C --> D
+{æ°ãããªãã¸ããªãä½ã?} D -->|Yes| E
+[GitHubã«æ°ãããªãã¸ããªãä½ã] E --> E1
+[.envãã¡ã¤ã«ããæå ±ãèª­ã] E1 --> E2[ãã¼ã¯ã³ãåå¾] E2 --
+> E3[GitHubã¨ã¤ãªã] E3 --> E4[ãªãã¸ããªåãªã©ãè¨­å®] E4 --> E5
+[ãªãã¸ããªãä½ã] E5 --> E6[å®äºã¡ãã»ã¼ã¸ãåºã] E6 --> Q
+[ããã¾ã] D -->|No| F{ã³ããããã?} F -->|Yes| G
+[Markdownãã¡ã¤ã«ããã³ããããä½ã] G --> H
+[å¨é¨ã®ãã¡ã¤ã«ãã¢ã³ã¹ãã¼ã¸] H --> I
+{ã³ãããã1ã¤ãã¤å¦ç} I --> J
 {ãã¡ã¤ã«åã¨ã³ãããã¡ãã»ã¼ã¸ãåå¾} J --> K
 {ãã¡ã¤ã«ãå¦ç} K --> L{ãã¡ã¤ã«ãã¹ãã¼ã¸} L --> M
-{å¤æ´ãã³ããã} M --> N{æ¬¡ã®ã³ãããã»ã¯ã·ã§ã³ããã?} N
--->|Yes| I N -->|No| O[ãªã¢ã¼ããªãã¸ããªã«ããã·ã¥] O --> P
-[å¦çå®äº] F -->|No| Q[å¦çå®äº] ``` ## éçºç¨ ```bash gaiah --
-repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits ``` ## ð¤
-è²¢ç®
-Gaiahãããã«è¯ãããããã«ãã³ãã¥ããã£ããã®è²¢ç®ãæ­è¿ãã¾ããã¢ã¤ãã¢ãææ¡ããã°å ±åãããå ´åã¯ã
-[GitHubãªãã¸ããª](https://github.com/Sunwood-ai-labs/Gaiah)ã§ issue
-ãéããããã«ãªã¯ã¨ã¹ããéä¿¡ãã¦ãã ããã ## ð
-ã©ã¤ã»ã³ã¹ Gaiahã¯ã[MITã©ã¤ã»ã³ã¹](https://opensource.org/
-licenses/
-MIT)ã®ä¸ã§ãªãªã¼ã¹ããã¦ãããã©ã¤ãã©ãªã®èªç±ãã¤ãªã¼ãã³ã½ã¼ã¹ã§ã®ä½¿ç¨ãå¤æ´ãéå¸ãå¯è½ã§ãã
-## ð è¬è¾
-Gaiahã¯ãä»¥ä¸ã®ã©ã¤ãã©ãªã®åªããæ©è½ã«åºã¥ãã¦æ§ç¯ããã¦ãã¾ã:
+{å¤æ´ãã³ããã} M --> N{æ¬¡ã®ã³ããããã?} N -->|Yes| I N --
+>|No| O[ãªã¢ã¼ãã«ããã·ã¥] O --> P[ããã¾ã] F -->|No| Q
+[ããã¾ã] ``` ## éçºèåã 1. æ°ããcondaç°å¢ãä½ãã¾ã:
+``` conda create -n gaiah python=3.11 ``` 2. condaç°å¢ã«å¥ãã¾ã: ```
+conda activate gaiah ``` 3. å¿è¦ãªãã®ãã¤ã³ã¹ãã¼ã«ãã¾ã: ```
+pip install gitpython python-dotenv PyGithub termcolor art ```
+ä¾¿å©ãªã³ãã³ã: ```bash script\activate-gaiah.bat ``` ```bash gaiah --
+repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits gaiah --
+create_repo --repo_name AIRA --description "AIRA: AI-Integrated Repository for
+Accelerated Development" --init_repo --repo_dir C:\Prj\AIRA --process_commits -
+-commit_msg_path .Gaiah.md ``` ## ð¤ ã¿ããªã§Gaiahãè¯ãããã
+Gaiahããã£ã¨è¯ãããã¢ã¤ãã¢ãããã°ãè¦ã¤ãããã
+[GitHubã®ãã¼ã¸](https://github.com/Sunwood-ai-labs/
+Gaiah)ã§æãã¦ãã ããã ## ð ã©ã¤ã»ã³ã¹
+Gaiahã¯MITã©ã¤ã»ã³ã¹ã§å¬éããã¦ããã®ã§ãèªç±ã«ä½¿ã£ãããå¤ããããéã£ããã§ãã¾ãã
+## ð æè¬
+Gaiahã¯ãæ¬¡ã®ãããªãã°ãããã©ã¤ãã©ãªã®ãããã§ä½ããã¨ãã§ãã¾ãã:
 - [GitPython](https://github.com/gitpython-developers/GitPython) - [python-
 dotenv](https://github.com/theskumar/python-dotenv) - [PyGithub](https://
 github.com/PyGithub/PyGithub) - [termcolor](https://pypi.org/project/termcolor/
 ) - [art](https://pypi.org/project/art/
-)
-ãããã®ãã­ã¸ã§ã¯ãã®éçºèã¨ã³ã³ããªãã¥ã¼ã¿ã¼ã®çæ§ãããªã¼ãã³ã½ã¼ã¹ã³ãã¥ããã£ã«è²´éãªè²¢ç®ããã¦ãã ãã£ããã¨ã«æè¬ãã¾ãã
---
--
-Gaiahãä½¿ç¨ãã¦Gitã¯ã¼ã¯ãã­ã¼ã®èªååãéå§ããAIä¸»å°ã®éçºã®åãè§£ãæ¾ã¡ã¾ããã!
-ðâ¨
+) ããããä½ã£ã¦ãããäººãã¡ã«æè¬ãã¾ãã --
+- ãããGaiahãä½¿ã£ã¦Gitãæ¥½ããä½¿ãããªãã¾ããã! ðâ¨
```

### Comparing `gaiah_toolkit-0.4.0/README.md` & `gaiah_toolkit-0.5.1/gaiah_toolkit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,153 +1,184 @@
-
-<p align="center">
-<img src="https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/Gaiah_icon1.png" width="100%">
-<br>
-<h1 align="center">Gaiah</h1>
-<h2 align="center">
-  ～Python Git Automation with Innovative Heuristics～
-
-[![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/MakiAi/Gaiah)
-[![Gaiah - Sunwood-ai-labs](https://img.shields.io/static/v1?label=Gaiah&message=Sunwood-ai-labs&color=blue&logo=github)](https://github.com/Gaiah/Sunwood-ai-labs "Go to GitHub repo")
-[![stars - Sunwood-ai-labs](https://img.shields.io/github/stars/Gaiah/Sunwood-ai-labs?style=social)](https://github.com/Gaiah/Sunwood-ai-labs)
-[![forks - Sunwood-ai-labs](https://img.shields.io/github/forks/Gaiah/Sunwood-ai-labs?style=social)](https://github.com/Gaiah/Sunwood-ai-labs)
-[![GitHub Last Commit](https://img.shields.io/github/last-commit/Sunwood-ai-labs/Gaiah)](https://github.com/Sunwood-ai-labs/Gaiah)
-[![GitHub Top Language](https://img.shields.io/github/languages/top/Sunwood-ai-labs/Gaiah)](https://github.com/Sunwood-ai-labs/Gaiah)
-[![GitHub Release](https://img.shields.io/github/v/release/Sunwood-ai-labs/Gaiah?sort=date&color=red)](https://github.com/Sunwood-ai-labs/Gaiah)
-[![GitHub Tag](https://img.shields.io/github/v/tag/Sunwood-ai-labs/Gaiah?color=orange)](https://github.com/Sunwood-ai-labs/Gaiah)
-
-</h2>
-
-<p align="center">
-  <a href="https://hamaruki.com/"><b>[🌐 Website]</b></a> •
-  <!-- <a href="https://arxiv.org/abs/2309.17452"><b>[📜 Paper]</b></a> • -->
-  <!-- <a href="https://huggingface.co/llm-agents"><b>[🤗 HF Models]</b></a> • -->
-  <a href="https://github.com/Sunwood-ai-labs/Gaiah"><b>[🐱 GitHub]</b></a>
-  <!-- <a href="https://9557c5365a6f44dc84.gradio.live"><b>[🐯 Gradio Demo]</b></a> -->
-  <a href="https://twitter.com/hAru_mAki_ch"><b>[🐦 Twitter]</b></a> •
-  <!-- <a href="https://www.reddit.com/r/LocalLLaMA/comments/1703k6d/tora_a_toolintegrated_reasoning_agent_for/"><b>[💬 Reddit]</b></a> • -->
-  <a href="https://hamaruki.com/how-to-control-git-with-python-example-of-using-the-gaiah-library/">[🍀 Official Blog]</a>
-  <!-- <a href="#-quick-start">Quick Start</a> • -->
-  <!-- <a href="#%EF%B8%8F-citation">Citation</a> -->
-</p>
-
-</p>
-
->[!IMPORTANT]
->このリポジトリは[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage)を活用しており、リリースノートやREADME、コミットメッセージの9割は[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ＋ [claude.ai](https://claude.ai/)で生成しています。
-
-## 🌟 はじめに
-
-Gaiahは、直感的でAIにやさしいメソッドを使用してGit操作を簡素化する革新的なPythonライブラリです。Gitリポジトリを制御するための高レベルなインターフェースを提供し、AIシステムがバージョン管理とシームレスに連携することを容易にします。新機能としてMarkdownから直接コミットを生成する機能が追加され、文書化されたコミットメッセージの管理がさらに効率的に行えます。
-
-## 🚀 主な特徴
-
-- 🤖 **AIフレンドリー**: AI主導の開発プロセスの独自の要件に対応するメソッドとユーティリティを提供し、AIを念頭に置いて設計されています。
-- 🌐 **リモートリポジトリのサポート**: リモートリポジトリとのシームレスな連携を可能にし、GitHubやその他のGitホスティングプラットフォームにリポジトリを作成、クローン、プッシュできるようにします。 
-- 📂 **リポジトリ管理**: 新しいリポジトリの初期化、ファイルの追加、コミットの作成、ブランチの管理をシンプルなPythonコードを介して簡単に行うことができます。
-- 🔧 **カスタマイズ**: 柔軟性とカスタマイズオプションを提供し、特定のニーズと設定に合わせてGitワークフローを調整できます。
-- 📘 **Markdownからのコミット生成**: Markdown形式のドキュメントから直接コミットを生成する機能を追加し、文書化されたコミットメッセージの効率的な管理を可能にします。
-
-## 📦 インストール
-
-Gaiahの使用を開始するには、次の手順に従ってください:
-
-1. 新しいconda環境を作成します:
-   ```
-   conda create -n gaiah python=3.11
-   ```
-2. conda環境をアクティベートします:
-   ```
-   conda activate gaiah
-   ```
-3. 必要な依存関係をインストールします:
-   ```
-   pip install gitpython python-dotenv PyGithub termcolor art
-   ```
-
-## 🎉 使用方法
-
-### CLI
-
-GaiahのCLI機能により、コマンドラインから直接Git操作を行うことができます。例えば、以下のコマンドを使用してリポジトリにコミットを追加することができます:
-```bash
-gaiah
-```
-
-### 応用的な使い方
-
-特定のプロジェクトディレクトリでGaiahを使用する場合、以下のようにリポジトリの場所やコミットメッセージのファイルパスを指定できます:
-
-```bash
-gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-```
-
-### リポジトリの初期化
-
-```bash
-gaiah --create_repo --repo_name Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
-```
-
-## 処理フロー
-
-```mermaid
-
-graph TD
-   A[ユーザーがCLIを実行] --> B{コマンドライン引数を解析}
-   B --> C{Gaiahオブジェクトを作成}
-   C --> D{--create_repoオプションが指定されている?}
-   D -->|Yes| E[新しいリポジトリをGitHub上に作成]
-   E --> E1[.envファイルから環境変数を読み込む]
-   E1 --> E2[環境変数からアクセストークンを取得]
-   E2 --> E3[GitHubオブジェクトを作成]
-   E3 --> E4[リポジトリ名とパラメータを指定]
-   E4 --> E5[GitHub上に新しいリポジトリを作成]
-   E5 --> E6[リポジトリ作成完了のメッセージを表示]
-   E6 --> Q[処理完了]
-   D -->|No| F{--process_commitsオプションが指定されている?}
-   F -->|Yes| G[コミットメッセージファイルからコミットを処理]
-   G --> H[すべてのファイルをアンステージ]
-   H --> I{コミットセクションごとに処理}
-   I --> J{ファイル名とコミットメッセージを取得}
-   J --> K{ファイルを処理}
-   K --> L{ファイルをステージ}
-   L --> M{変更をコミット}
-   M --> N{次のコミットセクションがある?}
-   N -->|Yes| I
-   N -->|No| O[リモートリポジトリにプッシュ]
-   O --> P[処理完了]
-   F -->|No| Q[処理完了]
-
-```
-
-## 開発用
-
-```bash
-gaiah --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits
-```
-
-
-
-
-## 🤝 貢献
-
-Gaiahをさらに良くするために、コミュニティからの貢献を歓迎します。アイデア、提案、バグ報告がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/Gaiah)で issue を開くか、プルリクエストを送信してください。
-
-## 📄 ライセンス
-
-Gaiahは、[MITライセンス](https://opensource.org/licenses/MIT)の下でリリースされており、ライブラリの自由かつオープンソースでの使用、変更、配布が可能です。
-
-## 🙏 謝辞
-
-Gaiahは、以下のライブラリの優れた機能に基づいて構築されています:
-
-- [GitPython](https://github.com/gitpython-developers/GitPython)
-- [python-dotenv](https://github.com/theskumar/python-dotenv)
-- [PyGithub](https://github.com/PyGithub/PyGithub)
-- [termcolor](https://pypi.org/project/termcolor/)
-- [art](https://pypi.org/project/art/)
-
-これらのプロジェクトの開発者とコントリビューターの皆様が、オープンソースコミュニティに貴重な貢献をしてくださったことに感謝します。
-
----
-
-Gaiahを使用してGitワークフローの自動化を開始し、AI主導の開発の力を解き放ちましょう! 🚀✨
+Metadata-Version: 2.1
+Name: gaiah_toolkit
+Version: 0.5.1
+Home-page: https://github.com/your_username/gaiah
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Version Control
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: gitpython
+Requires-Dist: python-dotenv
+Requires-Dist: PyGithub
+Requires-Dist: termcolor
+Requires-Dist: art
+
+
+<p align="center">
+<img src="https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/Gaiah_icon1.png" width="100%">
+<br>
+<h1 align="center">Gaiah</h1>
+<h2 align="center">
+  ～Python Git Automation with Innovative Heuristics～
+
+[![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/MakiAi/Gaiah)
+[![Gaiah - Sunwood-ai-labs](https://img.shields.io/static/v1?label=Gaiah&message=Sunwood-ai-labs&color=blue&logo=github)](https://github.com/Gaiah/Sunwood-ai-labs "Go to GitHub repo")
+[![stars - Sunwood-ai-labs](https://img.shields.io/github/stars/Gaiah/Sunwood-ai-labs?style=social)](https://github.com/Gaiah/Sunwood-ai-labs)
+[![forks - Sunwood-ai-labs](https://img.shields.io/github/forks/Gaiah/Sunwood-ai-labs?style=social)](https://github.com/Gaiah/Sunwood-ai-labs)
+[![GitHub Last Commit](https://img.shields.io/github/last-commit/Sunwood-ai-labs/Gaiah)](https://github.com/Sunwood-ai-labs/Gaiah)
+[![GitHub Top Language](https://img.shields.io/github/languages/top/Sunwood-ai-labs/Gaiah)](https://github.com/Sunwood-ai-labs/Gaiah)
+[![GitHub Release](https://img.shields.io/github/v/release/Sunwood-ai-labs/Gaiah?sort=date&color=red)](https://github.com/Sunwood-ai-labs/Gaiah)
+[![GitHub Tag](https://img.shields.io/github/v/tag/Sunwood-ai-labs/Gaiah?color=orange)](https://github.com/Sunwood-ai-labs/Gaiah)
+
+</h2>
+
+<p align="center">
+  <a href="https://hamaruki.com/"><b>[🌐 Website]</b></a> •
+  <!-- <a href="https://arxiv.org/abs/2309.17452"><b>[📜 Paper]</b></a> • -->
+  <!-- <a href="https://huggingface.co/llm-agents"><b>[🤗 HF Models]</b></a> • -->
+  <a href="https://github.com/Sunwood-ai-labs/Gaiah"><b>[🐱 GitHub]</b></a>
+  <!-- <a href="https://9557c5365a6f44dc84.gradio.live"><b>[🐯 Gradio Demo]</b></a> -->
+  <a href="https://twitter.com/hAru_mAki_ch"><b>[🐦 Twitter]</b></a> •
+  <!-- <a href="https://www.reddit.com/r/LocalLLaMA/comments/1703k6d/tora_a_toolintegrated_reasoning_agent_for/"><b>[💬 Reddit]</b></a> • -->
+  <a href="https://hamaruki.com/how-to-control-git-with-python-example-of-using-the-gaiah-library/">[🍀 Official Blog]</a>
+  <!-- <a href="#-quick-start">Quick Start</a> • -->
+  <!-- <a href="#%EF%B8%8F-citation">Citation</a> -->
+</p>
+
+</p>
+
+>[!IMPORTANT]
+>このリポジトリは[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage)を活用しており、リリースノートやREADME、コミットメッセージの9割は[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ＋ [claude.ai](https://claude.ai/)で生成しています。
+
+## 🌟 はじめに
+
+Gaiahは、初心者でも簡単に使えるPythonのライブラリです。Gitを使ってファイルの管理をするのを助けてくれます。新しいバージョンのGaiahでは、Markdownでコミットメッセージをかけるようになりました。
+
+## 🚀 Gaiahの特徴
+
+- 🤖 **AIにやさしい**: AIを使った開発に合わせて作られています。
+- 🌐 **リモートリポジトリ**: GitHubなどのサービスとつながります。
+- 📂 **リポジトリ管理**: 新しいリポジトリを作ったり、ファイルを追加したり、コミットしたり、ブランチを管理したりできます。
+- 🔧 **カスタマイズ**: 自分の好みに合わせてGitの使い方を変えられます。
+- 📘 **Markdownでコミット**: Markdownで書いたファイルからコミットメッセージを作れます。
+
+## 📦 インストールの仕方
+
+Gaiahを使うには、次のコマンドを実行してください:
+
+   ```
+   pip install gaiah-toolkit
+   ```
+
+## 🎉 使い方
+
+### コマンドライン
+
+Gaiahはコマンドラインから使えます。例えば、こんなふうにコミットできます:
+```bash
+gaiah
+```
+
+もっと細かく指定することもできます:
+```bash
+gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
+```
+
+### 新しいリポジトリを作る
+
+```bash
+gaiah --create_repo --repo_name Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
+```
+
+### .Gaiah.mdのコミットメッセージを一括送信
+
+Gaiahでは、.Gaiah.mdファイルにMarkdown形式でコミットメッセージをまとめて書いておくことができます。そして、次のコマンドを実行すると、.Gaiah.mdに書かれたコミットメッセージが一括でリポジトリに送信されます:
+
+```bash
+gaiah --process_commits
+```
+
+このコマンドを使えば、たくさんのコミットメッセージを一度に処理できるので、とても便利です。
+
+## Gaiahの中身
+
+Gaiahの処理の流れは、次の図のようになっています:
+
+```mermaid
+
+graph TD
+   A[ユーザーがコマンドを実行] --> B{コマンドを読み取る}
+   B --> C{Gaiahを準備}
+   C --> D{新しいリポジトリを作る?}
+   D -->|Yes| E[GitHubに新しいリポジトリを作る]
+   E --> E1[.envファイルから情報を読む]
+   E1 --> E2[トークンを取得]
+   E2 --> E3[GitHubとつなぐ]
+   E3 --> E4[リポジトリ名などを設定]
+   E4 --> E5[リポジトリを作る]
+   E5 --> E6[完了メッセージを出す]
+   E6 --> Q[おしまい]
+   D -->|No| F{コミットする?}
+   F -->|Yes| G[Markdownファイルからコミットを作る]
+   G --> H[全部のファイルをアンステージ]
+   H --> I{コミットを1つずつ処理}
+   I --> J{ファイル名とコミットメッセージを取得}
+   J --> K{ファイルを処理}
+   K --> L{ファイルをステージ}
+   L --> M{変更をコミット}
+   M --> N{次のコミットある?}
+   N -->|Yes| I
+   N -->|No| O[リモートにプッシュ]
+   O --> P[おしまい]
+   F -->|No| Q[おしまい]
+
+```
+
+## 開発者向け
+
+1. 新しいconda環境を作ります:
+   ```
+   conda create -n gaiah python=3.11
+   ```
+2. conda環境に入ります:
+   ```
+   conda activate gaiah
+   ```
+3. 必要なものをインストールします:
+   ```
+   pip install gitpython python-dotenv PyGithub termcolor art
+   ```
+
+便利なコマンド:
+```bash
+script\activate-gaiah.bat
+```
+
+```bash
+gaiah --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits
+gaiah --create_repo --repo_name AIRA --description "AIRA: AI-Integrated Repository for Accelerated Development" --init_repo --repo_dir C:\Prj\AIRA --process_commits --commit_msg_path .Gaiah.md
+```
+
+## 🤝 みんなでGaiahを良くしよう
+
+Gaiahをもっと良くするアイデアや、バグを見つけたら、[GitHubのページ](https://github.com/Sunwood-ai-labs/Gaiah)で教えてください。
+
+## 📄 ライセンス
+
+GaiahはMITライセンスで公開されているので、自由に使ったり、変えたり、配ったりできます。
+
+## 🙏 感謝
+
+Gaiahは、次のようなすばらしいライブラリのおかげで作ることができました:
+
+- [GitPython](https://github.com/gitpython-developers/GitPython)
+- [python-dotenv](https://github.com/theskumar/python-dotenv)
+- [PyGithub](https://github.com/PyGithub/PyGithub)
+- [termcolor](https://pypi.org/project/termcolor/)
+- [art](https://pypi.org/project/art/)
+
+これらを作ってくれた人たちに感謝します。
+
+---
+
+さあ、Gaiahを使ってGitを楽しく使いこなしましょう! 🚀✨
```

#### html2text {}

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1 Name: gaiah_toolkit Version: 0.5.1 Home-page: https://
+github.com/your_username/gaiah Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers Classifier: Topic :: Software
+Development :: Version Control Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: gitpython Requires-Dist: python-dotenv Requires-
+Dist: PyGithub Requires-Dist: termcolor Requires-Dist: art
        [https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/
                                Gaiah_icon1.png]
                               ************ GGaaiiaahh ************
  ********** ?ï?½?PPyytthhoonn GGiitt AAuuttoommaattiioonn wwiitthh IInnnnoovvaattiivvee HHeeuurriissttiiccss?ï?½? [[!![[HHuuggggiinngg FFaaccee
   SSppaacceess]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//bbaaddggee//%%FF00%%99FF%%AA44%%9977%%2200HHuuggggiinngg%%2200FFaaccee--SSppaacceess--
 bblluuee))]]((hhttttppss::////hhuuggggiinnggffaaccee..ccoo//ssppaacceess//MMaakkiiAAii//GGaaiiaahh)) [[!![[GGaaiiaahh -- SSuunnwwoooodd--aaii--llaabbss]]
        ((hhttttppss::////iimmgg..sshhiieellddss..iioo//ssttaattiicc//vv11??llaabbeell==GGaaiiaahh&&mmeessssaaggee==SSuunnwwoooodd--aaii--
@@ -19,71 +25,69 @@
    llaabbss//GGaaiiaahh??ccoolloorr==oorraannggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//GGaaiiaahh)) **********
    _[[_?ð_?_?_?_ _WW_ee_bb_ss_ii_tt_ee_]] â¢ _[[_?ð_?_?_?±_ _GG_ii_tt_HH_uu_bb_]] _[[_?ð_?_?_?¦_ _TT_ww_ii_tt_tt_ee_rr_]] â¢ _[_ð____ _O_f_f_i_c_i_a_l_ _B_l_o_g_]
 >[!IMPORTANT] >ãã®ãªãã¸ããªã¯[SourceSage](https://github.com/Sunwood-
 ai-labs/
 SourceSage)ãæ´»ç¨ãã¦ããããªãªã¼ã¹ãã¼ããREADMEãã³ãããã¡ãã»ã¼ã¸ã®9å²ã¯
 [SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ï¼ [claude.ai]
 (https://claude.ai/)ã§çæãã¦ãã¾ãã ## ð ã¯ããã«
-Gaiahã¯ãç´æçã§AIã«ããããã¡ã½ãããä½¿ç¨ãã¦Gitæä½ãç°¡ç´ åããé©æ°çãªPythonã©ã¤ãã©ãªã§ããGitãªãã¸ããªãå¶å¾¡ããããã®é«ã¬ãã«ãªã¤ã³ã¿ã¼ãã§ã¼ã¹ãæä¾ããAIã·ã¹ãã ããã¼ã¸ã§ã³ç®¡çã¨ã·ã¼ã ã¬ã¹ã«é£æºãããã¨ãå®¹æã«ãã¾ããæ°æ©è½ã¨ãã¦Markdownããç´æ¥ã³ããããçæããæ©è½ãè¿½å ãããææ¸åãããã³ãããã¡ãã»ã¼ã¸ã®ç®¡çãããã«å¹ççã«è¡ãã¾ãã
-## ð ä¸»ãªç¹å¾´ - ð¤ **AIãã¬ã³ããªã¼**:
-AIä¸»å°ã®éçºãã­ã»ã¹ã®ç¬èªã®è¦ä»¶ã«å¯¾å¿ããã¡ã½ããã¨ã¦ã¼ãã£ãªãã£ãæä¾ããAIãå¿µé ­ã«ç½®ãã¦è¨­è¨ããã¦ãã¾ãã
-- ð **ãªã¢ã¼ããªãã¸ããªã®ãµãã¼ã**:
-ãªã¢ã¼ããªãã¸ããªã¨ã®ã·ã¼ã ã¬ã¹ãªé£æºãå¯è½ã«ããGitHubããã®ä»ã®Gitãã¹ãã£ã³ã°ãã©ãããã©ã¼ã ã«ãªãã¸ããªãä½æãã¯ã­ã¼ã³ãããã·ã¥ã§ããããã«ãã¾ãã
-- ð **ãªãã¸ããªç®¡ç**:
-æ°ãããªãã¸ããªã®åæåããã¡ã¤ã«ã®è¿½å ãã³ãããã®ä½æããã©ã³ãã®ç®¡çãã·ã³ãã«ãªPythonã³ã¼ããä»ãã¦ç°¡åã«è¡ããã¨ãã§ãã¾ãã
+Gaiahã¯ãåå¿èã§ãç°¡åã«ä½¿ããPythonã®ã©ã¤ãã©ãªã§ããGitãä½¿ã£ã¦ãã¡ã¤ã«ã®ç®¡çãããã®ãå©ãã¦ããã¾ããæ°ãããã¼ã¸ã§ã³ã®Gaiahã§ã¯ãMarkdownã§ã³ãããã¡ãã»ã¼ã¸ããããããã«ãªãã¾ããã
+## ð Gaiahã®ç¹å¾´ - ð¤ **AIã«ãããã**:
+AIãä½¿ã£ãéçºã«åããã¦ä½ããã¦ãã¾ãã - ð
+**ãªã¢ã¼ããªãã¸ããª**:
+GitHubãªã©ã®ãµã¼ãã¹ã¨ã¤ãªããã¾ãã - ð
+**ãªãã¸ããªç®¡ç**:
+æ°ãããªãã¸ããªãä½ã£ããããã¡ã¤ã«ãè¿½å ããããã³ããããããããã©ã³ããç®¡çãããã§ãã¾ãã
 - ð§ **ã«ã¹ã¿ãã¤ãº**:
-æè»æ§ã¨ã«ã¹ã¿ãã¤ãºãªãã·ã§ã³ãæä¾ããç¹å®ã®ãã¼ãºã¨è¨­å®ã«åããã¦Gitã¯ã¼ã¯ãã­ã¼ãèª¿æ´ã§ãã¾ãã
-- ð **Markdownããã®ã³ãããçæ**:
-Markdownå½¢å¼ã®ãã­ã¥ã¡ã³ãããç´æ¥ã³ããããçæããæ©è½ãè¿½å ããææ¸åãããã³ãããã¡ãã»ã¼ã¸ã®å¹ççãªç®¡çãå¯è½ã«ãã¾ãã
-## ð¦ ã¤ã³ã¹ãã¼ã«
-Gaiahã®ä½¿ç¨ãéå§ããã«ã¯ãæ¬¡ã®æé ã«å¾ã£ã¦ãã ãã: 1.
-æ°ããcondaç°å¢ãä½æãã¾ã: ``` conda create -n gaiah python=3.11
-``` 2. condaç°å¢ãã¢ã¯ãã£ãã¼ããã¾ã: ``` conda activate gaiah
-``` 3. å¿è¦ãªä¾å­é¢ä¿ãã¤ã³ã¹ãã¼ã«ãã¾ã: ``` pip install
-gitpython python-dotenv PyGithub termcolor art ``` ## ð ä½¿ç¨æ¹æ³ ### CLI
-Gaiahã®CLIæ©è½ã«ãããã³ãã³ãã©ã¤ã³ããç´æ¥Gitæä½ãè¡ããã¨ãã§ãã¾ããä¾ãã°ãä»¥ä¸ã®ã³ãã³ããä½¿ç¨ãã¦ãªãã¸ããªã«ã³ããããè¿½å ãããã¨ãã§ãã¾ã:
-```bash gaiah ``` ### å¿ç¨çãªä½¿ãæ¹
-ç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§Gaiahãä½¿ç¨ããå ´åãä»¥ä¸ã®ããã«ãªãã¸ããªã®å ´æãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãæå®ã§ãã¾ã:
-```bash gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-``` ### ãªãã¸ããªã®åæå ```bash gaiah --create_repo --repo_name
+èªåã®å¥½ã¿ã«åããã¦Gitã®ä½¿ãæ¹ãå¤ãããã¾ãã - ð
+**Markdownã§ã³ããã**:
+Markdownã§æ¸ãããã¡ã¤ã«ããã³ãããã¡ãã»ã¼ã¸ãä½ãã¾ãã
+## ð¦ ã¤ã³ã¹ãã¼ã«ã®ä»æ¹
+Gaiahãä½¿ãã«ã¯ãæ¬¡ã®ã³ãã³ããå®è¡ãã¦ãã ãã: ``` pip
+install gaiah-toolkit ``` ## ð ä½¿ãæ¹ ### ã³ãã³ãã©ã¤ã³
+Gaiahã¯ã³ãã³ãã©ã¤ã³ããä½¿ãã¾ããä¾ãã°ããããªãµãã«ã³ãããã§ãã¾ã:
+```bash gaiah ``` ãã£ã¨ç´°ããæå®ãããã¨ãã§ãã¾ã: ```bash
+gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md ``` ###
+æ°ãããªãã¸ããªãä½ã ```bash gaiah --create_repo --repo_name
 Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:
 \Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
-``` ## å¦çãã­ã¼ ```mermaid graph TD A[ã¦ã¼ã¶ã¼ãCLIãå®è¡] --> B
-{ã³ãã³ãã©ã¤ã³å¼æ°ãè§£æ} B --> C
-{Gaiahãªãã¸ã§ã¯ããä½æ} C --> D{--
-create_repoãªãã·ã§ã³ãæå®ããã¦ãã?} D -->|Yes| E
-[æ°ãããªãã¸ããªãGitHubä¸ã«ä½æ] E --> E1
-[.envãã¡ã¤ã«ããç°å¢å¤æ°ãèª­ã¿è¾¼ã] E1 --> E2
-[ç°å¢å¤æ°ããã¢ã¯ã»ã¹ãã¼ã¯ã³ãåå¾] E2 --> E3
-[GitHubãªãã¸ã§ã¯ããä½æ] E3 --> E4
-[ãªãã¸ããªåã¨ãã©ã¡ã¼ã¿ãæå®] E4 --> E5
-[GitHubä¸ã«æ°ãããªãã¸ããªãä½æ] E5 --> E6
-[ãªãã¸ããªä½æå®äºã®ã¡ãã»ã¼ã¸ãè¡¨ç¤º] E6 --> Q[å¦çå®äº]
-D -->|No| F{--process_commitsãªãã·ã§ã³ãæå®ããã¦ãã?} F --
->|Yes| G[ã³ãããã¡ãã»ã¼ã¸ãã¡ã¤ã«ããã³ããããå¦ç] G
---> H[ãã¹ã¦ã®ãã¡ã¤ã«ãã¢ã³ã¹ãã¼ã¸] H --> I
-{ã³ãããã»ã¯ã·ã§ã³ãã¨ã«å¦ç} I --> J
+``` ### .Gaiah.mdã®ã³ãããã¡ãã»ã¼ã¸ãä¸æ¬éä¿¡
+Gaiahã§ã¯ã.Gaiah.mdãã¡ã¤ã«ã«Markdownå½¢å¼ã§ã³ãããã¡ãã»ã¼ã¸ãã¾ã¨ãã¦æ¸ãã¦ãããã¨ãã§ãã¾ããããã¦ãæ¬¡ã®ã³ãã³ããå®è¡ããã¨ã.Gaiah.mdã«æ¸ãããã³ãããã¡ãã»ã¼ã¸ãä¸æ¬ã§ãªãã¸ããªã«éä¿¡ããã¾ã:
+```bash gaiah --process_commits ```
+ãã®ã³ãã³ããä½¿ãã°ãããããã®ã³ãããã¡ãã»ã¼ã¸ãä¸åº¦ã«å¦çã§ããã®ã§ãã¨ã¦ãä¾¿å©ã§ãã
+## Gaiahã®ä¸­èº«
+Gaiahã®å¦çã®æµãã¯ãæ¬¡ã®å³ã®ããã«ãªã£ã¦ãã¾ã:
+```mermaid graph TD A[ã¦ã¼ã¶ã¼ãã³ãã³ããå®è¡] --> B
+{ã³ãã³ããèª­ã¿åã} B --> C{Gaiahãæºå} C --> D
+{æ°ãããªãã¸ããªãä½ã?} D -->|Yes| E
+[GitHubã«æ°ãããªãã¸ããªãä½ã] E --> E1
+[.envãã¡ã¤ã«ããæå ±ãèª­ã] E1 --> E2[ãã¼ã¯ã³ãåå¾] E2 --
+> E3[GitHubã¨ã¤ãªã] E3 --> E4[ãªãã¸ããªåãªã©ãè¨­å®] E4 --> E5
+[ãªãã¸ããªãä½ã] E5 --> E6[å®äºã¡ãã»ã¼ã¸ãåºã] E6 --> Q
+[ããã¾ã] D -->|No| F{ã³ããããã?} F -->|Yes| G
+[Markdownãã¡ã¤ã«ããã³ããããä½ã] G --> H
+[å¨é¨ã®ãã¡ã¤ã«ãã¢ã³ã¹ãã¼ã¸] H --> I
+{ã³ãããã1ã¤ãã¤å¦ç} I --> J
 {ãã¡ã¤ã«åã¨ã³ãããã¡ãã»ã¼ã¸ãåå¾} J --> K
 {ãã¡ã¤ã«ãå¦ç} K --> L{ãã¡ã¤ã«ãã¹ãã¼ã¸} L --> M
-{å¤æ´ãã³ããã} M --> N{æ¬¡ã®ã³ãããã»ã¯ã·ã§ã³ããã?} N
--->|Yes| I N -->|No| O[ãªã¢ã¼ããªãã¸ããªã«ããã·ã¥] O --> P
-[å¦çå®äº] F -->|No| Q[å¦çå®äº] ``` ## éçºç¨ ```bash gaiah --
-repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits ``` ## ð¤
-è²¢ç®
-Gaiahãããã«è¯ãããããã«ãã³ãã¥ããã£ããã®è²¢ç®ãæ­è¿ãã¾ããã¢ã¤ãã¢ãææ¡ããã°å ±åãããå ´åã¯ã
-[GitHubãªãã¸ããª](https://github.com/Sunwood-ai-labs/Gaiah)ã§ issue
-ãéããããã«ãªã¯ã¨ã¹ããéä¿¡ãã¦ãã ããã ## ð
-ã©ã¤ã»ã³ã¹ Gaiahã¯ã[MITã©ã¤ã»ã³ã¹](https://opensource.org/
-licenses/
-MIT)ã®ä¸ã§ãªãªã¼ã¹ããã¦ãããã©ã¤ãã©ãªã®èªç±ãã¤ãªã¼ãã³ã½ã¼ã¹ã§ã®ä½¿ç¨ãå¤æ´ãéå¸ãå¯è½ã§ãã
-## ð è¬è¾
-Gaiahã¯ãä»¥ä¸ã®ã©ã¤ãã©ãªã®åªããæ©è½ã«åºã¥ãã¦æ§ç¯ããã¦ãã¾ã:
+{å¤æ´ãã³ããã} M --> N{æ¬¡ã®ã³ããããã?} N -->|Yes| I N --
+>|No| O[ãªã¢ã¼ãã«ããã·ã¥] O --> P[ããã¾ã] F -->|No| Q
+[ããã¾ã] ``` ## éçºèåã 1. æ°ããcondaç°å¢ãä½ãã¾ã:
+``` conda create -n gaiah python=3.11 ``` 2. condaç°å¢ã«å¥ãã¾ã: ```
+conda activate gaiah ``` 3. å¿è¦ãªãã®ãã¤ã³ã¹ãã¼ã«ãã¾ã: ```
+pip install gitpython python-dotenv PyGithub termcolor art ```
+ä¾¿å©ãªã³ãã³ã: ```bash script\activate-gaiah.bat ``` ```bash gaiah --
+repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits gaiah --
+create_repo --repo_name AIRA --description "AIRA: AI-Integrated Repository for
+Accelerated Development" --init_repo --repo_dir C:\Prj\AIRA --process_commits -
+-commit_msg_path .Gaiah.md ``` ## ð¤ ã¿ããªã§Gaiahãè¯ãããã
+Gaiahããã£ã¨è¯ãããã¢ã¤ãã¢ãããã°ãè¦ã¤ãããã
+[GitHubã®ãã¼ã¸](https://github.com/Sunwood-ai-labs/
+Gaiah)ã§æãã¦ãã ããã ## ð ã©ã¤ã»ã³ã¹
+Gaiahã¯MITã©ã¤ã»ã³ã¹ã§å¬éããã¦ããã®ã§ãèªç±ã«ä½¿ã£ãããå¤ããããéã£ããã§ãã¾ãã
+## ð æè¬
+Gaiahã¯ãæ¬¡ã®ãããªãã°ãããã©ã¤ãã©ãªã®ãããã§ä½ããã¨ãã§ãã¾ãã:
 - [GitPython](https://github.com/gitpython-developers/GitPython) - [python-
 dotenv](https://github.com/theskumar/python-dotenv) - [PyGithub](https://
 github.com/PyGithub/PyGithub) - [termcolor](https://pypi.org/project/termcolor/
 ) - [art](https://pypi.org/project/art/
-)
-ãããã®ãã­ã¸ã§ã¯ãã®éçºèã¨ã³ã³ããªãã¥ã¼ã¿ã¼ã®çæ§ãããªã¼ãã³ã½ã¼ã¹ã³ãã¥ããã£ã«è²´éãªè²¢ç®ããã¦ãã ãã£ããã¨ã«æè¬ãã¾ãã
---
--
-Gaiahãä½¿ç¨ãã¦Gitã¯ã¼ã¯ãã­ã¼ã®èªååãéå§ããAIä¸»å°ã®éçºã®åãè§£ãæ¾ã¡ã¾ããã!
-ðâ¨
+) ããããä½ã£ã¦ãããäººãã¡ã«æè¬ãã¾ãã --
+- ãããGaiahãä½¿ã£ã¦Gitãæ¥½ããä½¿ãããªãã¾ããã! ðâ¨
```

### Comparing `gaiah_toolkit-0.4.0/gaiah/cli.py` & `gaiah_toolkit-0.5.1/gaiah/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,55 +25,21 @@
     parser.add_argument('--description', default='', help='リポジトリの説明')
     parser.add_argument('--private', action='store_true', help='プライベートリポジトリとして作成する')
     
     parser.add_argument('--init_repo', action='store_true', help='既存のディレクトリをGitリポジトリとして初期化する')
     parser.add_argument('--repo_dir', default='./', help='初期化するディレクトリのパス')
     parser.add_argument('--no_initial_commit', action='store_true', help='初期コミットを作成しない')
     
+    parser.add_argument('--branch_name', default=None, help='コミットに使用するブランチ名')
     parser.add_argument('--process_commits', action='store_true', help='マークダウンファイルから複数のコミットを行う')
     parser.add_argument('--commit_msg_path', default='.Gaiah.md', help='コミットメッセージファイルのパス')
 
     return parser.parse_args()
 
-
 def main():
     args = parse_arguments()
-
-    tprint("!  Gaiahへようこそ  !")
-
-    repo_dir = args.repo_dir if args.init_repo or args.process_commits else None
-    commit_msg_path = args.commit_msg_path if args.process_commits else None
-    gaiah = Gaiah(repo_dir, commit_msg_path)
-
-    if args.init_repo:
-        gaiah.init_local_repo(args.repo_dir, not args.no_initial_commit)
-
-    if args.create_repo:
-        repo_params = {
-            'description': args.description,
-            'private': args.private
-        }
-        logger.info(">>> リモートリポジトリを作成しています...")
-        gaiah.create_remote_repo(args.repo_name, repo_params)
-        
-        logger.info(">>> ブランチを作成しています...")
-        gaiah.create_branches()
-        
-        logger.info(">>> 初期ファイルを追加しています...")
-        gaiah.add_initial_files()
-        
-        logger.info(">>> 初期ファイルをコミットしています...")
-        gaiah.commit_initial_files()
-        
-        logger.info(">>> ブランチをマージしています...")
-        gaiah.merge_branches()
-        
-        logger.info(">>> マージしたブランチをプッシュしています...")
-        gaiah.push_merged_branches()
-
-    if args.process_commits:
-        gaiah.process_commits()
-
-    logger.success("全ての操作が正常に完了しました!")
+    tprint("!  Welcome to Gaiah  !")
+    gaiah = Gaiah(args)
+    gaiah.run()
 
 if __name__ == "__main__":
     main()
```

### Comparing `gaiah_toolkit-0.4.0/gaiah/gaiah_commit.py` & `gaiah_toolkit-0.5.1/gaiah/gaiah_commit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from loguru import logger
-from .utils import run_command
+from .utils import run_command, tqdm_sleep
 import os
 
 class GaiahCommit:
     FILENAME_REGEX = r'(?m)^###\s(.+)'
     COMMIT_MESSAGE_REGEX = r'```commit-msg\n(.*?)\n```'
 
     def __init__(self, repo):
@@ -65,15 +65,16 @@
             os.remove(commit_message_file)
             self.logger.success("Committed changes.")
 
         except Exception as e:
             self.logger.error(f"Error while committing changes: {e}")
             raise
 
-    def process_commits(self):
+
+    def process_commits(self, branch_name=None):
         """
         コミットメッセージファイルからコミットを処理する
         """
         try:
             with open(self.repo.commit_messages_path, "r", encoding="utf-8") as file:
                 content = file.read()
         except FileNotFoundError:
@@ -81,34 +82,38 @@
             self.logger.info(f"Creating an empty commit messages file: {self.repo.commit_messages_path}")
             with open(self.repo.commit_messages_path, "w", encoding="utf-8") as file:
                 file.write("")
             return
 
         branch_sections = re.split(r'(?m)^##\s(.+)', content)[1:]
 
+        self.unstage_files()
+        tqdm_sleep(5)
+        # ステージされているファイルをアンステージ
+        # run_command(["git", "reset"], cwd=self.repo.repo_dir)
+
         for i in range(0, len(branch_sections), 2):
-            branch_name = branch_sections[i].strip()
+            file_branch_name = branch_sections[i].strip()
             branch_content = branch_sections[i + 1]
 
             commits = re.split(self.FILENAME_REGEX, branch_content)
             if commits and not commits[0].strip():
                 commits = commits[1:]
 
             for j in range(0, len(commits), 2):
                 filename = commits[j].strip()
                 commit_message_section = commits[j + 1]
-                self.process_commit_section(filename, commit_message_section, branch_name)
+                self.process_commit_section(filename, commit_message_section, branch_name or file_branch_name)
 
-            # self.repo.push_to_remote(branch_name=branch_name)
-            
             # developブランチにマージ
-            self.repo.merge_to_develop(branch_name)
-            
+            self.repo.merge_to_develop(branch_name or file_branch_name)
+
             # マージ後のブランチを削除
-            self.repo.delete_branch(branch_name)
+            self.repo.delete_branch(branch_name or file_branch_name)
+
 
     def process_commit_section(self, filename, commit_message_section, branch_name):
         """
         コミットセクションを処理する
         """
         commit_message_match = re.search(self.COMMIT_MESSAGE_REGEX, commit_message_section, re.DOTALL)
         if commit_message_match:
@@ -130,22 +135,25 @@
     def process_file(self, filename, commit_message, branch_name=None):
         """
         ファイルを処理する
         """
         try:
             if os.path.exists(os.path.join(self.repo.repo_dir, filename)):
                 self.stage_file(filename, "modified")
+                self.logger.info("file is modified")
             else:
                 self.stage_file(filename, "deleted")
+                self.logger.info("file is deleted")
 
             changed_files = run_command(["git", "diff", "--staged", "--name-only"], cwd=self.repo.repo_dir).splitlines()
-
+            
+            self.logger.info(f"changed_files is {changed_files}")
             if filename in changed_files:
                 self.commit_changes(commit_message, branch_name)
                 # self.repo.push_to_remote(branch_name=branch_name)
             else:
                 self.logger.info(f"No changes detected in file: {filename}")
-                self.unstage_files()
+                # self.unstage_files()
 
         except Exception as e:
             self.logger.error(f"Error while processing file: {filename} - {e}")
             raise
```

### Comparing `gaiah_toolkit-0.4.0/gaiah/gaiah_github.py` & `gaiah_toolkit-0.5.1/gaiah/gaiah_github.py`

 * *Files identical despite different names*

### Comparing `gaiah_toolkit-0.4.0/gaiah/gaiah_repo.py` & `gaiah_toolkit-0.5.1/gaiah/gaiah_repo.py`

 * *Files identical despite different names*

### Comparing `gaiah_toolkit-0.4.0/gaiah/utils.py` & `gaiah_toolkit-0.5.1/gaiah/utils.py`

 * *Files identical despite different names*

### Comparing `gaiah_toolkit-0.4.0/gaiah_toolkit.egg-info/PKG-INFO` & `gaiah_toolkit-0.5.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: gaiah_toolkit
-Version: 0.4.0
-Home-page: https://github.com/your_username/gaiah
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Version Control
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: gitpython
-Requires-Dist: python-dotenv
-Requires-Dist: PyGithub
-Requires-Dist: termcolor
-Requires-Dist: art
-
 
 <p align="center">
 <img src="https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/Gaiah_icon1.png" width="100%">
 <br>
 <h1 align="center">Gaiah</h1>
 <h2 align="center">
   ～Python Git Automation with Innovative Heuristics～
@@ -48,121 +33,137 @@
 </p>
 
 >[!IMPORTANT]
 >このリポジトリは[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage)を活用しており、リリースノートやREADME、コミットメッセージの9割は[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ＋ [claude.ai](https://claude.ai/)で生成しています。
 
 ## 🌟 はじめに
 
-Gaiahは、直感的でAIにやさしいメソッドを使用してGit操作を簡素化する革新的なPythonライブラリです。Gitリポジトリを制御するための高レベルなインターフェースを提供し、AIシステムがバージョン管理とシームレスに連携することを容易にします。新機能としてMarkdownから直接コミットを生成する機能が追加され、文書化されたコミットメッセージの管理がさらに効率的に行えます。
+Gaiahは、初心者でも簡単に使えるPythonのライブラリです。Gitを使ってファイルの管理をするのを助けてくれます。新しいバージョンのGaiahでは、Markdownでコミットメッセージをかけるようになりました。
 
-## 🚀 主な特徴
+## 🚀 Gaiahの特徴
 
-- 🤖 **AIフレンドリー**: AI主導の開発プロセスの独自の要件に対応するメソッドとユーティリティを提供し、AIを念頭に置いて設計されています。
-- 🌐 **リモートリポジトリのサポート**: リモートリポジトリとのシームレスな連携を可能にし、GitHubやその他のGitホスティングプラットフォームにリポジトリを作成、クローン、プッシュできるようにします。 
-- 📂 **リポジトリ管理**: 新しいリポジトリの初期化、ファイルの追加、コミットの作成、ブランチの管理をシンプルなPythonコードを介して簡単に行うことができます。
-- 🔧 **カスタマイズ**: 柔軟性とカスタマイズオプションを提供し、特定のニーズと設定に合わせてGitワークフローを調整できます。
-- 📘 **Markdownからのコミット生成**: Markdown形式のドキュメントから直接コミットを生成する機能を追加し、文書化されたコミットメッセージの効率的な管理を可能にします。
+- 🤖 **AIにやさしい**: AIを使った開発に合わせて作られています。
+- 🌐 **リモートリポジトリ**: GitHubなどのサービスとつながります。
+- 📂 **リポジトリ管理**: 新しいリポジトリを作ったり、ファイルを追加したり、コミットしたり、ブランチを管理したりできます。
+- 🔧 **カスタマイズ**: 自分の好みに合わせてGitの使い方を変えられます。
+- 📘 **Markdownでコミット**: Markdownで書いたファイルからコミットメッセージを作れます。
 
-## 📦 インストール
+## 📦 インストールの仕方
 
-Gaiahの使用を開始するには、次の手順に従ってください:
+Gaiahを使うには、次のコマンドを実行してください:
 
-1. 新しいconda環境を作成します:
-   ```
-   conda create -n gaiah python=3.11
    ```
-2. conda環境をアクティベートします:
-   ```
-   conda activate gaiah
-   ```
-3. 必要な依存関係をインストールします:
-   ```
-   pip install gitpython python-dotenv PyGithub termcolor art
+   pip install gaiah-toolkit
    ```
 
-## 🎉 使用方法
+## 🎉 使い方
 
-### CLI
+### コマンドライン
 
-GaiahのCLI機能により、コマンドラインから直接Git操作を行うことができます。例えば、以下のコマンドを使用してリポジトリにコミットを追加することができます:
+Gaiahはコマンドラインから使えます。例えば、こんなふうにコミットできます:
 ```bash
 gaiah
 ```
 
-### 応用的な使い方
-
-特定のプロジェクトディレクトリでGaiahを使用する場合、以下のようにリポジトリの場所やコミットメッセージのファイルパスを指定できます:
-
+もっと細かく指定することもできます:
 ```bash
 gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
 ```
 
-### リポジトリの初期化
+### 新しいリポジトリを作る
 
 ```bash
 gaiah --create_repo --repo_name Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
 ```
 
-## 処理フロー
+### .Gaiah.mdのコミットメッセージを一括送信
+
+Gaiahでは、.Gaiah.mdファイルにMarkdown形式でコミットメッセージをまとめて書いておくことができます。そして、次のコマンドを実行すると、.Gaiah.mdに書かれたコミットメッセージが一括でリポジトリに送信されます:
+
+```bash
+gaiah --process_commits
+```
+
+このコマンドを使えば、たくさんのコミットメッセージを一度に処理できるので、とても便利です。
+
+## Gaiahの中身
+
+Gaiahの処理の流れは、次の図のようになっています:
 
 ```mermaid
 
 graph TD
-   A[ユーザーがCLIを実行] --> B{コマンドライン引数を解析}
-   B --> C{Gaiahオブジェクトを作成}
-   C --> D{--create_repoオプションが指定されている?}
-   D -->|Yes| E[新しいリポジトリをGitHub上に作成]
-   E --> E1[.envファイルから環境変数を読み込む]
-   E1 --> E2[環境変数からアクセストークンを取得]
-   E2 --> E3[GitHubオブジェクトを作成]
-   E3 --> E4[リポジトリ名とパラメータを指定]
-   E4 --> E5[GitHub上に新しいリポジトリを作成]
-   E5 --> E6[リポジトリ作成完了のメッセージを表示]
-   E6 --> Q[処理完了]
-   D -->|No| F{--process_commitsオプションが指定されている?}
-   F -->|Yes| G[コミットメッセージファイルからコミットを処理]
-   G --> H[すべてのファイルをアンステージ]
-   H --> I{コミットセクションごとに処理}
+   A[ユーザーがコマンドを実行] --> B{コマンドを読み取る}
+   B --> C{Gaiahを準備}
+   C --> D{新しいリポジトリを作る?}
+   D -->|Yes| E[GitHubに新しいリポジトリを作る]
+   E --> E1[.envファイルから情報を読む]
+   E1 --> E2[トークンを取得]
+   E2 --> E3[GitHubとつなぐ]
+   E3 --> E4[リポジトリ名などを設定]
+   E4 --> E5[リポジトリを作る]
+   E5 --> E6[完了メッセージを出す]
+   E6 --> Q[おしまい]
+   D -->|No| F{コミットする?}
+   F -->|Yes| G[Markdownファイルからコミットを作る]
+   G --> H[全部のファイルをアンステージ]
+   H --> I{コミットを1つずつ処理}
    I --> J{ファイル名とコミットメッセージを取得}
    J --> K{ファイルを処理}
    K --> L{ファイルをステージ}
    L --> M{変更をコミット}
-   M --> N{次のコミットセクションがある?}
+   M --> N{次のコミットある?}
    N -->|Yes| I
-   N -->|No| O[リモートリポジトリにプッシュ]
-   O --> P[処理完了]
-   F -->|No| Q[処理完了]
+   N -->|No| O[リモートにプッシュ]
+   O --> P[おしまい]
+   F -->|No| Q[おしまい]
 
 ```
 
-## 開発用
+## 開発者向け
 
+1. 新しいconda環境を作ります:
+   ```
+   conda create -n gaiah python=3.11
+   ```
+2. conda環境に入ります:
+   ```
+   conda activate gaiah
+   ```
+3. 必要なものをインストールします:
+   ```
+   pip install gitpython python-dotenv PyGithub termcolor art
+   ```
+
+便利なコマンド:
 ```bash
-gaiah --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits
+script\activate-gaiah.bat
 ```
 
+```bash
+gaiah --repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits
+gaiah --create_repo --repo_name AIRA --description "AIRA: AI-Integrated Repository for Accelerated Development" --init_repo --repo_dir C:\Prj\AIRA --process_commits --commit_msg_path .Gaiah.md
+```
 
+## 🤝 みんなでGaiahを良くしよう
 
-
-## 🤝 貢献
-
-Gaiahをさらに良くするために、コミュニティからの貢献を歓迎します。アイデア、提案、バグ報告がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/Gaiah)で issue を開くか、プルリクエストを送信してください。
+Gaiahをもっと良くするアイデアや、バグを見つけたら、[GitHubのページ](https://github.com/Sunwood-ai-labs/Gaiah)で教えてください。
 
 ## 📄 ライセンス
 
-Gaiahは、[MITライセンス](https://opensource.org/licenses/MIT)の下でリリースされており、ライブラリの自由かつオープンソースでの使用、変更、配布が可能です。
+GaiahはMITライセンスで公開されているので、自由に使ったり、変えたり、配ったりできます。
 
-## 🙏 謝辞
+## 🙏 感謝
 
-Gaiahは、以下のライブラリの優れた機能に基づいて構築されています:
+Gaiahは、次のようなすばらしいライブラリのおかげで作ることができました:
 
 - [GitPython](https://github.com/gitpython-developers/GitPython)
 - [python-dotenv](https://github.com/theskumar/python-dotenv)
 - [PyGithub](https://github.com/PyGithub/PyGithub)
 - [termcolor](https://pypi.org/project/termcolor/)
 - [art](https://pypi.org/project/art/)
 
-これらのプロジェクトの開発者とコントリビューターの皆様が、オープンソースコミュニティに貴重な貢献をしてくださったことに感謝します。
+これらを作ってくれた人たちに感謝します。
 
 ---
 
-Gaiahを使用してGitワークフローの自動化を開始し、AI主導の開発の力を解き放ちましょう! 🚀✨
+さあ、Gaiahを使ってGitを楽しく使いこなしましょう! 🚀✨
```

#### html2text {}

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1 Name: gaiah_toolkit Version: 0.4.0 Home-page: https://
-github.com/your_username/gaiah Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers Classifier: Topic :: Software
-Development :: Version Control Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: gitpython Requires-Dist: python-dotenv Requires-
-Dist: PyGithub Requires-Dist: termcolor Requires-Dist: art
        [https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/
                                Gaiah_icon1.png]
                               ************ GGaaiiaahh ************
  ********** ?ï?½?PPyytthhoonn GGiitt AAuuttoommaattiioonn wwiitthh IInnnnoovvaattiivvee HHeeuurriissttiiccss?ï?½? [[!![[HHuuggggiinngg FFaaccee
   SSppaacceess]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//bbaaddggee//%%FF00%%99FF%%AA44%%9977%%2200HHuuggggiinngg%%2200FFaaccee--SSppaacceess--
 bblluuee))]]((hhttttppss::////hhuuggggiinnggffaaccee..ccoo//ssppaacceess//MMaakkiiAAii//GGaaiiaahh)) [[!![[GGaaiiaahh -- SSuunnwwoooodd--aaii--llaabbss]]
        ((hhttttppss::////iimmgg..sshhiieellddss..iioo//ssttaattiicc//vv11??llaabbeell==GGaaiiaahh&&mmeessssaaggee==SSuunnwwoooodd--aaii--
@@ -25,71 +19,69 @@
    llaabbss//GGaaiiaahh??ccoolloorr==oorraannggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//GGaaiiaahh)) **********
    _[[_?ð_?_?_?_ _WW_ee_bb_ss_ii_tt_ee_]] â¢ _[[_?ð_?_?_?±_ _GG_ii_tt_HH_uu_bb_]] _[[_?ð_?_?_?¦_ _TT_ww_ii_tt_tt_ee_rr_]] â¢ _[_ð____ _O_f_f_i_c_i_a_l_ _B_l_o_g_]
 >[!IMPORTANT] >ãã®ãªãã¸ããªã¯[SourceSage](https://github.com/Sunwood-
 ai-labs/
 SourceSage)ãæ´»ç¨ãã¦ããããªãªã¼ã¹ãã¼ããREADMEãã³ãããã¡ãã»ã¼ã¸ã®9å²ã¯
 [SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ï¼ [claude.ai]
 (https://claude.ai/)ã§çæãã¦ãã¾ãã ## ð ã¯ããã«
-Gaiahã¯ãç´æçã§AIã«ããããã¡ã½ãããä½¿ç¨ãã¦Gitæä½ãç°¡ç´ åããé©æ°çãªPythonã©ã¤ãã©ãªã§ããGitãªãã¸ããªãå¶å¾¡ããããã®é«ã¬ãã«ãªã¤ã³ã¿ã¼ãã§ã¼ã¹ãæä¾ããAIã·ã¹ãã ããã¼ã¸ã§ã³ç®¡çã¨ã·ã¼ã ã¬ã¹ã«é£æºãããã¨ãå®¹æã«ãã¾ããæ°æ©è½ã¨ãã¦Markdownããç´æ¥ã³ããããçæããæ©è½ãè¿½å ãããææ¸åãããã³ãããã¡ãã»ã¼ã¸ã®ç®¡çãããã«å¹ççã«è¡ãã¾ãã
-## ð ä¸»ãªç¹å¾´ - ð¤ **AIãã¬ã³ããªã¼**:
-AIä¸»å°ã®éçºãã­ã»ã¹ã®ç¬èªã®è¦ä»¶ã«å¯¾å¿ããã¡ã½ããã¨ã¦ã¼ãã£ãªãã£ãæä¾ããAIãå¿µé ­ã«ç½®ãã¦è¨­è¨ããã¦ãã¾ãã
-- ð **ãªã¢ã¼ããªãã¸ããªã®ãµãã¼ã**:
-ãªã¢ã¼ããªãã¸ããªã¨ã®ã·ã¼ã ã¬ã¹ãªé£æºãå¯è½ã«ããGitHubããã®ä»ã®Gitãã¹ãã£ã³ã°ãã©ãããã©ã¼ã ã«ãªãã¸ããªãä½æãã¯ã­ã¼ã³ãããã·ã¥ã§ããããã«ãã¾ãã
-- ð **ãªãã¸ããªç®¡ç**:
-æ°ãããªãã¸ããªã®åæåããã¡ã¤ã«ã®è¿½å ãã³ãããã®ä½æããã©ã³ãã®ç®¡çãã·ã³ãã«ãªPythonã³ã¼ããä»ãã¦ç°¡åã«è¡ããã¨ãã§ãã¾ãã
+Gaiahã¯ãåå¿èã§ãç°¡åã«ä½¿ããPythonã®ã©ã¤ãã©ãªã§ããGitãä½¿ã£ã¦ãã¡ã¤ã«ã®ç®¡çãããã®ãå©ãã¦ããã¾ããæ°ãããã¼ã¸ã§ã³ã®Gaiahã§ã¯ãMarkdownã§ã³ãããã¡ãã»ã¼ã¸ããããããã«ãªãã¾ããã
+## ð Gaiahã®ç¹å¾´ - ð¤ **AIã«ãããã**:
+AIãä½¿ã£ãéçºã«åããã¦ä½ããã¦ãã¾ãã - ð
+**ãªã¢ã¼ããªãã¸ããª**:
+GitHubãªã©ã®ãµã¼ãã¹ã¨ã¤ãªããã¾ãã - ð
+**ãªãã¸ããªç®¡ç**:
+æ°ãããªãã¸ããªãä½ã£ããããã¡ã¤ã«ãè¿½å ããããã³ããããããããã©ã³ããç®¡çãããã§ãã¾ãã
 - ð§ **ã«ã¹ã¿ãã¤ãº**:
-æè»æ§ã¨ã«ã¹ã¿ãã¤ãºãªãã·ã§ã³ãæä¾ããç¹å®ã®ãã¼ãºã¨è¨­å®ã«åããã¦Gitã¯ã¼ã¯ãã­ã¼ãèª¿æ´ã§ãã¾ãã
-- ð **Markdownããã®ã³ãããçæ**:
-Markdownå½¢å¼ã®ãã­ã¥ã¡ã³ãããç´æ¥ã³ããããçæããæ©è½ãè¿½å ããææ¸åãããã³ãããã¡ãã»ã¼ã¸ã®å¹ççãªç®¡çãå¯è½ã«ãã¾ãã
-## ð¦ ã¤ã³ã¹ãã¼ã«
-Gaiahã®ä½¿ç¨ãéå§ããã«ã¯ãæ¬¡ã®æé ã«å¾ã£ã¦ãã ãã: 1.
-æ°ããcondaç°å¢ãä½æãã¾ã: ``` conda create -n gaiah python=3.11
-``` 2. condaç°å¢ãã¢ã¯ãã£ãã¼ããã¾ã: ``` conda activate gaiah
-``` 3. å¿è¦ãªä¾å­é¢ä¿ãã¤ã³ã¹ãã¼ã«ãã¾ã: ``` pip install
-gitpython python-dotenv PyGithub termcolor art ``` ## ð ä½¿ç¨æ¹æ³ ### CLI
-Gaiahã®CLIæ©è½ã«ãããã³ãã³ãã©ã¤ã³ããç´æ¥Gitæä½ãè¡ããã¨ãã§ãã¾ããä¾ãã°ãä»¥ä¸ã®ã³ãã³ããä½¿ç¨ãã¦ãªãã¸ããªã«ã³ããããè¿½å ãããã¨ãã§ãã¾ã:
-```bash gaiah ``` ### å¿ç¨çãªä½¿ãæ¹
-ç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§Gaiahãä½¿ç¨ããå ´åãä»¥ä¸ã®ããã«ãªãã¸ããªã®å ´æãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãæå®ã§ãã¾ã:
-```bash gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-``` ### ãªãã¸ããªã®åæå ```bash gaiah --create_repo --repo_name
+èªåã®å¥½ã¿ã«åããã¦Gitã®ä½¿ãæ¹ãå¤ãããã¾ãã - ð
+**Markdownã§ã³ããã**:
+Markdownã§æ¸ãããã¡ã¤ã«ããã³ãããã¡ãã»ã¼ã¸ãä½ãã¾ãã
+## ð¦ ã¤ã³ã¹ãã¼ã«ã®ä»æ¹
+Gaiahãä½¿ãã«ã¯ãæ¬¡ã®ã³ãã³ããå®è¡ãã¦ãã ãã: ``` pip
+install gaiah-toolkit ``` ## ð ä½¿ãæ¹ ### ã³ãã³ãã©ã¤ã³
+Gaiahã¯ã³ãã³ãã©ã¤ã³ããä½¿ãã¾ããä¾ãã°ããããªãµãã«ã³ãããã§ãã¾ã:
+```bash gaiah ``` ãã£ã¨ç´°ããæå®ãããã¨ãã§ãã¾ã: ```bash
+gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md ``` ###
+æ°ãããªãã¸ããªãä½ã ```bash gaiah --create_repo --repo_name
 Gaiah_Sample05 --description "Gaiah_Sample05 repo" --init_repo --repo_dir C:
 \Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits --commit_msg_path .Gaiah.md
-``` ## å¦çãã­ã¼ ```mermaid graph TD A[ã¦ã¼ã¶ã¼ãCLIãå®è¡] --> B
-{ã³ãã³ãã©ã¤ã³å¼æ°ãè§£æ} B --> C
-{Gaiahãªãã¸ã§ã¯ããä½æ} C --> D{--
-create_repoãªãã·ã§ã³ãæå®ããã¦ãã?} D -->|Yes| E
-[æ°ãããªãã¸ããªãGitHubä¸ã«ä½æ] E --> E1
-[.envãã¡ã¤ã«ããç°å¢å¤æ°ãèª­ã¿è¾¼ã] E1 --> E2
-[ç°å¢å¤æ°ããã¢ã¯ã»ã¹ãã¼ã¯ã³ãåå¾] E2 --> E3
-[GitHubãªãã¸ã§ã¯ããä½æ] E3 --> E4
-[ãªãã¸ããªåã¨ãã©ã¡ã¼ã¿ãæå®] E4 --> E5
-[GitHubä¸ã«æ°ãããªãã¸ããªãä½æ] E5 --> E6
-[ãªãã¸ããªä½æå®äºã®ã¡ãã»ã¼ã¸ãè¡¨ç¤º] E6 --> Q[å¦çå®äº]
-D -->|No| F{--process_commitsãªãã·ã§ã³ãæå®ããã¦ãã?} F --
->|Yes| G[ã³ãããã¡ãã»ã¼ã¸ãã¡ã¤ã«ããã³ããããå¦ç] G
---> H[ãã¹ã¦ã®ãã¡ã¤ã«ãã¢ã³ã¹ãã¼ã¸] H --> I
-{ã³ãããã»ã¯ã·ã§ã³ãã¨ã«å¦ç} I --> J
+``` ### .Gaiah.mdã®ã³ãããã¡ãã»ã¼ã¸ãä¸æ¬éä¿¡
+Gaiahã§ã¯ã.Gaiah.mdãã¡ã¤ã«ã«Markdownå½¢å¼ã§ã³ãããã¡ãã»ã¼ã¸ãã¾ã¨ãã¦æ¸ãã¦ãããã¨ãã§ãã¾ããããã¦ãæ¬¡ã®ã³ãã³ããå®è¡ããã¨ã.Gaiah.mdã«æ¸ãããã³ãããã¡ãã»ã¼ã¸ãä¸æ¬ã§ãªãã¸ããªã«éä¿¡ããã¾ã:
+```bash gaiah --process_commits ```
+ãã®ã³ãã³ããä½¿ãã°ãããããã®ã³ãããã¡ãã»ã¼ã¸ãä¸åº¦ã«å¦çã§ããã®ã§ãã¨ã¦ãä¾¿å©ã§ãã
+## Gaiahã®ä¸­èº«
+Gaiahã®å¦çã®æµãã¯ãæ¬¡ã®å³ã®ããã«ãªã£ã¦ãã¾ã:
+```mermaid graph TD A[ã¦ã¼ã¶ã¼ãã³ãã³ããå®è¡] --> B
+{ã³ãã³ããèª­ã¿åã} B --> C{Gaiahãæºå} C --> D
+{æ°ãããªãã¸ããªãä½ã?} D -->|Yes| E
+[GitHubã«æ°ãããªãã¸ããªãä½ã] E --> E1
+[.envãã¡ã¤ã«ããæå ±ãèª­ã] E1 --> E2[ãã¼ã¯ã³ãåå¾] E2 --
+> E3[GitHubã¨ã¤ãªã] E3 --> E4[ãªãã¸ããªåãªã©ãè¨­å®] E4 --> E5
+[ãªãã¸ããªãä½ã] E5 --> E6[å®äºã¡ãã»ã¼ã¸ãåºã] E6 --> Q
+[ããã¾ã] D -->|No| F{ã³ããããã?} F -->|Yes| G
+[Markdownãã¡ã¤ã«ããã³ããããä½ã] G --> H
+[å¨é¨ã®ãã¡ã¤ã«ãã¢ã³ã¹ãã¼ã¸] H --> I
+{ã³ãããã1ã¤ãã¤å¦ç} I --> J
 {ãã¡ã¤ã«åã¨ã³ãããã¡ãã»ã¼ã¸ãåå¾} J --> K
 {ãã¡ã¤ã«ãå¦ç} K --> L{ãã¡ã¤ã«ãã¹ãã¼ã¸} L --> M
-{å¤æ´ãã³ããã} M --> N{æ¬¡ã®ã³ãããã»ã¯ã·ã§ã³ããã?} N
--->|Yes| I N -->|No| O[ãªã¢ã¼ããªãã¸ããªã«ããã·ã¥] O --> P
-[å¦çå®äº] F -->|No| Q[å¦çå®äº] ``` ## éçºç¨ ```bash gaiah --
-repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits ``` ## ð¤
-è²¢ç®
-Gaiahãããã«è¯ãããããã«ãã³ãã¥ããã£ããã®è²¢ç®ãæ­è¿ãã¾ããã¢ã¤ãã¢ãææ¡ããã°å ±åãããå ´åã¯ã
-[GitHubãªãã¸ããª](https://github.com/Sunwood-ai-labs/Gaiah)ã§ issue
-ãéããããã«ãªã¯ã¨ã¹ããéä¿¡ãã¦ãã ããã ## ð
-ã©ã¤ã»ã³ã¹ Gaiahã¯ã[MITã©ã¤ã»ã³ã¹](https://opensource.org/
-licenses/
-MIT)ã®ä¸ã§ãªãªã¼ã¹ããã¦ãããã©ã¤ãã©ãªã®èªç±ãã¤ãªã¼ãã³ã½ã¼ã¹ã§ã®ä½¿ç¨ãå¤æ´ãéå¸ãå¯è½ã§ãã
-## ð è¬è¾
-Gaiahã¯ãä»¥ä¸ã®ã©ã¤ãã©ãªã®åªããæ©è½ã«åºã¥ãã¦æ§ç¯ããã¦ãã¾ã:
+{å¤æ´ãã³ããã} M --> N{æ¬¡ã®ã³ããããã?} N -->|Yes| I N --
+>|No| O[ãªã¢ã¼ãã«ããã·ã¥] O --> P[ããã¾ã] F -->|No| Q
+[ããã¾ã] ``` ## éçºèåã 1. æ°ããcondaç°å¢ãä½ãã¾ã:
+``` conda create -n gaiah python=3.11 ``` 2. condaç°å¢ã«å¥ãã¾ã: ```
+conda activate gaiah ``` 3. å¿è¦ãªãã®ãã¤ã³ã¹ãã¼ã«ãã¾ã: ```
+pip install gitpython python-dotenv PyGithub termcolor art ```
+ä¾¿å©ãªã³ãã³ã: ```bash script\activate-gaiah.bat ``` ```bash gaiah --
+repo_dir C:\Prj\Gaiah_Sample\Gaiah_Sample05 --process_commits gaiah --
+create_repo --repo_name AIRA --description "AIRA: AI-Integrated Repository for
+Accelerated Development" --init_repo --repo_dir C:\Prj\AIRA --process_commits -
+-commit_msg_path .Gaiah.md ``` ## ð¤ ã¿ããªã§Gaiahãè¯ãããã
+Gaiahããã£ã¨è¯ãããã¢ã¤ãã¢ãããã°ãè¦ã¤ãããã
+[GitHubã®ãã¼ã¸](https://github.com/Sunwood-ai-labs/
+Gaiah)ã§æãã¦ãã ããã ## ð ã©ã¤ã»ã³ã¹
+Gaiahã¯MITã©ã¤ã»ã³ã¹ã§å¬éããã¦ããã®ã§ãèªç±ã«ä½¿ã£ãããå¤ããããéã£ããã§ãã¾ãã
+## ð æè¬
+Gaiahã¯ãæ¬¡ã®ãããªãã°ãããã©ã¤ãã©ãªã®ãããã§ä½ããã¨ãã§ãã¾ãã:
 - [GitPython](https://github.com/gitpython-developers/GitPython) - [python-
 dotenv](https://github.com/theskumar/python-dotenv) - [PyGithub](https://
 github.com/PyGithub/PyGithub) - [termcolor](https://pypi.org/project/termcolor/
 ) - [art](https://pypi.org/project/art/
-)
-ãããã®ãã­ã¸ã§ã¯ãã®éçºèã¨ã³ã³ããªãã¥ã¼ã¿ã¼ã®çæ§ãããªã¼ãã³ã½ã¼ã¹ã³ãã¥ããã£ã«è²´éãªè²¢ç®ããã¦ãã ãã£ããã¨ã«æè¬ãã¾ãã
---
--
-Gaiahãä½¿ç¨ãã¦Gitã¯ã¼ã¯ãã­ã¼ã®èªååãéå§ããAIä¸»å°ã®éçºã®åãè§£ãæ¾ã¡ã¾ããã!
-ðâ¨
+) ããããä½ã£ã¦ãããäººãã¡ã«æè¬ãã¾ãã --
+- ãããGaiahãä½¿ã£ã¦Gitãæ¥½ããä½¿ãããªãã¾ããã! ðâ¨
```

### Comparing `gaiah_toolkit-0.4.0/setup.py` & `gaiah_toolkit-0.5.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Version Control",
     ],
     package_data={
         'gaiah': ['README.md',
-                  'requirements.txt'],
+                  'requirements.txt',
+                  'template/*'], 
     },
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/your_username/gaiah",
     install_requires=[
             'gitpython',
             'python-dotenv',
```

### Comparing `gaiah_toolkit-0.4.0/tests/test_cli.py` & `gaiah_toolkit-0.5.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gaiah_toolkit-0.4.0/tests/test_main.py` & `gaiah_toolkit-0.5.1/tests/test_main.py`

 * *Files identical despite different names*

