
# 定时重启

如果已经部署过 `v2ray` 应用, 不想每周升级, 请删除 `.github/workflows/upgrade.yml` 文件。

## 设置 Secrets 变量

  Settings >  Secrets

  添加

  - IBM_ENDPOINT: `https://api.us-south.cf.cloud.ibm.com`
  - IBM_USERNAME: 账号
  - IBM_PASSWORD: 密码
  - IBM_APPNAME: 你应用名称

## 修改文件名

  修改 `CI` 脚本 `.github/workflows/restart.yml.backup` 文件为 `.github/workflows/restart.yml` 即可。

  设置完毕后, 每周一凌晨0点, 都会重新启动 v2ray.
