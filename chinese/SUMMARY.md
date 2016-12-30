# 目录


* [简介](README.md)
* [安装配置](setup.md)
    * [需求](requirement.md)
    * [安装](installation.md)
    * [运行时配置](runtime-configure.md)
    * [资源类型](resources.md)
* [预定义常量](constants.md)
* [范例](tutorials.md)
* [应用配置](appconfig.md)
* Yaf_Application — The Yaf_Application class
    * Yaf_Application::app — Retrieve an Application instance
    * Yaf_Application::bootstrap — Call bootstrap
    * Yaf_Application::clearLastError — Clear the last error info
    * Yaf_Application::__clone — Yaf_Application can not be cloned
    * Yaf_Application::__construct — Yaf_Application constructor
    * Yaf_Application::__destruct — The __destruct purpose
    * Yaf_Application::environ — Retrive environ
    * Yaf_Application::execute — Execute a callback
    * Yaf_Application::getAppDirectory — Get the application directory
    * Yaf_Application::getConfig — Retrive the config instance
    * Yaf_Application::getDispatcher — Get Yaf_Dispatcher instance
    * Yaf_Application::getLastErrorMsg — Get message of the last occurred error
    * Yaf_Application::getLastErrorNo — Get code of last occurred error
    * Yaf_Application::getModules — Get defined module names
    * Yaf_Application::run — Start Yaf_Application
    * Yaf_Application::setAppDirectory — Change the application directory
    * Yaf_Application::__sleep — Yaf_Application can not be serialized
    * Yaf_Application::__wakeup — Yaf_Application can not be unserialized
* Yaf_Bootstrap_Abstract — The Yaf_Bootstrap_Abstract class
* Yaf_Dispatcher — The Yaf_Dispatcher class
    * Yaf_Dispatcher::autoRender — Switch on/off autorendering
    * Yaf_Dispatcher::catchException — Switch on/off exception catching
    * Yaf_Dispatcher::__clone — Yaf_Dispatcher can not be cloned
    * Yaf_Dispatcher::__construct — Yaf_Dispatcher constructor
    * Yaf_Dispatcher::disableView — Disable view rendering
    * Yaf_Dispatcher::dispatch — Dispatch a request
    * Yaf_Dispatcher::enableView — enable view rendering
    * Yaf_Dispatcher::flushInstantly — Switch on/off the instant flushing
    * Yaf_Dispatcher::getApplication — Retrive the application
    * Yaf_Dispatcher::getInstance — Retrive the dispatcher instance
    * Yaf_Dispatcher::getRequest — Retrive the request instance
    * Yaf_Dispatcher::getRouter — Retrive router instance
    * Yaf_Dispatcher::initView — Initialize view and return it
    * Yaf_Dispatcher::registerPlugin — Register a plugin
    * Yaf_Dispatcher::returnResponse — The returnResponse purpose
    * Yaf_Dispatcher::setDefaultAction — Change default action name
    * Yaf_Dispatcher::setDefaultController — Change default controller name
    * Yaf_Dispatcher::setDefaultModule — Change default module name
    * Yaf_Dispatcher::setErrorHandler — Set error handler
    * Yaf_Dispatcher::setRequest — The setRequest purpose
    * Yaf_Dispatcher::setView — Set a custom view engine
    * Yaf_Dispatcher::__sleep — Yaf_Dispatcher can not be serialized
    * Yaf_Dispatcher::throwException — Switch on/off exception throwing
    * Yaf_Dispatcher::__wakeup — Yaf_Dispatcher can not be unserialized
* Yaf_Config_Abstract — The Yaf_Config_Abstract class
    * Yaf_Config_Abstract::get — Getter
    * Yaf_Config_Abstract::readonly — Find a config whether readonly
    * Yaf_Config_Abstract::set — Setter
    * Yaf_Config_Abstract::toArray — Cast to array
* Yaf_Config_Ini — The Yaf_Config_Ini class
    * Yaf_Config_Ini::__construct — Yaf_Config_Ini constructor
    * Yaf_Config_Ini::count — The count purpose
    * Yaf_Config_Ini::current — The current purpose
    * Yaf_Config_Ini::__get — The __get purpose
    * Yaf_Config_Ini::__isset — The __isset purpose
    * Yaf_Config_Ini::key — The key purpose
    * Yaf_Config_Ini::next — The next purpose
    * Yaf_Config_Ini::offsetExists — The offsetExists purpose
    * Yaf_Config_Ini::offsetGet — The offsetGet purpose
    * Yaf_Config_Ini::offsetSet — The offsetSet purpose
    * Yaf_Config_Ini::offsetUnset — The offsetUnset purpose
    * Yaf_Config_Ini::readonly — The readonly purpose
    * Yaf_Config_Ini::rewind — The rewind purpose
    * Yaf_Config_Ini::__set — The __set purpose
    * Yaf_Config_Ini::toArray — Returns a PHP array
    * Yaf_Config_Ini::valid — The valid purpose
* Yaf_Config_Simple — The Yaf_Config_Simple class
    * Yaf_Config_Simple::__construct — The __construct purpose
    * Yaf_Config_Simple::count — The count purpose
    * Yaf_Config_Simple::current — The current purpose
    * Yaf_Config_Simple::__get — The __get purpose
    * Yaf_Config_Simple::__isset — The __isset purpose
    * Yaf_Config_Simple::key — The key purpose
    * Yaf_Config_Simple::next — The next purpose
    * Yaf_Config_Simple::offsetExists — The offsetExists purpose
    * Yaf_Config_Simple::offsetGet — The offsetGet purpose
    * Yaf_Config_Simple::offsetSet — The offsetSet purpose
    * Yaf_Config_Simple::offsetUnset — The offsetUnset purpose
    * Yaf_Config_Simple::readonly — The readonly purpose
    * Yaf_Config_Simple::rewind — The rewind purpose
    * Yaf_Config_Simple::__set — The __set purpose
    * Yaf_Config_Simple::toArray — Returns a PHP array
    * Yaf_Config_Simple::valid — The valid purpose
* Yaf_Controller_Abstract — The Yaf_Controller_Abstract class
    * Yaf_Controller_Abstract::__clone — Yaf_Controller_Abstract can not be cloned
    * Yaf_Controller_Abstract::__construct — Yaf_Controller_Abstract constructor
    * Yaf_Controller_Abstract::display — The display purpose
    * Yaf_Controller_Abstract::forward — foward to another action
    * Yaf_Controller_Abstract::getInvokeArg — The getInvokeArg purpose
    * Yaf_Controller_Abstract::getInvokeArgs — The getInvokeArgs purpose
    * Yaf_Controller_Abstract::getModuleName — Get module name
    * Yaf_Controller_Abstract::getRequest — Retrieve current request object
    * Yaf_Controller_Abstract::getResponse — Retrieve current response object
    * Yaf_Controller_Abstract::getView — Retrieve the view engine
    * Yaf_Controller_Abstract::getViewpath — The getViewpath purpose
    * Yaf_Controller_Abstract::init — Controller initializer
    * Yaf_Controller_Abstract::initView — The initView purpose
    * Yaf_Controller_Abstract::redirect — Redirect to a URL
    * Yaf_Controller_Abstract::render — Render view template
    * Yaf_Controller_Abstract::setViewpath — The setViewpath purpose
* Yaf_Action_Abstract — The Yaf_Action_Abstract class
    * Yaf_Action_Abstract::execute — Action entry point
    * Yaf_Action_Abstract::getController — Retrieve controller object
* Yaf_View_Interface — The Yaf_View_Interface class
    * Yaf_View_Interface::assign — Assign value to View engine
    * Yaf_View_Interface::display — Render and output a template
    * Yaf_View_Interface::getScriptPath — The getScriptPath purpose
    * Yaf_View_Interface::render — Render a template
    * Yaf_View_Interface::setScriptPath — The setScriptPath purpose
* Yaf_View_Simple — The Yaf_View_Simple class
    * Yaf_View_Simple::assign — Assign values
    * Yaf_View_Simple::assignRef — The assignRef purpose
    * Yaf_View_Simple::clear — Clear Assigned values
    * Yaf_View_Simple::__construct — Constructor of Yaf_View_Simple
    * Yaf_View_Simple::display — Render and display
    * Yaf_View_Simple::eval — Render template
    * Yaf_View_Simple::__get — Retrieve assigned variable
    * Yaf_View_Simple::getScriptPath — Get templates directory
    * Yaf_View_Simple::__isset — The __isset purpose
    * Yaf_View_Simple::render — Render template
    * Yaf_View_Simple::__set — Set value to engine
    * Yaf_View_Simple::setScriptPath — Set tempaltes directory
* Yaf_Loader — The Yaf_Loader class
    * Yaf_Loader::autoload — The autoload purpose
    * Yaf_Loader::clearLocalNamespace — The clearLocalNamespace purpose
    * Yaf_Loader::__clone — The __clone purpose
    * Yaf_Loader::__construct — The __construct purpose
    * Yaf_Loader::getInstance — The getInstance purpose
    * Yaf_Loader::getLibraryPath — get the library path
    * Yaf_Loader::getLocalNamespace — The getLocalNamespace purpose
    * Yaf_Loader::import — The import purpose
    * Yaf_Loader::isLocalName — The isLocalName purpose
    * Yaf_Loader::registerLocalNamespace — register local class prefix
    * Yaf_Loader::setLibraryPath — Change the library path
    * Yaf_Loader::__sleep — The __sleep purpose
    * Yaf_Loader::__wakeup — The __wakeup purpose
* Yaf_Plugin_Abstract — The Yaf_Plugin_Abstract class
    * Yaf_Plugin_Abstract::dispatchLoopShutdown — The dispatchLoopShutdown purpose
    * Yaf_Plugin_Abstract::dispatchLoopStartup — The dispatchLoopStartup purpose
    * Yaf_Plugin_Abstract::postDispatch — The postDispatch purpose
    * Yaf_Plugin_Abstract::preDispatch — The preDispatch purpose
    * Yaf_Plugin_Abstract::preResponse — The preResponse purpose
    * Yaf_Plugin_Abstract::routerShutdown — The routerShutdown purpose
    * Yaf_Plugin_Abstract::routerStartup — RouterStartup hook
* Yaf_Registry — The Yaf_Registry class
    * Yaf_Registry::__clone — The __clone purpose
    * Yaf_Registry::__construct — Yaf_Registry implements singleton
    * Yaf_Registry::del — Remove an item from registry
    * Yaf_Registry::get — Retrieve an item from registry
    * Yaf_Registry::has — Check whether an item exists
    * Yaf_Registry::set — Add an item into registry
* Yaf_Request_Abstract — The Yaf_Request_Abstract class
    * Yaf_Request_Abstract::getActionName — The getActionName purpose
    * Yaf_Request_Abstract::getBaseUri — The getBaseUri purpose
    * Yaf_Request_Abstract::getControllerName — The getControllerName purpose
    * Yaf_Request_Abstract::getEnv — Retrieve ENV varialbe
    * Yaf_Request_Abstract::getException — The getException purpose
    * Yaf_Request_Abstract::getLanguage — The getLanguage purpose
    * Yaf_Request_Abstract::getMethod — The getMethod purpose
    * Yaf_Request_Abstract::getModuleName — The getModuleName purpose
    * Yaf_Request_Abstract::getParam — The getParam purpose
    * Yaf_Request_Abstract::getParams — The getParams purpose
    * Yaf_Request_Abstract::getRequestUri — The getRequestUri purpose
    * Yaf_Request_Abstract::getServer — Retrieve SERVER variable
    * Yaf_Request_Abstract::isCli — The isCli purpose
    * Yaf_Request_Abstract::isDispatched — The isDispatched purpose
    * Yaf_Request_Abstract::isGet — The isGet purpose
    * Yaf_Request_Abstract::isHead — The isHead purpose
    * Yaf_Request_Abstract::isOptions — The isOptions purpose
    * Yaf_Request_Abstract::isPost — The isPost purpose
    * Yaf_Request_Abstract::isPut — The isPut purpose
    * Yaf_Request_Abstract::isRouted — The isRouted purpose
    * Yaf_Request_Abstract::isXmlHttpRequest — The isXmlHttpRequest purpose
    * Yaf_Request_Abstract::setActionName — The setActionName purpose
    * Yaf_Request_Abstract::setBaseUri — set base URI
    * Yaf_Request_Abstract::setControllerName — The setControllerName purpose
    * Yaf_Request_Abstract::setDispatched — The setDispatched purpose
    * Yaf_Request_Abstract::setModuleName — The setModuleName purpose
    * Yaf_Request_Abstract::setParam — The setParam purpose
    * Yaf_Request_Abstract::setRequestUri — The setRequestUri purpose
    * Yaf_Request_Abstract::setRouted — The setRouted purpose
* Yaf_Request_Http — The Yaf_Request_Http class
    * Yaf_Request_Http::__clone — The __clone purpose
    * Yaf_Request_Http::__construct — Constructor of Yaf_Request_Http
    * Yaf_Request_Http::get — Retrieve variable from client
    * Yaf_Request_Http::getCookie — Retrieve Cookie variable
    * Yaf_Request_Http::getFiles — The getFiles purpose
    * Yaf_Request_Http::getPost — Retrieve POST variable
    * Yaf_Request_Http::getQuery — Fetch a query parameter
    * Yaf_Request_Http::getRequest — The getRequest purpose
    * Yaf_Request_Http::isXmlHttpRequest — Whether a Ajax Request
* Yaf_Request_Simple — The Yaf_Request_Simple class
    * Yaf_Request_Simple::__clone — The __clone purpose
    * Yaf_Request_Simple::__construct — Constructor of Yaf_Request_Simple
    * Yaf_Request_Simple::get — The get purpose
    * Yaf_Request_Simple::getCookie — The getCookie purpose
    * Yaf_Request_Simple::getFiles — The getFiles purpose
    * Yaf_Request_Simple::getPost — The getPost purpose
    * Yaf_Request_Simple::getQuery — The getQuery purpose
    * Yaf_Request_Simple::getRequest — The getRequest purpose
    * Yaf_Request_Simple::isXmlHttpRequest — The isXmlHttpRequest purpose
* Yaf_Response_Abstract — The Yaf_Response_Abstract class
    * Yaf_Response_Abstract::appendBody — append to body
    * Yaf_Response_Abstract::clearBody — The clearBody purpose
    * Yaf_Response_Abstract::clearHeaders — The clearHeaders purpose
    * Yaf_Response_Abstract::__clone — The __clone purpose
    * Yaf_Response_Abstract::__construct — The __construct purpose
    * Yaf_Response_Abstract::__destruct — The __destruct purpose
    * Yaf_Response_Abstract::getBody — Retrieve a exists content
    * Yaf_Response_Abstract::getHeader — The getHeader purpose
    * Yaf_Response_Abstract::prependBody — The prependBody purpose
    * Yaf_Response_Abstract::response — send response
    * Yaf_Response_Abstract::setAllHeaders — The setAllHeaders purpose
    * Yaf_Response_Abstract::setBody — Set content to response
    * Yaf_Response_Abstract::setHeader — The setHeader purpose
    * Yaf_Response_Abstract::setRedirect — The setRedirect purpose
    * Yaf_Response_Abstract::__toString — The __toString purpose
* Yaf_Route_Interface — The Yaf_Route_Interface class
    * Yaf_Route_Interface::assemble — assemble a request
    * Yaf_Route_Interface::route — route a request
* Yaf_Route_Map — The Yaf_Route_Map class
    * Yaf_Route_Map::assemble — Assemble a url
    * Yaf_Route_Map::__construct — The __construct purpose
    * Yaf_Route_Map::route — The route purpose
* Yaf_Route_Regex — The Yaf_Route_Regex class
    * Yaf_Route_Regex::assemble — Assemble a url
    * Yaf_Route_Regex::__construct — Yaf_Route_Regex constructor
    * Yaf_Route_Regex::route — The route purpose
* Yaf_Route_Rewrite — The Yaf_Route_Rewrite class
    * Yaf_Route_Rewrite::assemble — Assemble a url
    * Yaf_Route_Rewrite::__construct — Yaf_Route_Rewrite constructor
    * Yaf_Route_Rewrite::route — The route purpose
* Yaf_Router — The Yaf_Router class
    * Yaf_Router::addConfig — Add config-defined routes into Router
    * Yaf_Router::addRoute — Add new Route into Router
    * Yaf_Router::__construct — Yaf_Router constructor
    * Yaf_Router::getCurrentRoute — Get the effective route name
    * Yaf_Router::getRoute — Retrieve a route by name
    * Yaf_Router::getRoutes — Retrieve registered routes
    * Yaf_Router::route — The route purpose
* Yaf_Route_Simple — The Yaf_Route_Simple class
    * Yaf_Route_Simple::assemble — Assemble a url
    * Yaf_Route_Simple::__construct — Yaf_Route_Simple constructor
    * Yaf_Route_Simple::route — Route a request
* Yaf_Route_Static — The Yaf_Route_Static class
    * Yaf_Route_Static::assemble — Assemble a url
    * Yaf_Route_Static::match — The match purpose
    * Yaf_Route_Static::route — Route a request
* Yaf_Route_Supervar — The Yaf_Route_Supervar class
    * Yaf_Route_Supervar::assemble — Assemble a url
    * Yaf_Route_Supervar::__construct — The __construct purpose
    * Yaf_Route_Supervar::route — The route purpose
* Yaf_Session — The Yaf_Session class
    * Yaf_Session::__clone — The __clone purpose
    * Yaf_Session::__construct — Constructor of Yaf_Session
    * Yaf_Session::count — The count purpose
    * Yaf_Session::current — The current purpose
    * Yaf_Session::del — The del purpose
    * Yaf_Session::__get — The __get purpose
    * Yaf_Session::getInstance — The getInstance purpose
    * Yaf_Session::has — The has purpose
    * Yaf_Session::__isset — The __isset purpose
    * Yaf_Session::key — The key purpose
    * Yaf_Session::next — The next purpose
    * Yaf_Session::offsetExists — The offsetExists purpose
    * Yaf_Session::offsetGet — The offsetGet purpose
    * Yaf_Session::offsetSet — The offsetSet purpose
    * Yaf_Session::offsetUnset — The offsetUnset purpose
    * Yaf_Session::rewind — The rewind purpose
    * Yaf_Session::__set — The __set purpose
    * Yaf_Session::__sleep — The __sleep purpose
    * Yaf_Session::start — The start purpose
    * Yaf_Session::__unset — The __unset purpose
    * Yaf_Session::valid — The valid purpose
    * Yaf_Session::__wakeup — The __wakeup purpose
* Yaf_Exception — The Yaf_Exception class
    * Yaf_Exception::__construct — The __construct purpose
    * Yaf_Exception::getPrevious — The getPrevious purpose
    * Yaf_Exception_TypeError — The Yaf_Exception_TypeError class
    * Yaf_Exception_StartupError — The Yaf_Exception_StartupError class
    * Yaf_Exception_DispatchFailed — The Yaf_Exception_DispatchFailed class
    * Yaf_Exception_RouterFailed — The Yaf_Exception_RouterFailed class
    * Yaf_Exception_LoadFailed — The Yaf_Exception_LoadFailed class
    * Yaf_Exception_LoadFailed_Module — The Yaf_Exception_LoadFailed_Module class
    * Yaf_Exception_LoadFailed_Controller — The Yaf_Exception_LoadFailed_Controller class
    * Yaf_Exception_LoadFailed_Action — The Yaf_Exception_LoadFailed_Action class
    * Yaf_Exception_LoadFailed_View — The Yaf_Exception_LoadFailed_View class