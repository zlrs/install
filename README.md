# Homebrew (un)installer
本repo已修改brew索引源为清华大学镜像。（参考：https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/）
通过本repo的`install.sh`脚本，安装时所使用的brew索引源就是清华的。
目前暂时需要手动将`$(brew --repo homebrew/core)`的地址也换为清华的homebrew-core地址。

## Install Homebrew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/zlrs/install/master/install.sh)"
git -C "$(brew --repo homebrew/core)" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-core.git
```

More installation information and options at https://docs.brew.sh/Installation.html.

### Linux and Windows 10 Subsystem for Linux

Install Homebrew on Linux and Windows 10 Subsystem for Linux: https://docs.brew.sh/Linuxbrew.

## Uninstall Homebrew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/uninstall.sh)"
```

Download the uninstall script and run `/bin/bash uninstall.sh --help` to view more uninstall options.
