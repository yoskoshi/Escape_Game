# Escape_Game
## Githubでコード管理するために必要なGit操作マニュアル(コマンド編)
### githubからVSCode(ゲームの場合はUnity)にプロジェクトを持ってくる方法
1. このGithubリポジトリにアクセス権限をリクエストした覚えのない人はDiscordのmemoにGithubのユーザー名を書く。

2. 僕がcollaboratorに追加したらその旨をDiscordのmemoで言うので、それを確認したらGithubで登録したメールアドレスのメールボックスでGithubからのメールを確認して、招待を承認する。

3. 招待を承認したらGithubのプロジェクトに該当するリポジトリにアクセスし、緑色のCodeボタンを押す。

![git_clone1](https://github.com/yoskoshi/Escape_Game/assets/110778997/5971a822-4f90-4d63-bf50-17530a39fd4d)

4. 緑色のコードを押したら、HTTPSを選択してその下のURLの右のボタンを押してURLをコピーする。

![git_clone2](https://github.com/yoskoshi/Escape_Game/assets/110778997/3414ac00-8379-4a5c-8f39-a8c1a333c225)

5. githubのプロジェクトを入れたいディレクトリまで移動して、`git clone コピーしたURL`というコマンドをターミナル(Mac)またはコマンドプロンプト(windows)に打って下の画像のようなのが出るか確認する。

![git_clone3](https://github.com/yoskoshi/Escape_Game/assets/110778997/8b418c5f-a210-41c5-ac06-7c4d0e801ba7)

6. 移動しているディレクトリの中にプロジェクトが入っていると思うので、そのプロジェクトをVSCode(ゲームの場合はUnity)で開く。

### 変更内容をgithubに載せる方法
1. プロジェクトまでディレクトリを移動する。

2. `git checkout -b 作りたい機能のブランチ名`をターミナル(Mac)またはコマンドプロンプト(windows)に打って、VSCodeの左下に画像のように作りたい機能のブランチ名があるか確認。(Unityの場合はブランチ名が表示されないので、`git branch`で作りたい機能のブランチ名に他とは違う色が着いているか確認する)

![git_push1](https://github.com/yoskoshi/Escape_Game/assets/110778997/d2f1dd07-b0e2-457a-a12e-4470ef90eb0f)

3. 機能を実装する。

4. 実装できたら、`git status`で以下の画像のように自分が変更したファイルが赤くなっているか確認する。

![git_push2](https://github.com/yoskoshi/Escape_Game/assets/110778997/5f1612c9-dae1-4964-b6a7-56cbab8858f5)

5. 確認できたら、`git add 変更したファイル名`をターミナル(Mac)またはコマンドプロンプト(windows)に打つ。

6. もう一回`git status`をターミナル(Mac)またはコマンドプロンプト(windows)に打って、以下の画像のように変更したファイルが緑色になっているか確認する。

![git_push3](https://github.com/yoskoshi/Escape_Game/assets/110778997/7fe155a8-7880-4625-85c0-b1c7e37a252f)

7. 確認できたら、`git commit -m "<ここに作った機能の説明をする>"`をターミナル(Mac)またはコマンドプロンプト(windows)に打って、以下の画像のようになったか確認する。

![git_push4](https://github.com/yoskoshi/Escape_Game/assets/110778997/2a74e2ba-9d89-4a9a-b75e-0d9ae782d823)

8. 確認できたら、`git push origin 作ったブランチの名前`をターミナル(Mac)またはコマンドプロンプト(windows)に打って、以下の画像のようになったか確認する。

![git_push5](https://github.com/yoskoshi/Escape_Game/assets/110778997/bbe83d3f-69ef-4a5c-8fc5-6a3ac7a572d3)
