# css-framework
A minimalistic, opinionated utility first css framework 

## Spacing

There are a handful of utilities for padding and margin. You can easily manipulate spacing horizontally, vertically or all around. There are also macro's for centering (-auto). 

### Classes

| Padding | Result |
| - | - |
|`p-{value}` | padding all around element (top, left, bottom, right) |
|`px-{value}` | horizontal padding (left, right) |
|`py-{value}` | vertical padding (top, bottom) |
|`px-auto` | applies automatic horizontal padding for centering elements. |

| Margin  | |
| - | - |
|`m-{value}` | margin all around element (top, left, bottom, right) |
|`mx-{value}` | horizontal margin (left, right) |
|`my-{value}` | vertical margin (top, bottom) |
|`mx-auto` | applies automatic horizontal padding for centering elements. |

### Values

Each key maps to a specific `rem` value (see table). You may use macros (sm, md, lg, ...) remniscent of Tailwind CSS, or numeric values.

| Numeric | Macro | Value (px) | Value (rem) |
|-----|--------|------|---------|
| 0   | —      | 0px  | 0       |
| 1   | —      | 4px  | 0.25rem |
| 2   | sm     | 8px  | 0.5rem  |
| 3   | —      | 12px | 0.75rem |
| 4   | md     | 16px | 1rem    |
| 5   | —      | 20px | 1.25rem |
| 6   | lg     | 24px | 1.5rem  |
| 8   | xlg    | 32px | 2rem    |
| 10  | —      | 40px | 2.5rem  |
| 12  | xxlg   | 48px | 3rem    |


### Examples

```html
<div class="p-4">
    Padding on all sides (top, left, right, bottom)

</div>
<div class="mx-2 my-sm">Horizontal and vertical margin of 0.5rem/8px (using both keys and macros)

</div>
<div class="px-lg py-1">
    Horizontal padding of 1.5rem/24px & vertical padding of 0.25rem / 4px
</div>
```