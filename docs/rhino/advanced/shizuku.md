# shizuku

v7.1.1 新增

要使用该模块请确保已安装[shizuku App](https://github.com/RikkaApps/Shizuku/releases)并激活，
并且授予了此应用权限，对于 root 用户也可以选择安装[Sui](https://github.com/RikkaApps/Sui) (未进行测试)

使用 shizuku 可以以更高的权限执行 shell 命令，以及调用一些系统 api

## shizuku(cmd)

- cmd \{ string } shell 命令
- return \{ [ShellResult](./shell#shellresult) } 运行结果

使用 shizuku 运行一条 shell 命令，如果 shizuku 不可用将抛出错误

```js
shizuku("input tap 500 500");
```

## shizuku.isAlive()

- return \{ boolean }

返回 shizuku 是否可用
