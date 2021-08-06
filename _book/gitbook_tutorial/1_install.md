# 安装GitBook

 ## 1、环境要求 
 > GitBook 是一个基于 Node.js 的命令行工具，所以要确保环境中已安装 Node.js.  
 检验Node.js是否安装成功  

 ```
  $ node -v
  v12.11.1
 ```

  ## 2、安装命令行工具 gitbook-cli
  > 通过npm命令来安装gitbook-cli，  执行命令：  

  ```
  $ npm install gitbook-cli -g
  ```  

   > 上面命令运行完成之后，你可以使用下面的命令来检验是否安装成功。  

  ```
  $ gitbook -V
  CLI version: 2.3.2
  Installing GitBook 3.2.3
  ```  

  ## 3、安装编辑器gitbook-editor
  * ### 1)、windows用户
  ```
  $ choco install gitbook-editor
  ```
  * ### 2)、mac用户  
  ```
  $ brew install gitbook-editor
  ```