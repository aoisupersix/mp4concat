# mp4concat

Files shot with GoPro are split into 4.01GB pieces.

You can combine multiple files that have been split into one file without re-encoding (no video degradation).

## Requirements

- [ffmpeg](https://ffmpeg.org/)

## Usage

Download and run the binary for the OS you are using from [Release](https://github.com/aoisupersix/mp4concat/releases).

Display the contents of your GoPro's SD card in order of oldest to newest, and select all the video files you want to merge into one video. Only MP4 files will be used.

Once you have pasted the list of files, activate the terminal (click on it) and hit the enter key. If you expand the window a little, you can see the status without scrolling.

The combined file is output to the same directory as the input file.

## What's happening

Create a file with a list of files passed to a temporary folder (depending on the OS) and combine them with [ffmpeg's concat](https://trac.ffmpeg.org/wiki/Concatenate).

### Notice

GPS information of stream 03 will not be copied.
If you need GPS metadata, please use official application.

## Platforms that are likely to work

I tried to run it on Windows 11.

Binaries for Linux and MacOSX are also generated, but have not been tested.

---

GoProで撮影したファイルは4.01GBごとに分割されてしまいます。

分割されてしまった複数ファイルを、再エンコードを行わずに1つのファイルに結合します（動画の劣化がありません）。

## 要件

- [ffmpeg](https://ffmpeg.org/)

## 使い方

[リリース](https://github.com/aoisupersix/mp4concat/releases)から利用しているOS用のバイナリをダウンロードして実行します。

GoProの撮影済みのSDカードの中身を日付の古い順に表示して、1つの動画に結合したい動画ファイルを全て選択します。このとき、THMファイルも一緒に選択してしまって構いません。MP4ファイルだけを利用します。

ファイルの一覧を貼り付けられたら、terminalをアクティブにして（クリックして）、エンターキーを推します。ウィンドウを少し広げるとスクロールせずに状況が表示されます。

結合後のファイルは入力されたファイルと同じディレクトリに出力します。

## 何が起きているのか

一時フォルダ(OSによって異なります)に渡されたファイルの一覧が記載されたファイルを作成し、[ffmpegのconcat](https://trac.ffmpeg.org/wiki/Concatenate)で結合します。

### 注意

03番のストリームに入っているGPSメタデータはコピーされません。
GPS情報が必要な場合は、純正のアプリを使用してください。

## 動作すると思われるプラットフォーム

Windows 11で動作確認してます。

Linux、MacOSX用のバイナリも生成していますが、動作は未確認です。
