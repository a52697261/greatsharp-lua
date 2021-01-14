---
description: Root Menu.
---

# Menu

## property: <a id="property"></a>

* `page`\(integer\)
* `isVisible`\(boolean\)

## Functions: <a id="functions"></a>

### CreateMenu <a id="permashow"></a>

`UI.Menu.CreateMenu(name: string, displayName: string, page: number)`:Menu

| Argument | Type | Description |
| :--- | :--- | :--- |
| **name** | string | Internal name. |
| **displayName** | string | Display name. |
| **page** | number | Base menu page. |

Create and returns a root menu item.

**​**‌

### :AddTooltip <a id="addtooltip"></a>

`menu:AddTooltip(tooltipString: string)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **tooltipString** | string | Tooltip string. |



### :AddMenu <a id="permashow"></a>

`menu:AddMenu(name: string, displayName: string)`:Menu

| Argument | Type | Description |
| :--- | :--- | :--- |
| **name** | string | Internal name. |
| **displayName** | string | Display name. |

Create and returns sub menu.



### :AddCheckBox <a id="permashow"></a>

`menu:AddCheckBox(name: string, displayName: string, [defaultValue: boolean, callback:function])`:CheckBox

| Argument | Type | Description |
| :--- | :--- | :--- |
| **name** | string | Internal name. |
| **displayName** | string | Display name. |
| **defaultValue** | boolean | Default value. |
| **callback** | function | Callback when value change. |

Add a checkbox to menu.



### :AddColorPicker <a id="permashow"></a>

`menu:AddColorPicker(name: string, displayName: string, [defaultValue: color,hasCheckBox: boolean, checkBoxDefaultValue: boolean callback:function])`:ColorPicker

| Argument | Type | Description |
| :--- | :--- | :--- |
| **name** | string | Internal name. |
| **displayName** | string | Display name. |
| **defaultValue** | color | Default color value. |
| **hasCheckBox** | boolean | Has checkbox |
| **checkBoxDefaultValue** | boolean | Checkbox default value. |
| **callback** | function | Callback when value change. |

Add a colorpicker to menu.



### :AddInfo

`menu:AddInfo(name: string, displayName: string)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **name** | string | Internal name. |
| **displayName** | string | Display name. |

Add an info text to menu.



### :AddKeyBind <a id="permashow"></a>

`menu:AddKeyBind(name: string, displayName: string, key: integer,  [defaultValue: boolean,isToggle: boolean, callback:function])`:KeyBind

| Argument | Type | Description |
| :--- | :--- | :--- |
| **name** | string | Internal name. |
| **displayName** | string | Display name. |
| **defaultValue** | boolean | Default color value. |
| **isToggle** | boolean | Is toggle. |
| **callback** | function | Callback when value change. |

Add a keybind to menu.



### :AddList <a id="permashow"></a>

`menu:AddList(name: string, displayName: string, items: string table,  [defaultValue: integer, callback:function])`:List

| Argument | Type | Description |
| :--- | :--- | :--- |
| **name** | string | Internal name. |
| **displayName** | string | Display name. |
| **items** | string table | Select items. |
| **defaultValue** | integer | Default select value. |
| **callback** | function | Callback when value change. |

Add a list to menu.



### :AddSlider <a id="permashow"></a>

`menu:AddSlider(name: string, displayName: string, defaultValue: integer, minimumValue: integer, maximumValue: integer,  [step: integer, callback:function])`:Slider

| Argument | Type | Description |
| :--- | :--- | :--- |
| **name** | string | Internal name. |
| **displayName** | string | Display name. |
| **defaultValue** | integer | Default value. |
| **minimumValue** | integer | Minimum value. |
| **maximumValue** | integer | Maximum value. |
| **step** | integer | Slider step per pix. |
| **callback** | function | Callback when value change. |

Add a slider to menu.









