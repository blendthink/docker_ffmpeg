# FFmpeg
　 Mac で撮った動画を Twitter にアップするために
 FFmpeg を Docker コンテナ内で使用できるようにしました(笑)

## 使い方

```docker
docker-compose -d up

docker-compose exec ffmpeg /bin/bash

# コンテナ内で実行する
ffmpeg -version
```

## よく使うコマンド

```docker
# コンテナ内で実行する
ffmpeg -i ~.mov ~.mp4
```

## その他
- [FFmpeg Static Builds](https://www.johnvansickle.com/ffmpeg/)
