#  MY FIRST ASYNC I/O!
### 你学习NODE.JS赢得很多！
LEARN YOU THE NODE.JS FOR MUCH WIN!
### 我的第一个异步I / O！ （练习4的13）
MY FIRST ASYNC I/O! (Exercise 4 of 13) 

#### **编写一个使用单个异步文件系统操作的程序来读取一个文件，并将其中包含的换行符的数量打印到控制台（stdout），类似于运行   cat file | wc -l。**

Write a program that uses a single asynchronous filesystem operation to read a file and print the number of newlines it contains to the console (stdout), similar to running  cat file | wc -l.

#### **要读取的文件的完整路径将作为第一个命令行参数提供。**

The full path to the file to read will be provided as the first  command-line  argument.

# HINTS  提示 

#### 这个问题的解决方案与前面的问题几乎是一样的，除了现在必须使用Node.js方法： 异步。

The solution to this problem is almost the same as the previous problem  except you must now do it the Node.js way: ++asynchronous++. 

#### 而不是使用 fs.readFileSync（），你会想使用 fs.readFile（） ，而不是使用这个方法的返回值，你需要从一个回调函数中收集你传入的值作为第二个参数。要了解有关回调的更多信息，请查看：(https://github.com/maxogden/art-of-node#callbacks).  

Instead of   fs.readFileSync()  you will want to use   fs.readFile()   and  instead of using the return value of this method you need to collect the value from a callback function that you pass in as the second argument. To learn more about callbacks, check out:  
(https://github.com/maxogden/art-of-node#callbacks). 

#### 请记住，惯用的 Node.js 回调通常具有签名：

Remember that idiomatic Node.js callbacks normally have the signature:

     function callback (err, data) { /* ... */ }  
     
#### 所以你可以通过检查第一个参数是否为真来检查是否发生错误.如果没有错误,你应该有你的 Buffer 对象作为第二个参数。 和  readFileSync()  一样，你可以提供'utf8'作为第二个参数，并把回调作为第三个参数，你将得到一个字符串，而不是一个缓冲区。


 so you can check if an error occurred by checking whether the first
 argument is truthy. If there is no error, you should have your Buffer
 object as the second argument. As with  readFileSync() , you can supply'utf8' as the second argument and put the callback as the third argument and you will get a String instead of a Buffer.
 
####  通过将浏览器指向此处可以找到有关 fs 模块的文档：
####  file:///Users/dllo/.nvm/versions/node/v8.9.4/lib/node_modules/learnyounode /node_apidoc/fs.html

 Documentation on the fs module can be found by pointing your browser here: file:///Users/dllo/.nvm/versions/node/v8.9.4/lib/node_modules/learnyounode/node_apidoc/fs.html
  
 _________________________________________________________________________
 
####  » 要再次打印这些说明，请运行：*<font color=gray size=5 >learnyounode print</font><br/>*
 
» To print these instructions again, run: <font color=gray size=3 >learnyounode print</font><br/>
 
####  » 要在测试环境中执行程序，请运行：*<font color=gray size=5 >learnyounode run program.js</font><br/>*
» To execute your program in a test environment, run: <font color=gray size=3 >learnyounode run program.js</font><br/>

#### » 要验证您的程序，请运行：*<font color=gray size=5 >learnyounode verify program.js</font><br/>*
» To verify your program, run: ：<font color=gray size=3 >learnyounode verify program.js</font><br/>

#### » For help run: *<font color=gray size=5 >learnyounode help</font><br/>*
» 帮助运行：<font color=gray size=3 >learnyounode help</font><br/>


































