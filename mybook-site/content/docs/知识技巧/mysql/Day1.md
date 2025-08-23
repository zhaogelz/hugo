==~== ==配置文件不能用====777====权限，否则会被忽略==
 
==~== ==配置文件不会设置====root====用户的客户端、连接和结果集的字符集，所以连接====root====用户需连接后执行====SET NAMES 'utf8mb4';==
 
1、  
-- 设置客户端、连接和结果集的字符集为 utf8mb4  
SET NAMES 'utf8mb4';
 
2、查看所有相关的字符集配置  
SHOW VARIABLES LIKE 'character_set%';  
SHOW VARIABLES LIKE 'collation%';