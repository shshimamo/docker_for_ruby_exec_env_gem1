# docker_for_ruby_exec_env_gem1
The first way to manage gems with Docker

イメージビルド時にbundle installを実行する方法。
まずDockerfileにCOPY命令を追加してGemfileとGemfile.lockがコピーされるようにする。
続けてRUN命令でbundle installが実行されるようにする。

新しくgemを追加したりアップグレードするたびにイメージの再ビルドが必要。
```
docker-compose build
```
