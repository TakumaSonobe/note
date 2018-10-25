# Githubの使い方

## 初め方

### Githubで新しいリポジトリを作成
1. GitHubのマイページにて、`Repositories`のタブより`New`を選択
1. 任意のRepository nameを決める
1. PublicかPrivateの選択をする（Privateは有償）
1. Initialize this repository with a README は後から作成するためNoneのままで大丈夫

以上にてGitHub側の設定は完了

### PC側の設定
```
cd [GitHubで管理したいローカルのリポジトリ]
mkdir [GitHubで作成したRepository name]
git init
```

```Bash:example 
cd /work/rocal/repository
git init
```

以上にてPC側の設定は完了

### 初めてのPush

#### 1. Gitのリポジトリが管理されている階層にて、何かしらのファイルを作成する。
```
touch [ファイル名]
```

```Bash:example
touch README.md
```

#### 2. add,commitする

```
git add .
git commit -m "[コミットのコメント]"
```

```Bash:example 
git add .
git commit -m "FirstCommit"
```

#### 3. GitHubのリモートリポジトリ情報を追加する
```
git remote add origin [リモートリポジトリ情報]
```

```Bash:example 
git remote add origin https://github.com/xxxx/sample-repository.git
```

2回目以降この操作はいらない

#### 4. ローカルリポジトリをリモートリポジトリへ反映させる
```
git push origin master
```

2回目以降は
```
git push
```
のみで大丈夫



以下、GitHubでの例を示す

 …or create a new repository on the command line

```Bash:example
echo "# note" >> README.md
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:TakumaSonobe/note.git
git push -u origin master
```
