#v5应用说明
后台登录处理
readme.md-cms
1 #本堂课讨论登录
2 ##管理员（用数据库来记录）
3 管理员对象属性
ID  帐号    密码
1   admin   xxxx
2   root    xxxx

define('GROUP_PATH','Cms/');

Cms/App(放置所有应用的目录)
Cms/App/V5(v5应用只管理，后台登录，退出，界面显示)
通过v5应用登录后台
Cms/App/V5/Control/LoginControl.class.php/Login
url写法：
http://localhost/v5/cms/index.php/v5/login/login
http://localhost/v5/cms/index.php/v5/login/code
 admin   7fef6171469e8Dd32c0559f88b377245

$_SESSION=array();
session_unset();
session_destroy();
//session(NULL);
文章
栏目
栏目表(Table)
cid 栏目名称  父级(pid)  关键字 (keywords)  描述(description)


娱乐-》{
   电影
   明星-》{体育 ，电影}
}

文章(Article)
aid
标题(title)
栏目(cid)
关键字(keywords)
描述(description)
正文(Content)
查看次数(click)
缩略图(thumb)
发布者(uid)
来源(source)
作者(author)
发表时间(addtime)
1970......2038秒数  数值
2013-2-22 ISO
更新时间(updatetime)
