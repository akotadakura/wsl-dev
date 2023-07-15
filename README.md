# wsl-dev

## 実行

```shell
# cloneしたら、トップディレクトリでsudo実行に必要なパスワードをファイルに起こす
$ vim password
# 実行
$ ansible-playbook local.yml -e "ansible_become_password=`cat ./password`"
```