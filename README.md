# alpine-jst

ホストのTimezoneがAsia/Tokyoな環境で、コンテナとホストの時刻がずれる(主にWindowsで発生)問題を解消するためのイメージです。
以下を実行することで強制的にコンテナの時刻をあわせます。

```sh
docker run --rm --privileged kanfushihara/alpine-jst hwclock -s --localtime
```
