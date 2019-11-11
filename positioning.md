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

**Remove** from the **default flow** to the left or right, allowing content to flow around it.

If there are three `<div>`'s positioned like so:

```markup
<html>
    <head>
        <style>
            p {
                width: 50px;
                border: 1px black solid;
            }
            .container {
                width: 200px;
            }
            .one {
                color: red;
            }
            .two {
                color: green;
            }
            .three {
                color: blue;
            }
        </style>
    </head>

    <body>
        <div class="container">
            <div class="one"><p>one</p></div>
            <div class="two"><p>two</p></div>
            <div class="three"><p>three</p></div>
        </div>
    </body>
</html>
```

![](.gitbook/assets/image%20%285%29.png)

This results in three `<div>` blocks flowing one after the other. If the first  and second one were to be `float`'ed to the `left`, the result would be:

![](.gitbook/assets/image%20%286%29.png)

Here we can see '**one'** and '**two'** having been both removed from the natural **document flow** and **'three'** placing its content as closely as it can to where it ought to as the only remaining element in the **document flow**. 

{% hint style="danger" %}
`<div>`'s and `<p>`'s probably are **not the best example** to use for this...
{% endhint %}

## Clear

Resets the **position of an element** to where it'd normally fall in the **document flow.** 

