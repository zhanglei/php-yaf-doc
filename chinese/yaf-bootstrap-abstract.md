<?xml version="1.0" encoding="utf-8"?>
<!-- $Revision: 327529 $ -->

<phpdoc:classref xml:id="class.yaf-bootstrap-abstract" xmlns:phpdoc="http://php.net/ns/phpdoc" xmlns="http://docbook.org/ns/docbook" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:xi="http://www.w3.org/2001/XInclude">

 <title>The Yaf_Bootstrap_Abstract class</title>
 <titleabbrev>Yaf_Bootstrap_Abstract</titleabbrev>

 <partintro>

<!-- {{{ Yaf_Bootstrap_Abstract intro -->
  <section xml:id="yaf-bootstrap-abstract.intro">
   &reftitle.intro;
   <para>
     Bootstrap是用来在Application运行(run)之前做一些初始化工作的机制.
   </para>
   <para>
    你可以通过继承<classname>Yaf_Bootstrap_Abstract</classname>
    来定义自己的Bootstrap类.
   </para>
   <para>
    在Bootstrap类中所有以"_init"开头的公有的方法,
    都会被按照定义顺序依次在<methodname>Yaf_Application::bootstrap</methodname>
    被调用的时刻调用.
   </para>
  </section>
<!-- }}} -->

 <section role="examples">
  &reftitle.examples;
  <example>
   <title>Bootstrap example</title>
   <programlisting role="php">
<![CDATA[
<?php
   /* bootstrap class should be defined under ./application/Bootstrap.php */
   class Bootstrap extends Yaf_Bootstrap_Abstract {
        public function _initConfig(Yaf_Dispatcher $dispatcher) {
            var_dump(__METHOD__);
        }
        public function _initPlugin(Yaf_Dispatcher $dispatcher) {
            var_dump(__METHOD__);
        }
   }

   $config = array(
       "application" => array(
           "directory" => dirname(__FILE__) . "/application/",
       ),
   );
 
   $app = new Yaf_Application($config);
   $app->bootstrap();
?>
]]>
   </programlisting>
   &example.outputs.similar;
   <screen>
<![CDATA[
string(22) "Bootstrap::_initConfig"
string(22) "Bootstrap::_initPlugin"
]]>
   </screen>
  </example>
 </section>

  <section xml:id="yaf-bootstrap-abstract.synopsis">
   &reftitle.classsynopsis;

<!-- {{{ Synopsis -->
   <classsynopsis>
    <ooclass><classname>Yaf_Bootstrap_Abstract</classname></ooclass>

<!-- {{{ Class synopsis -->
    <classsynopsisinfo>
     <ooclass>
      <modifier>abstract</modifier>
      <classname>Yaf_Bootstrap_Abstract</classname>
     </ooclass>
    </classsynopsisinfo>
    <classsynopsisinfo role="comment">&Properties;</classsynopsisinfo>
    
    <classsynopsisinfo role="comment">&Methods;</classsynopsisinfo>
   </classsynopsis>
<!-- }}} -->

  </section>

 </partintro>

</phpdoc:classref>

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