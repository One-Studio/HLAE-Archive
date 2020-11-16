# HLAE-Archive

从 [advancedfx原项目](https://github.com/advancedfx/advancedfx) 搬运得到，并用 JSdelivr 作为CDN加速，使用工具 [ReleaseDelivr](https://github.com/One-Studio/ReleaseDelivr)

## 最新HLAE下载链接示例：

> 版本号和zip文件名利用API获得，或者直接从download_link获得下载链接，见下文

https://cdn.jsdelivr.net/gh/One-Studio/HLAE-Archive@master/dist/hlae_2_109_2_1.zip
https://cdn.jsdelivr.net/gh/One-Studio/HLAE-Archive@master/dist/HLAE_Setup.exe

## 某个版本的下载链接

通过下面的API接口获取历史版本号，比如 `v2.109.2.1`，下载链接：

https://cdn.jsdelivr.net/gh/One-Studio/HLAE-Archive@v2.109.2.1/dist/hlae_2_109_2_1.zip

## 本搬运仓库API：

版本号：https://cdn.jsdelivr.net/gh/One-Studio/HLAE-Archive@master/version

下载链接（ `/n` 分割）：https://cdn.jsdelivr.net/gh/One-Studio/HLAE-Archive@master/download_link

API接口 Json格式：https://cdn.jsdelivr.net/gh/One-Studio/HLAE-Archive@master/api.json

| API          | 类型     | 含义                                          |
| ------------ | -------- | --------------------------------------------- |
| Version      | string   | 版本号                                        |
| VersionList  | []string | 历史版本                                      |
| ReleaseTime  | string   | 最新版本的发布时间 (格式2020-10-20T12:16:01Z) |
| Checktime    | string   | 搬运时检查的时间                              |
| DownloadLink | []string | 下载链接                                      |
| Format       | int      | 格式(1=7z, 2=zip)                             |
| ReleaseNote  | string   | 更新日志                                      |