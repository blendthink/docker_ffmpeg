# FFmpeg
　 FFmpeg を Docker コンテナ内で使用して、動画のアスペクト比・サイズ・形式などの編集をできるようにしました。

## 使い方

```docker
docker-compose up -d

docker-compose exec ffmpeg /bin/bash

# コンテナ内で実行する
ffmpeg -version
```

## よく使うコマンド

コンテナ内で実行する
```docker
ffmpeg -i ~.mov -r 24 ~.gif
ffmpeg -i ~.mov ~.mp4

ffmpeg -i movie.mp4 -s 1920x1200 movie_out.mp4

ffmpeg -i movie.mp4 -vf scale=-1:1200 movie_out.mp4
```

## その他
- [FFmpeg Static Builds](https://www.johnvansickle.com/ffmpeg/)
