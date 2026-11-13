# NovelScript Engine v1.4 Desktop（Windowsネイティブ版）

ブラウザやWebViewを使わず、Windows標準のデスクトップウィンドウとして動作するGUIシナリオエディタ／テストプレイヤーです。

## 利用者のPCにPythonは不要

完成した NovelScriptEngine.exe はPythonランタイムとTk/Tclを同梱する単体実行ファイルです。利用者はPythonをインストールする必要がありません。通常利用時のインターネット接続も不要です。

## v1.4：右クリックメニュー／セーブ・ロード／バックログ

ゲーム画面を右クリックするとゲーム内メニューが開きます。

- セーブ・ロード：10個のセーブスロットを一覧表示し、保存・読み込み・削除が可能
- 保存内容：シナリオ位置、変数、背景・立ち絵、BGM状態、表示中の文章・タイプライター位置、選択肢待機状態、エンディングフラグ、バックログ
- シナリオごとにセーブを分離し、Windowsのユーザーデータ領域に保存。EXE更新後も維持
- バックログ：過去の台詞と選択した選択肢を時系列でスクロール閲覧
- 選択肢待機中・wait命令中も右クリックメニューは開ける

## 既存機能

- 画面内の選択肢カード表示、クリック／数字キー1〜9による選択
- ゲーム画面クリックで文字送り。タイプライター中は1回目で全文表示、2回目で次へ
- 文字表示設定：フォント、サイズ、色、太さ、揃え、会話ウィンドウ／全画面／字幕、配置、透過、速度
- .nse / .txt の編集・保存、.nproj の読み込み変換、シーン／ラベル一覧、構文チェック
- 背景、立ち絵、WAV BGM／効果音、分岐、変数、エンディング

## Windows EXEの取得

GitHubの **Actions** タブ → **Build Windows EXE** → **Run workflow** を実行します。完了した実行のArtifactsから **NovelScriptEngine-Windows-x64** をダウンロードし、ZIPを展開して NovelScriptEngine.exe をダブルクリックします。ソースZIPの更新でも自動ビルドされます。

ビルド時のみGitHubのWindows runner上でPython 3.12とPyInstallerを使用します。利用者のWindows PCにPythonは不要です。

## 保存先

- 表示設定：%APPDATA%\NovelScriptEngine\settings.json
- セーブ：%APPDATA%\NovelScriptEngine\saves\<シナリオ識別子>\slot_01.json ～ slot_10.json

保存ファイルはEXEの外に置かれ、更新後も残ります。素材の権利情報は ASSET_CREDITS.md を参照してください。
