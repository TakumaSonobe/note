# �v���C�x�[�g���|�W�g�������git clone

## ����
�����l������`git clone`���Ă݂�

```
git clone https://github.com/username/private-repository.git
```

��������G���[���Ԃ��Ă���

```
fatal: could not create leading directories of '@github.com:KatayamaLab/FCHEV-gym-model.git': Invalid argument
```

## �����@

����Ńv���C�x�[�g���|�W�g������N���[���ł���


```
git clone https://username@github.com/username/private-repository.git
```

(����)
`@github.com/username/private-repository.git`�̕����́Aclone with HTTPS �𗘗p���邱��

![git](https://github.com/TakumaSonobe/note/blob/master/How_to_use_Git/clone.PNG)

��肭�����Ƃ��̂悤�ȉ�ʂ��\�������

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

## �Q�l
https://stackoverflow.com/questions/24008982/git-access-to-private-repository-using-https