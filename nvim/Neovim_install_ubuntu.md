## 在ubuntu上手动安装neovim 0.9
- 下载neovim 0.9
  - https://github.com/neovim/neovim/releases/tag/v0.9.0 在本链接下载nvim.appimage
- 执行以下指令
  ```shell
  #添加执行权限
  chmod o+x nvim.appimage

  #解压缩
  ./nvim.appimage --appimage-extract

  #创建快速连接
  sudo mv squashfs-root /
  sudo ln -s /squashfs-root/AppRun /usr/bin/nvim
  nvim
  ```
