# uclog
使用golang编写的日志库

使用方法
1. 在配置中添加如下配置
  #日志等级: (debug, info, warn, error, critical)
  log_level = debug
  log_file = syslog
2. 初始化
  path := beego.AppConfig.String("log_file")
  level := beego.AppConfig.String("log_level")
  uclog.Initialize("templateserver", path, level)
