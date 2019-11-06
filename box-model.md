# Box Model

Every **HTML Element** produces a **"box"** on the webpage with three main properties that can be used to influence the CSS, the **Margin, Border,** and **Padding.** 

![](.gitbook/assets/image%20%281%29.png)

**Margin** is the property used to create space **around** the element, _**outside**_ of any **defined borders**. \([w3](https://www.w3schools.com/css/css_margin.asp)\)

**Padding** is the property used to create space around an **element's content**, _**inside**_ of any **defined borders.**

{% hint style="info" %}
**Margins** -- Outside! **Padding** -- Inside!
{% endhint %}

When defining the **values** for **margin,** and **padding** there are a few ways to go about it. \(Are there others?\)

The **first option** is to simplu specify the property and use a **single value**. This will apply the value to **each side**.

```css
ul li {
    padding: 10px;
}
```

The **second option** is to use the property name for the **specific side** you want to edit and supply **a single value**:

```css
ul li {
    padding-left: 10px;
}
```

The **third option** is to use **four values** - one for each side of the box. **The order in which you list the values is very important!** The order is:

> &lt;left&gt; &lt;top&gt; &lt;right&gt; &lt;bottom&gt;

That is, starting with the **left side** the numbers follow along the edge of the box in a **clockwise** manner..

{% hint style="danger" %}
**Note!** **Vertical Margins** will **collapse**. Meaning that if **two boxes, one atop the other**, both have **touching margins** of **5px**, the margin between them **will be 5px**, _not_ **10px**.
{% endhint %}

{% hint style="warning" %}
Box properties are **additive** - the **width** alone does _not_ include the distances added for **margin, padding,** or **borders.**
{% endhint %}

