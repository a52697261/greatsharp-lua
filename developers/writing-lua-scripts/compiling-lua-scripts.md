# Compiling lua scripts

**Compiling scripts can give a slight performance boost, although you should be fine without it.**

\*\*\*\*

Download

1. Download the archive and extract it anywhere
2. Copy the script you want to compile into the extracted folder
3. Open command prompt, navigate to that folder

After you successfully extracted it, type the following command:

{% code title="compile.cmd" %}
```text
luajit.exe -b script.lua compiled.ljbc
```
{% endcode %}

