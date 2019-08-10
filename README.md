# Pytubeが急に下のようなエラーで使えなくなった方へ...

```
    signature = cipher.get_signature(js, stream['s'])
KeyError 's'
```

```
regex pattern ((?:v=|\/)([0-9A-Za-z_-]{11}).*) had zero matches
```

これらのエラーは`mixins.py`というファイルが悪さしています。
(下のほうのエラーは別の理由があるとも聞きます。僕は治りました。)

# 使用方法
`mixins.py`をこのGitの``mixins.py``で上書きするだけ。
インストール場所はOSによって違います。

【宣伝】pytubeの使いかたは[ここ](https://qiita.com/Cyber_Hacnosuke/items/d722eae05d6f7c41a9b7)まで。

# お断り
このエラーとその対応方法は2019年6月時点で有効でした。今は有効かどうか、~~またエラーが修正されているかどうか~~は確認していません。(最新版にすればエラーは治るようですが一部の方はまだ駄目なようです。)
*必ずバックアップを取ってください。*
おかしいと感じたらすぐにインストールしなおしてください。

```
$ pip uninstall pytube
$ pip install pytube
```

# その他
このファイルは僕の平穏な生活を妨げない限り、自由に使ってもらって構いません。