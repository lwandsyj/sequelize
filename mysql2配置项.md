+ host: 主机名，默认localhost

+ prot ： mysql 端口号，默认 3306

+ user: mysql 用户名

+ password: 密码

+ database: 要连接的数据库

+ charset: 字符集，这在MySQL的SQL级别（如utf8_general_ci）中称为“排序规则” 。如果指定了SQL级字符集（如utf8mb4），则使用该字符集的默认排序规则。（默认值：'UTF8_GENERAL_CI'

+ timezone: 在MySQL服务器上配置的时区。这用于将类型转换服务器的日期/时间值键入JavaScript Date对象，反之亦然。这可以是'local'，'Z'或形式的偏移+HH:MM或-HH:MM。（默认值：'local'）

         timezone: '+08:00',

+ connectTimeout：与MySQL服务器的初始连接期间发生超时之前的毫秒数。（默认值：10000）

+ supportBigNumbers：当处理数据库中的大数（BIGINT和DECIMAL列）时，应启用此选项（默认值：）false

+ bigNumberStrings：同时启用supportBigNumbers和bigNumberStrings强制将大数字（BIGINT和DECIMAL列）始终作为JavaScript String对象返回（默认值：）false

+ dateStrings：强制日期类型（TIMESTAMP，DATETIME，DATE）以字符串形式返回，而不是膨胀为JavaScript Date对象。可以是true/ false或要保留为字符串的类型名称数组。（默认值：false）

+ debug：将协议详细信息打印到stdout。可以是true/ false或应该打印的包类型名称数组。（默认值：false）

+ trace：生成堆栈跟踪Error以包括库入口的调用站点（“长堆栈跟踪”）。大多数通话的性能都会有所下降。（默认值：true）

+ ssl:

        ssl: {
            ca : fs.readFileSync(__dirname + '/mysql-ca.crt')
        }