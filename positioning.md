# Positioning

An elements **position** can be influenced via the **position** property using one of four values:

## Static Positioning

**Static positioning** stacks elements one after the other down the page. This is often referred to as the **flow of a document**. This refers to **block elements** only, as **in-line** elements will not create a new line for themselves. 

## Relative Positioning

**Relative positioning** moves the element from its default position in a particular direction. If **relative** is used, then the **way in which it is moved** is described by using all or some of the properties **left, top, right,** or **bottom.**

```css
#links {
    position: relative;
    top: 20px;
    left: 50px;
}
```

{% hint style="success" %}
To better understand **left, top, right,** and **bottom**, I have found that it is helpful to **add** the words **"from the"** to them when thinking about them. For example, `top: 20px;` is **20px** _**from**_ **the top** and `left: 50px;` is **50px** _**from**_ **the left.**
{% endhint %}

Despite the element _**appearing**_ to no longer be in its **default position**, it will still take up space in **document flow** as though it were _**still** in its_ **default position**_._ 

So, **relative** **positioning** does **not** remove an element from the **flow of the document**.

## Absolute and Fixed Positioning

**Both** of these positionings will **remove** an element from the **document flow** to a **fixed place**. Where it moves is determined by the **left, top, right,** and **bottom** properties like with **relative** positioning.

The difference is that **Absolute** is **relative to the body** of the document, whereas **Fixed** is **relative to the window.**

## Float

## Clear

