# splint 安装使用

1. 说明

   * splint是inux平台静态c代码检测工具

2. 安装

   * 下载 splint3.1.1 

   * 安装

     ```
     # 1. 解压缩
     tar -xvzf splint-3.1.1.Linux.tgz
     # 2. 配置
     cd splint-3.1.1
     sudo mkdir /usr/local/splint
     ./configure --prefix=/usr/local/splint
     # 3. 编译
     make
     (如果缺少相关的依赖请依次安装，aclocal + automake 的版本如果对不上，请修改Makefile，删除对应的版本号)
     # 4. 安装
     make install
     # 5. 配置环境变量
     sudo vim ~/.bashrc
     # 进入最后一行
     export PATH=$PATH:/usr/local/splint/bin
     
     export LARCH_PATH=/usr/local/splint/share/splint/lib
     
     export LCLIMPORTDIR=/usr/local/splint/share/splint/imports
     
     # 6. 配置文件生效
     source ~/.bashrc
     ```

3. 使用

   * splint xx.c

4. 本人编译的生成文件 out 目录下
