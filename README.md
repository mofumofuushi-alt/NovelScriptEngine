# NovelScript Engine v1.1 Desktop

Windows向けのネイティブGUIシナリオエディタ／テストプレイヤーです。完成版 NovelScriptEngine.exe はPythonランタイムとTk/Tclを同梱するため、利用者のWindows PCにPythonをインストールする必要はありません。通常利用はオフラインで動作します。

## 文字表示のカスタマイズ

メイン画面の「文字表示設定」から、ゲーム画面の見せ方を調整できます。

- インストール済みフォント、文字サイズ（10〜48pt）、太字／標準
- 本文と話者名の文字色、左寄せ／中央揃え／右寄せ
- 会話ウィンドウ／全画面テキスト／字幕スタイル
- ウィンドウの表示位置、高さ、左右余白、背景色、枠線色、透過パターン
- タイプライター表示のON/OFFと1文字あたりの速度（10〜200ms）
- 設定画面のプレビュー、次回起動時にも残るユーザー別保存

設定はシナリオファイルから独立して保存され、既存のNovelScript命令や.nseの互換性は変更しません。

## Windows EXE

1. GitHubの **Actions** タブを開き、**Build Windows EXE** を選びます。
2. **Run workflow** を実行します（ソースZIPを更新してpushした場合も自動で起動します）。
3. 完了した実行のArtifactsから NovelScriptEngine-Windows-x64 をダウンロードします。
4. ZIPを展開し、NovelScriptEngine.exe をダブルクリックします。

利用者のWindows PCにPythonは不要です。ビルド時のみGitHubのWindows runner上でPython 3.12とPyInstallerを使います。

## その他の主な機能

- .nse / .txt シナリオの作成・編集・読み込み・保存
- .nproj の読み込みと .nse への変換
- シーン／ラベル一覧、ジャンプ、命令テンプレート、構文チェック
- ネイティブウィンドウのテストプレイヤー
- 背景・立ち絵・選択肢・分岐・変数・エンディング
- WAV形式のBGM／効果音、5分間のサンプルとオリジナル素材

## 文字表示設定の保存先

Windows: %APPDATA%\NovelScriptEngine\settings.json

素材の権利情報はソースZIP内の ASSET_CREDITS.md を参照してください。
