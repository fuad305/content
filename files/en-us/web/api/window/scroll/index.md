---
title: Window.scroll()
slug: Web/API/Window/scroll
tags:
  - API
  - CSSOM View
  - Method
  - NeedsMarkupWork
  - Reference
browser-compat: api.Window.scroll
---
{{APIRef}}

The **`Window.scroll()`** method scrolls the window to a
particular place in the document.

## Syntax

```js
scroll(x-coord, y-coord)
scroll(options)
```

### Parameters

- `x-coord` is the pixel along the horizontal axis of the document that you
  want displayed in the upper left.
- `y-coord` is the pixel along the vertical axis of the document that you
  want displayed in the upper left.

\- or -

- `options`
  - : A dictionary containing the following parameters:
    - `top`
      - : Specifies the number of pixels along the Y axis to scroll the window or element.
    - `left`
      - : Specifies the number of pixels along the X axis to scroll the window or element.
    - `behavior`
      - : Specifies whether the scrolling should animate smoothly (`smooth`), or happen instantly in a single jump (`auto`, the default value).

## Examples

```html
<!-- put the 100th vertical pixel at the top of the window -->

<button onclick="scroll(0, 100);">click to scroll to the 100th pixel</button>
```

Using `options`:

```js
window.scroll({
  top: 100,
  left: 100,
  behavior: 'smooth'
});
```

## Notes

{{domxref("Window.scrollTo()")}} is effectively the same as this method. For relative
scrolling, see {{domxref("Window.scrollBy()")}}, {{domxref("Window.scrollByLines()")}},
and {{domxref("Window.scrollByPages()")}}.

For scrolling elements, see {{domxref("Element.scrollTop")}} and
{{domxref("Element.scrollLeft")}}.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{domxref("Window.scrollByLines()")}}
- {{domxref("Window.scrollByPages()")}}
- {{domxref("Element.scrollIntoView()")}}
