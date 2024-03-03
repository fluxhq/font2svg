

font2svg is a FREE API that returns SVG of text rendered in a given font. RTL fonts are supported. fonts with ligatures and kernings like kanji also supported. 

Use with `vercel/og` to render fonts with ligatures, kernings and also RTL fonts. For example arabic and hindi fonts don't render correctly with `vercel/og`. You don't need to bundle fonts with your edge function as well.

## Usage

Copy the below link in your browser to see it working. That's it, you don't need any api keys for now.


### Request


```
http://font2svg.pages.dev/api/tosvg?text=Render Me&font_size=20&font_family=Noto Sans&font_weight=400&font_style=italic
```


| parameter | values | comments | 
|----------|----------|----------|
| text `required` | any string with no new lines | 
| font_size `optional` | defaults to `12` | 
| font_family `optional` | google font family name e.g `Noto Sans`  | Check table below for all font family names
| font_weight `optional`| `100\|200\|300\|400\|500\|600\|700\|800\|900\|` | defaults to `400`. Check table below for supported weights of a particular font.
| font_style `optional` | `normal\|italic` | defaults to `normal`

## NOTE
1. You have to encode URL params as text might contain spaces.
2. Please open a github issue if you want extra features or report bugs.

## List of Google Fonts

| Font Family | Weights | Styles |
|----------|----------|----------|
| Noto Sans | `100\|200\|300\|400\|500\|600\|700\|800\|900` | italic,normal |
| Row 2, Column 1 | Row 2, Column 2 | Row 2, Column 3 |
| Row 3, Column 1 | Row 3, Column 2 | Row 3, Column 3 |
