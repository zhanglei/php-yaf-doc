# 运行时配置 

这些函数的行为受 php.ini 中的设置影响。

## Yaf 配置选项
名字 |	默认 |	可修改范围 |	更新日志
--  | -- |  -- | --
yaf.library	 | | 	its PHP_INI_ALL  value	| 
yaf.action_prefer	| 0|	its PHP_INI_ALL value	|
yaf.lowcase_path	| 0 |	its PHP_INI_ALL value	|
yaf.use_spl_autoload |	0 |	its PHP_INI_ALL value	 |
yaf.forward_limit|	5 |	its PHP_INI_ALL value	|
yaf.name_suffix	 | 1|	its PHP_INI_ALL value	 |
yaf.name_separator | |	 	its PHP_INI_ALL value	|
yaf.cache_config	| 0	| its PHP_INI_SYSTEM value	|
yaf.environ	 | product |	its PHP_INI_SYSTEM value	|
yaf.use_namespace|	0|	its PHP_INI_ALL value	|
这是配置指令的简短说明。

## 说明
* yaf.library string
The global library path, Yaf_loader will search global library in this directory.

* yaf.action_prefer integer
If there is only one part in PATH_INFO, should it consider as a controller or action.

If this configure On, it will be considered as a Action name.

* yaf.lowcase_path integer
Whether lowercase all the path during the class autoloading.

* yaf.use_spl_autoload integer
When this value is On, if Yaf_Loader can not find a class, it will return FALSE, then give chance to other auto load function to be called.

When this value is Off(default), Yaf_Loader::autoload() will always return TRUE.

* yaf.forward_limit integer
The max forward count, default is 5. that means you can have a max value of 5 in the forward stack.

This is a protection for prevent recursive Yaf_Controller_Abstract::forward().

* yaf.name_suffix integer
When this On, Yaf_Loader will identify a class by it's suffix to decide whether it is a MVC Class.

When this Off, Yaf_Loader will look at the prefix of the class name.

* yaf.name_separator string
When this is not empty, Yaf_Loader will identify the class suffix and string value of this.

For example, when this value is "_", Yaf_Loader will take Index_Controller as a Controller Class, IndexController as a normal class.

* yaf.cache_config integer
If this is On, and in the meantime you are using ini config file as the parameter of Yaf_Application(), the compiling result of the ini config file will be cached in the PHP process.

Note:
Yaf examine the mtime of the ini file, if it was changed since last compiling, Yaf will reload it.
Warning
Yaf use the ini file path as the cache entry key, so do use the absolute path in ini file path, otherwise there might be some conflicts if two application use the same relative path of ini config.
* yaf.environ string
This value is "product" by default, used for Yaf to fetch the config section of a ini config file.

That is, if this value is "product", Yaf will use the section named "product" in the ini config file(the first parameter of the Yaf_Application) as the final config of the Yaf_Application.

* yaf.use_namespace integer
Only works as of PHP 5.3, if this value is On, All class of Yaf will named in namespace style.

For example, Yaf_Route_Rewrite => \Yaf\Route\Rewrite, Yaf_Controller_Abstract => \Yaf\Controller_Abstract (Abstract is the keyword, can not used as a class name)