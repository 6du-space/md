# 自动更新设计文档

哈希算法为 BLAKE2b

当前实现是 https://libsodium.gitbook.io/doc/hashing/generic_hashing

签名算法为 ed25519

当前实现是 https://libsodium.gitbook.io/doc/public-key_cryptography/public-key_signatures

更新有几个组成部分

1. 版本信息服务器前缀列表
2. 版本号地址
3. 版本清单 - 模块服务器列表的hash 模块的hash（可以有多个）
4. 模块服务器列表
5. 模块名称 - 版本号 - 校验HASH

