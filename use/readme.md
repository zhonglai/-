* 目的

  可以更快速的使用tscancode进行代码扫描

* 配置方法

  1. 配置tscancode安装路径

     * 进入use目录下的 tscancode.cfg文件，将 release/linux/TscanCodeV2.14.2395.linux目录下的tscancode路径更新到配置文件

     * 将use目录下的tscancode给与可执行权限

       ```
       chmod a+x tscancode
       ```

   2. 将use目录下的tscancode文件 + tscancode.cfg文件更新到系统的PATH路径

      ```
      sudo cp tscancode tscancode.cfg /usr/local/bin
      ```

   3.  然后就可以在任意目录进行使用了

      ```
      tscancode x.c x.xml
      ```

      
