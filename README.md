# Mac-Brew
针对mac os安装问题

最近在mac os上安装homebrew时遇到一些问题：
在根据官网指导执行 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)”命令成功后，执行brew时提示-bash: brew: command not found
搜索相关资料后，发现解决办法如下:在终端执行 sudo vim .bash_profile -> PATH=/user/local/bin:$PATH -> source .bash_profile -> 重启终端
然而我发现还是提示-bash: command not fonud，可能是我还有一些操作未执行
最后我找到一篇提供了比较合理的解决办法的文章，而且很详细，最终的结果也是可以正常安装homebrew，执行brew命令成，文章链接:https://blog.csdn.net/H_Zaiii/article/details/105615597?depth_1-utm_source=distribute.pc_relevant.none-task-blog-OPENSEARCH-1&utm_source=distribute.pc_relevant.none-task-blog-OPENSEARCH-1
