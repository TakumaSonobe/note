# プライベートリポジトリからのgit clone

## 事象
何も考えずに`git clone`してみた

```
git clone https://github.com/username/private-repository.git
```

そしたらエラーが返ってきた

```
fatal: could not create leading directories of '@github.com:KatayamaLab/FCHEV-gym-model.git': Invalid argument
```

## 解決法

これでプライベートリポジトリからクローンできた


```
git clone https://username@github.com/username/private-repository.git
```

(注意)
`@github.com/username/private-repository.git`の部分は、clone with HTTPS を利用すること

![git]()

上手くいくとこのような画面が表示される

```
C:\Users\TAKUMA\Documents\GitHub>git clone https://TakumaSonobe@github.com/KatayamaLab/FCHEV-gym-model.git
Cloning into 'FCHEV-gym-model'...
Password for 'https://TakumaSonobe@github.com':
remote: Enumerating objects: 218, done.
remote: Counting objects: 100% (218/218), done.
remote: Compressing objects: 100% (153/153), done.
Rremote: Total 499 (delta 104), reused 160 (delta 55), pack-reused 281eceiving objects:  75% (375/499), 19.54 MiB | 154.00 KiB/s

Receiving objects: 100% (499/499), 19.58 MiB | 93.00 KiB/s, done.
Resolving deltas: 100% (221/221), done.
```

## 参考
https://stackoverflow.com/questions/24008982/git-access-to-private-repository-using-https