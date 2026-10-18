# webp-share

カメラ・アルバムの画像を縮小・圧縮して、共有シートから Discord などへ添付するツール。
HTML 1枚だけの静的ページで、画像処理はすべてブラウザ内で完結します（サーバー送信なし）。

https://ayu0616.github.io/webp-share/

- 最大10枚（Discord の添付上限に準拠）、↑↓で並べ替え
- 画質・最大辺を指定して再変換、⤓で個別保存
- 出力形式: WebP（Chrome/Edge/Firefox）／JPEG（Safari は canvas の WebP 書き出し非対応のため自動で切替）
- 共有は Web Share API（`navigator.share({files})`）
