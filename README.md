# Flutter for web 環境構築

- Flutterのweb版での環境構築です。androidも頑張ればできます。
- 途中remote-containerを開かないといけないので動画を参考にしてください。

- 動画
   - [参考動画](https://gitlab.com/welcome-to-sodai/flutter-web/-/raw/master/video.mov?inline=false)

## FlutterDock

1. リポジトリをクローン

   ```
   git clone https://github.com/takassh23/flutter-for-web.git flutter_app/flutterdock
   ```

2. flutterdock階層で

   ```
   docker-compose build workspace
   ```

   いつも通り最初は長いです。wifi環境が良いときにやりましょう。

4. コンテナを構築、起動

   ```
   docker-compose up -d workspace
   ```

5. vscodeのremote-containerでworkspaceを開く

6. workspaceのbashに入りFlutterアプリを作成

   ```
   flutter create .
   ```

7. サーバーを起動

   ```
   flutter run
   ```

    そのうち右下にopenが出るのでクリックするとブラウザが開きます

## 使い方

- 始めるとき flutterdockの階層で
   ```bash
   docker-compose up -d workspace
   ```
- 終わるとき
   ```bash
   docker-compose down
   ```
