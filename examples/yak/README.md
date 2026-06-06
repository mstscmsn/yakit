# Yaklang 示例脚本

这里是《[Yakit 使用指南](../../README.md)》第 10 章用到的全部 Yak 示例脚本，每个都**真实验证可运行**。

## 如何运行

**方式一：命令行（yak 引擎）**

```bash
# 注意是 yak <文件>，不是 yak run <文件>
yak 01_basic.yak
```

**方式二：Yakit 的 Yak Runner（图形界面）**

1. 打开 Yakit → 顶部菜单 **Yak Runner** → **打开文件**，选择某个 `.yak`。
2. 点击右上角橙色 **执行** 按钮，结果显示在底部「输出」面板。

## 关于本地测试目标

`06`~`11` 这几个网络相关的例子默认请求 `http://127.0.0.1:9999`。运行前可在本机起一个简易 HTTP 服务作为靶子：

```bash
python3 -m http.server 9999 --bind 127.0.0.1
```

## 文件列表

| 文件 | 演示内容 |
| --- | --- |
| `01_basic.yak` | 变量、类型、格式化输出 |
| `02_collection.yak` | 切片与 map、遍历 |
| `03_control.yak` | if / for / switch |
| `04_func.yak` | 函数、多返回值、闭包 |
| `05_str_codec.yak` | 字符串处理与编码哈希 |
| `06_error_concurrency.yak` | 错误处理与并发 |
| `07_http_poc.yak` | poc 库发 HTTP 包 |
| `08_fuzz.yak` | fuzz 库与 fuzztag |
| `09_servicescan.yak` | 端口扫描与指纹识别 |
| `10_crawler.yak` | 基础爬虫 |
| `11_yakit_output.yak` | yakit 库日志输出 |

> ⚠️ 仅可对你拥有合法授权的目标使用，详见主指南的「法律与合规声明」。
