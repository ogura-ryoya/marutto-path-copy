# marutto-path-copy

Windows Explorerでファイル・フォルダのパスを整形してコピーするAutoHotkey v2スクリプト

`Ctrl + Alt + C` で実行

## できること

### ファイルを1つ選択

```text id="f7v0x1"
C:\Users\ユーザー名\Documents\sample.txt
```

ファイルのフルパスをコピー

### フォルダを1つ選択

```text id="g2c9j4"
C:\Users\ユーザー名\Documents\SampleFolder\
```

フォルダのフルパスをコピー、末尾に `\` を付加

### 複数選択

```text id="n3p6k8"
C:\Users\ユーザー名\Documents\
Folder1\
Folder2\
file1.txt
file2.txt
file10.txt
```

* 現在のフォルダを先頭に追加
* フォルダを上に配置
* ファイルを下に配置
* 同じ種類は名前順でソート

## 導入

1. AutoHotkey v2を[インストール](https://www.autohotkey.com/download/ahk-v2.exe)
2. `marutto-path-copy.ahk` を[ダウンロード](https://github.com/ogura-ryoya/marutto-path-copy/releases/download/v1.0.0/marutto-path-copy.ahk)
3. `marutto-path-copy.ahk` ファイルを実行

### Windows起動時に自動実行

1. `Win + R` を押す
2. `shell:startup` と入力してEnter
3. `marutto-path-copy.ahk` のショートカットをスタートアップフォルダに追加

## 動作環境

* Windows
* AutoHotkey v2

## その他

`\\?\` / `\\?\UNC\` 形式のパスを通常形式に変換
