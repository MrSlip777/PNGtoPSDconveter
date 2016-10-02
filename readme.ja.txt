Adobe Photoshop PSD ファイル読み込み
2008/01/19 sasao (http://tmp.junkbox.info/)

元ネタは、
Yet Another PSD Parser
http://www.codeproject.com/KB/graphics/PSDParser.aspx
です。

■ ビルド
- ビルドには、 Visual C# 2005 Express Edition 以上が必要です。
- 参照設定には、Dllsフォルダの .dll を利用してください。
  (Endogine.dll, Endogine.Editors.dll)

■ 修正内容

- レイヤ名に日本語などの多バイト文字が含まれていた場合に、
  正しく読み込めないバグを修正
- サムネイル画像が圧縮されていた場合に例外が出ることに対応
- サンプルプログラムで .psd ファイルを Drag&Drop したとき、
  long file name で読み込むよう修正

■ 既知の問題

- 1レイヤしかない場合に読み込みに失敗する場合がある
- PSDファイルの書き出しに対しては多バイト文字に未対応

以上。