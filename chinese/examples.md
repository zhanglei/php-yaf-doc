<?xml version="1.0" encoding="utf-8"?>
<!-- $Revision: 321987 $ -->

<chapter xml:id="yaf.examples" xmlns="http://docbook.org/ns/docbook" xmlns:xlink="http://www.w3.org/1999/xlink">
 &reftitle.examples;
 <example>
  <title>A classic Application directory layout</title>
  <screen>
<![CDATA[
- index.php 
- .htaccess 
+ conf
  |- application.ini //application config
- application/
  - Bootstrap.php   
  + controllers
     - Index.php //default controller
  + views    
     |+ index   
        - index.phtml //view template for default action
  + modules 
  - library
  - models  
  - plugins 
]]>
 </screen>
 </example>
 <example>
  <title>Entry</title>
  <para>index.php in the top directory is the only way in of the application, you should rewrite all request to it(you can use .htaccess in Apache+php_mod) </para>
   <programlisting role="php">
<![CDATA[
<?php
define("APPLICATION_PATH",  dirname(__FILE__));

$app  = new Yaf_Application(APPLICATION_PATH . "/conf/application.ini");
$app->bootstrap() //call bootstrap methods defined in Bootstrap.php
 ->run();
?>
]]>
   </programlisting>
 </example>

 <example>
  <title>Rewrite rule</title>
  <screen>
<![CDATA[
#for apache (.htaccess)
RewriteEngine On
RewriteCond %{REQUEST_FILENAME} !-f
RewriteRule .* index.php

#for nginx
server {
  listen ****;
  server_name  domain.com;
  root   document_root;
  index  index.php index.html index.htm;

  if (!-e $request_filename) {
    rewrite ^/(.*)  /index.php/$1 last;
  }
}

#for lighttpd
$HTTP["host"] =~ "(www.)?domain.com$" {
  url.rewrite = (
     "^/(.+)/?$"  => "/index.php/$1",
  )
}
]]>
  </screen>
 </example>

 <example>
  <title>Application config</title>
   <programlisting role="ini">
<![CDATA[
[yaf]
;APPLICATION_PATH is the constant defined in index.php
application.directory=APPLICATION_PATH "/application/" 

;product section inherit from yaf section
[product:yaf]
foo=bar
]]>
   </programlisting>
 </example>

 <example>
  <title>Default controller</title>
   <programlisting role="php">
<![CDATA[
<?php
class IndexController extends Yaf_Controller_Abstract {
   /* default action */
   public function indexAction() {
       $this->view->word = "hello world";
   }
}
?>
?>
]]>
   </programlisting>
 </example>

 <example>
  <title>Default view template</title>
   <programlisting role="php">
<![CDATA[
<html>
 <head>
   <title>Hello World</title>
 </head>
 <body>
   <?php echo $word;?>
 </body>
</htlm>
]]>
   </programlisting>
  </example>

  <example>
   <title>Run the Applicatioin</title>
    &example.outputs.similar;
   <screen>
<![CDATA[
<html>
 <head>
   <title>Hello World</title>
 </head>
 <body>
   hello world
 </body>
</htlm>
]]>
   </screen> 
  </example>
</chapter>

<!-- Keep this comment at the end of the file
Local variables:
mode: sgml
sgml-omittag:t
sgml-shorttag:t
sgml-minimize-attributes:nil
sgml-always-quote-attributes:t
sgml-indent-step:1
sgml-indent-data:t
indent-tabs-mode:nil
sgml-parent-document:nil
sgml-default-dtd-file:"~/.phpdoc/manual.ced"
sgml-exposed-tags:nil
sgml-local-catalogs:nil
sgml-local-ecat-files:nil
End:
vim600: syn=xml fen fdm=syntax fdl=2 si
vim: et tw=78 syn=sgml
vi: ts=1 sw=1
-->