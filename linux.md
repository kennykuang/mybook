常用命令

1、文件中查看关键词：

cat -n  index.php | grep  test

解释：在文中index.php文件中查找 test关键词的行  -n表示展示行号，不展示行号可以去掉

2、查询文件中 从第10到第20行的记录

sed -n “10,20p”  index.php 
解释：查询index.php 从 10到20行之间的记录

3、查询从第20行 往后推20行的记录

cat -n index.php | tail -n +20 | head -n 20

4、cat -n index.php | grep test |more  查询结果交给more

5、cat -n index.php | grep test > /Users/smzdm/test.txt   查询test的结果 放在test.txt

6、cat index.php | wc -l    确定 index.php文件有多少行

7、ps -ef 查询进程  或者 ps aux 查询进程   杀死进程  kill -9  pid

8、ps -ef | grep php 查询PHP相关的进程

9、netstat -lntup 查端口  netstat -lntup

10、lsof -i:8000 lsof -:809 lsof i:808 lsof -i:80 查询某个端口的情况  lsof i:12121212

11、top  查询服务器状态 

12、free 查询内存使用情况

13、打开文件  cat index.php   tail -f index.php  vim index.php  小文件可以，大文件就不行了

推荐网址：https://link.juejin.im/?target=https%3A%2F%2Fmp.weixin.qq.com%2Fs%3F__biz%3DMzI4Njg5MDA5NA%3D%3D%26mid%3D2247484231%26idx%3D1%26sn%3D4cf217a4d692a7aba804e5d96186b15b%26chksm%3Debd74246dca0cb5024de2f1d9f9e2ecb631e49752713c25bbe44f44856e919df5a973049c189%26scene%3D21%23wechat_redirect




