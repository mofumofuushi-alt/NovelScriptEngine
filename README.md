# NovelScript Engine v1.0 Desktop

Windows向けのネイティブGUIシナリオエディタ／テストプレイヤーです。完成版の NovelScriptEngine.exe はPythonランタイムとTk/Tclを同梱するため、利用者のWindows PCにPythonをインストールする必要はありません。通常利用はオフラインで動作します。

## 最初のWindows EXEを生成する方法

1. このリポジトリの Code タブを開き、Add file → Upload files を選択します。
2. 配布された NovelScriptEngine-Source-Optimized.zip を、そのままリポジトリ直下へアップロードします。ZIPは展開せず、そのままアップロードしてください。
3. Commit changes を押すと、Build Windows EXE ワークフローが自動で開始します。
4. Actions タブ → Build Windows EXE → 最新の実行を開きます。
5. ビルドが成功したら、Artifacts の NovelScriptEngine-Windows-x64 をダウンロードします。
6. ダウンロードしたZIPを展開し、NovelScriptEngine.exe をダブルクリックします。

また、ソースZIPをアップロードした後は Actions → Build Windows EXE → Run workflow から手動で再ビルドできます。

## ビルド内容

- Windows Server 2022 runnerでPython 3.12とPyInstallerを用意し、EXEを生成します。
- 利用者のWindows PCにはPythonをインストールしません。
- 完成EXEはPython/Tk/Tclランタイムとアプリ素材を内蔵し、通常利用時はオフラインで動作します。
- ビルド時に8件の回帰テストを実行します。
- EXEはワンファイル形式で出力されます。初回起動時は内部展開のため少し時間がかかる場合があります。

## 主な機能

- .nse / .txt シナリオの作成・編集・読み込み・保存
- .nproj の読み込みと .nse への変換
- シーン／ラベル一覧、ジャンプ、命令テンプレート、構文チェック
- ネイティブウィンドウのテストプレイヤー
- 背景・立ち絵・選択肢・分岐・変数・エンディング
- WAV形式のBGM／効果音
- 約5分のサンプルプロジェクトとオリジナル素材

素材の権利情報は、ビルド元ZIP内の ASSET_CREDITS.md を参照してください。
