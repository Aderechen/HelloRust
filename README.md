
# Install Rust And toolchains
1.安装 Homebrew（macOS系统，如果还没有安装）:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. 使用 Homebrew 安装 Rust：
```sh
brew install rustup
rustup-init
```

3. 配置Rust 环境：
按照提示进行配置，通常选择默认选项即可。
```sh
Current installation options:


   default host triple: aarch64-apple-darwin
     default toolchain: stable (default)
               profile: default
  modify PATH variable: yes
1) Proceed with standard installation (default - just press enter)
2) Customize installation
3) Cancel installation
```
3. 如果想要卸载Rust
```sh
rustup self uninstall
```


4. 初始化仓库
+ 打开终端，克隆仓库到本地：
```sh
git clone https://github.com/yourusername/yourrepository.git
```
+ 进入仓库目录：
```sh
cd yourrepository
```
+ 初始化 Cargo 项目：
```sh
cargo new .
```

5. Cargo 环境配置
根据你的提示信息，似乎需要重新启动当前的 shell，或者手动配置环境变量来包含 Cargo 的 bin 目录。以下是详细的步骤：
    1.   在终端中运行：
   ```sh
   . "$HOME/.cargo/env"
   ```
    2. 验证 Cargo 是否可用：
   ```sh
   cargo --version
   ```
    3. 编辑 `~/.zshrc` 文件，添加：
   ```sh
   . "$HOME/.cargo/env"
   ```
    4. 重新加载 `~/.zshrc` 文件：
   ```sh
   source ~/.zshrc
   ```
    5. 最后再验证一次 Cargo：
   ```sh
   cargo --version
   ```

完成这些步骤后，你应该可以在 macOS 上顺利使用 Rust 工具链了。如果还有其他问题，请随时告诉我。