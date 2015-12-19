# kindeditor-cos

基于腾讯云COS云对象存储的PHP富文本编辑器

编辑器是基于KindEditor 4.1.10 版本进行改进的 

为兼容PHP7，修改了部分 php/JSON.php 文件及COS原始include.php文件

demo.php 是演示文件，仅做测试使用！

file_manager_json.php 是图片中心，地址调用了OCS的地址，但本地路径还是调用tmp目录

达到100%兼容性还需要待研究！

主要修改两个文件： php/upload_json.php 和 php/Qcloud_cos/Conf.php

其他方面暂无其他的修改，php/Qcloud_cos/Conf.php主要改几个方面：

const APPID = 'ID'; //COS的ID
const SECRET_ID = 'COS的SECRET_ID';
const SECRET_KEY = 'COS的SECRET_KEY';
    
php/upload_json.php主要改几个方面：

$bucketName = "这里修改为你COS的bucket";


欢迎一起交流PHP

团队博客：http://tech.ynho.com

腾讯微博：http://t.qq.com/xinyi007

新浪微博：http://weibo.com/ynho

微信/QQ添加：xinyi007/59471（请注明：PHP技术交流） 