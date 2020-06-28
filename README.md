# IBM Cloud Foundry (2020-09-14 14:00 更新)

- 第一步

  注册 [IBM Cloud](https://cloud.ibm.com/registration) 账号
  
- 第二步

  创建 [Cloud Foundry](https://cloud.ibm.com/catalog/starters/cloud-foundry?runtime=go)

- 第三步

  fork 本项目

- 添加 Secrets 变量

  Settings > Secrets

  添加

  - IBM_ENDPOINT: `https://api.us-south.cf.cloud.ibm.com`
  - IBM_USERNAME: 账号
  - IBM_PASSWORD: 密码
  - IBM_APPNAME: 你应用名称
  
  - APP_UUID: V2ray UUID, 可以作用 `http://www.uuid.online/` 生成一个。
  - APP_ALTERID: 额外ID, 建议使用 `0`
  - APP_WSPATH: 路径, 建议使用 `/`

- 修改 `README.md`

  设置完毕后, 

  修改任意文件保存, `CI` 就会执行, 并会立即更新 `v2ray`.

  且在, 每周一凌晨0点, 都会下载最新的 `v2ray` 推送到 `IBM` 云上。
