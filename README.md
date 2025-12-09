# css-framework
A minimalistic, opinionated utility first css framework 
## Spacing

There are a handful of utilities for padding and margin. You can easily manipulate spacing horizontally, vertically, or all around. Macros such as `-auto` allow automatic centering behavior.

### Classes

#### Padding

| Class | Result | CSS |
| - | - | - |
| `p-{value}` | padding on all sides | `padding: {value};` |
| `px-{value}` | horizontal padding | `padding-left: {value}; padding-right: {value};` |
| `py-{value}` | vertical padding | `padding-top: {value}; padding-bottom: {value};` |
| `px-auto` | automatic horizontal spacing | `padding-left: auto; padding-right: auto;` |

#### Margin

| Class | Result | CSS |
| - | - | - |
| `m-{value}` | margin on all sides | `margin: {value};` |
| `mx-{value}` | horizontal margin | `margin-left: {value}; margin-right: {value};` |
| `my-{value}` | vertical margin | `margin-top: {value}; margin-bottom: {value};` |
| `mx-auto` | horizontal centering | `margin-left: auto; margin-right: auto;` |

---

### Values

Each key maps to a specific `rem` value (and corresponding pixel value).  
You may use numeric keys or macros (`sm`, `md`, `lg`, etc.), similar to Tailwind CSS.

| Numeric | Macro | Value (px) | Value (rem) | CSS |
|-----|--------|------------|-------------|-----|
| 0   | —      | 0px        | 0           | `padding: 0;` / `margin: 0;` |
| 1   | —      | 4px        | 0.25rem     | `padding: 0.25rem;` / `margin: 0.25rem;` |
| 2   | sm     | 8px        | 0.5rem      | `padding: 0.5rem;` / `margin: 0.5rem;` |
| 3   | —      | 12px       | 0.75rem     | `padding: 0.75rem;` / `margin: 0.75rem;` |
| 4   | md     | 16px       | 1rem        | `padding: 1rem;` / `margin: 1rem;` |
| 5   | —      | 20px       | 1.25rem     | `padding: 1.25rem;` / `margin: 1.25rem;` |
| 6   | lg     | 24px       | 1.5rem      | `padding: 1.5rem;` / `margin: 1.5rem;` |
| 8   | xlg    | 32px       | 2rem        | `padding: 2rem;` / `margin: 2rem;` |
| 10  | —      | 40px       | 2.5rem      | `padding: 2.5rem;` / `margin: 2.5rem;` |
| 12  | xxlg   | 48px       | 3rem        | `padding: 3rem;` / `margin: 3rem;` |


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


## Container Module

The container module contains a macro for declaring large width containers as well as macros for width manipulation in general.

## Containers

Containers provide fixed maximum widths for structuring page layouts. Each container size centers the content automatically and includes horizontal padding for consistent spacing.

| Container | Max Width | CSS |
|-------|-----------|------|
| `container-sm`   | 640px  | `max-width: 640px; margin-left: auto; margin-right: auto; padding-left: 1rem; padding-right: 1rem;` |
| `container-md`   | 768px  | `max-width: 768px; margin-left: auto; margin-right: auto; padding-left: 1rem; padding-right: 1rem;` |
| `container-lg`   | 1024px | `max-width: 1024px; margin-left: auto; margin-right: auto; padding-left: 1rem; padding-right: 1rem;` |
| `container-xlg`  | 1280px | `max-width: 1280px; margin-left: auto; margin-right: auto; padding-left: 1rem; padding-right: 1rem;` |
| `container-xxlg` | 1536px | `max-width: 1536px; margin-left: auto; margin-right: auto; padding-left: 1rem; padding-right: 1rem;` |


### Width Utilities

You can apply width using fixed rem-based values (`xxs` → `xxxlg`) or functional macros (`full`, `fit`, `max`, `screen`).

#### Values

| Width  | Value (rem) | Value (px) | CSS |
|--------|-------------|------------|-----|
| xxs    | 0.5rem      | 8px        | `width: 0.5rem;` |
| xs     | 1rem        | 16px       | `width: 1rem;` |
| sm     | 1.5rem      | 24px       | `width: 1.5rem;` |
| md     | 2rem        | 32px       | `width: 2rem;` |
| lg     | 2.5rem      | 40px       | `width: 2.5rem;` |
| xlg    | 3rem        | 48px       | `width: 3rem;` |
| xxlg   | 3.5rem      | 56px       | `width: 3.5rem;` |
| xxxlg  | 4rem        | 64px       | `width: 4rem;` |

#### Macros

| Macro  | CSS |
|--------|------|
| full   | `width: 100%;` |
| fit    | `width: fit-content;` |
| max    | `width: max-content;` |
| screen | `width: 100vw;` |