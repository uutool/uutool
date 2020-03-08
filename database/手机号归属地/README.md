# uutool
手机号码归属地数据库，数据最后更新于2019年11月，数据共计437142条。

## 数据来源

原始数据来源：https://github.com/xluohome/phonedata（非常感谢作者的精心整理！）

原始数据文件：（phonetmp.csv）
https://gitee.com/oss/phonedata/attach_files

数据在phonetmp.csv的基础上整理加入了区域相关信息

上游数据不能保证百分之百的准确，请使用时自行甄别。


## 数据表结构
phone_location.sql共分为2个表

### 号码段表：phone_list

id=>数据库自增ID

number=>7位长度的号码段

type=>运营商类型，1移动, 2联通, 3电信, 4电信虚拟, 5联通虚拟, 6移动虚拟，7电信卫星,8电信物联网

region_id=>区域ID，对应phone_region的id列

### 区域表：phone_region

id=>数据库自增ID

province =>区域省份

city=>区域城市

zip_code=>城市邮政编码

area_code=>区号

### CSV格式文件，phone_location.csv

结构类似于：1300000,1,2

同上表中的phone_list,第一列表示号码段，第二列为区域ID，第三列为运营商类型

### 想直接使用归属地查询工具？
https://uutool.cn/phone-batch/












