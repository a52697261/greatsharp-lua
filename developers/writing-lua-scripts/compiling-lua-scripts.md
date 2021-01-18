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

