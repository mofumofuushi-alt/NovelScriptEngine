# NovelScript Engine v1.0 Desktop

Windows向けのネイティブGUIシナリオエディタ／テストプレイヤーです。完成版 `NovelScriptEngine.exe` はPythonランタイムとTk/Tclを同梱するため、利用者のWindows PCにPythonをインストールする必要はありません。通常利用はオフラインで動作します。

## Windows EXEのビルド

1. GitHubの **Actions** タブを開きます。
2. **Build Windows EXE** を選択します。
3. **Run workflow** を実行します。
4. 完了後、Artifactsから `NovelScriptEngine-Windows-x64` をダウンロードします。
5. ZIPを展開し、`NovelScriptEngine.exe` をダブルクリックして起動します。

ビルド元のソース一式は `NovelScriptEngine-Source.zip.b64` に格納され、ワークフローが自動的に復元します。

## 主な機能

- `.nse` / `.txt` シナリオの作成・編集・読み込み・保存
- `.nproj` の読み込みと `.nse` への変換
- シーン／ラベル一覧、ジャンプ、命令テンプレート、構文チェック
- ネイティブウィンドウのテストプレイヤー
- 背景・立ち絵・選択肢・分岐・変数・エンディング
- WAV形式のBGM／効果音
- 5分間のサンプルプロジェクトとオリジナル素材

詳細はソース内の `WINDOWS_BUILD_GUIDE.md` と `ASSET_CREDITS.md` を参照してください。
