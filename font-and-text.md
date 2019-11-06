# Font and Text

## Font Collections

To specify which to use, one may use the **specific name of the font**, its **family name**, or its **collection name**.

| Family Name | Collection Name |
| :--- | :--- |
| Times New Roman | serif |
| Arial | sans-serif |
| Comic Sans | cursive |
| Impact | fantasy |
| Courier New | monospace |

To account for the possibility of users' browsers being unable to render certain fonts, multiple names can be listed like so:

```css
body {
    font-family: Arial, Helvetica, sans-serif;
}
```

**The order matters**: starting with the **left-most** mentioned name, the browser will attempt to render the selected elements' text using that font. This means that the **right-most** font that is mentioned is to be used as a **fail-safe.**

\*\*\*\*

