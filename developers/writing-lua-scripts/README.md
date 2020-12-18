# Writing lua scripts

To get started with lua scripting, you'll need a suitable text editor. We suggest [VS Code](https://code.visualstudio.com/) or [Sublime Text](https://www.sublimetext.com/), but in theory [Notepad++](https://notepad-plus-plus.org/download/) or even the built-in Microsoft Notepad will probably work just fine. After choosing an editor, head over to

If you're unfamiliar with the Lua programming language, [Lua in 5 minutes](https://learnxinyminutes.com/docs/lua/) is a great guide to get started.



## Things to keep in mind:

* By default, all loaded lua modules **do not** share the same environment. This means that  2 modules could use a global variable with the same name.
* ~~To prevent this, always remember to make your variables, functions, etc **local**~~

