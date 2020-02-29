
The simplified and slightly modified version of [Lumberjack](https://github.com/natefinch/lumberjack) package that integrates nicely with the [Zap](https://github.com/uber-go/zap) sugarred logging which has a 4-10x faster than the other structured logging.

Both Zap and Lumberjack simplified by the [ITRLog](https://github.com/itrepablik/itrlog) package.
 
# Installation
```
go get github.com/itrepablik/lumberjack
```

# Modified Version of Lumberjack
The main reason why we have some modified version of Lumberjack package because of this line [#222](https://github.com/natefinch/lumberjack/blob/v2.0/lumberjack.go) from the original source code of Lumberjack.  This function **openNew** will be executed during the log rotation which **renamed** the existing backup log file and then backup the 

# License
Code is distributed under MIT license, feel free to use it in your proprietary projects as well.
