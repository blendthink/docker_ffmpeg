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

コンテナ内で実行する
```docker
ffmpeg -i ~.mov ~.mp4

ffmpeg -i movie.mp4 -s 1920x1200 movie_out.mp4

ffmpeg -i movie.mp4 -vf scale=-1:1200 movie_out.mp4
```

## その他
- [FFmpeg Static Builds](https://www.johnvansickle.com/ffmpeg/)
