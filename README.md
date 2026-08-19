# aika-reels

Instagramリール投稿用の動画ホスティング専用リポジトリ。

Instagram Graph APIは動画を**公開URLからしか取り込めない**(2026-08-19に`upload_type=resumable`を検証したが`The parameter video_url is required`で使用不可)。
`x-auto-poster`の`reel_finish.py`で仕上げた動画をここへpushし、raw URLをGraph APIに渡すためだけに存在する。

- 置くもの: 投稿予定・投稿済みのInstagramリール動画(`videos/`)
- 置かないもの: NSFW/Fanvue向けコンテンツ、認証情報、生成前の素材

判断軸・手順の正本は非公開の `ai-beauty-sns` ドキュメント側にある。
