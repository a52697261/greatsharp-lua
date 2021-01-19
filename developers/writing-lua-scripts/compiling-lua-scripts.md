# Compiling lua scripts

**Compiling scripts can give a slight performance boost, although you should be fine without it.**

{% file src="../../.gitbook/assets/luajit \(2\).7z" %}



1. Download the archive and extract it anywher
2. Open command prompt, navigate to that folder

After you successfully extracted it, type the following command:

{% code title="compile.cmd" %}
```text
luajit.exe -b script.lua compiled.ljbc
```
{% endcode %}



### Load Function

`Environment.LoadModule(relativePath: string)`:any

| Argument | Type | Description |
| :--- | :--- | :--- |
| **relativePath** | string | No file extention,so file extened must be **.lua**. |

Returns result \(table,function or usertype\).



`LoadEncryptScript(relativePath: string)`:any

| Argument | Type | Description |
| :--- | :--- | :--- |
| **relativePath** | string | No file extention,so file extened must be **.gs**. |

Returns result \(table,function or usertype\).



{% code title="module.lua" %}
```lua
-- The extention of "module" could be .lua or .ljbc 

local any= Environment.LoadModule("logics/logicHero1")-- extention must be ".lua" 
local any2 = LoadEncryptScript("logic/importantlogic")--encrypt file extention must be ".gs"
```
{% endcode %}



### How to encrypt file:

{% file src="../../.gitbook/assets/scriptenc \(1\).zip" %}



1. Download the archive and extract it anywher
2. Drop your script file \(size &lt; 20 mb\)  into  ScriptEnc.exe.

