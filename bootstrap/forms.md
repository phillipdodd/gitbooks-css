# Forms

Official documentation [available here](https://getbootstrap.com/docs/4.0/components/forms/).

## Container

First, we need to create a **div** with the class name **container** to wrap our form in. To quote their [documentation](https://getbootstrap.com/docs/4.0/layout/overview/#containers):

> Containers are the most basic layout element in Bootstrap and are **required when using our default grid system.**

```markup
<div class="container">
// ...
</div>
```

## Form-Group

Each of our controls will need to be within a **div** with the class name **form-group**. To quote their [documentation](https://getbootstrap.com/docs/4.0/components/forms/#form-groups):

> The `.form-group` class is the easiest way to add some structure to forms. It provides a flexible class that encourages proper grouping of labels, controls, optional help text, and form validation messaging. By default it only applies `margin-bottom`, but it picks up additional styles in `.form-inline` as needed. Use it with `<fieldset>`s, `<div>`s, or nearly any other element.

```markup
<div class="container">
    <form>
    <div class="form-group">
        <label for="formGroupExampleInput">Example label</label>
        <input 
            type="text" 
            class="form-control" 
            id="formGroupExampleInput" 
            placeholder="Example input">
    </div>
</div>
```

{% hint style="info" %}
**Note:** it is important that the [**&lt;label&gt;** element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label)'s **for** attribute value is **equal to** its corresponding **&lt;input&gt;** element's value for **id**.
{% endhint %}

## Form-Check

It is important to note as well that the **&lt;label&gt;** can come _after_ the input in some cases, like with [a checkbox or radio control](https://getbootstrap.com/docs/4.0/components/input-group/#checkboxes-and-radios). 

Additionally, these controls use a **div** with a class name of **form-check** instead of **form-group:**

> Default checkboxes and radios are improved upon with the help of `.form-check`, **a single class for both input types that improves the layout and behavior of their HTML elements**. Checkboxes are for selecting one or several options in a list, while radios are for selecting one option from many.

{% hint style="info" %}
**Note:** While `.form-check` is required, `.form-group` can **still be used** for its styling benefits.
{% endhint %}

```markup
<div class="container">
    <form>
    <div class="form-group">
        <label for="formGroupExampleInput">Example label</label>
        <input 
            type="text" 
            class="form-control" 
            id="formGroupExampleInput" 
            placeholder="Example input">
    </div>
    <div class="form-check">
        <input 
            type="checkbox"
            class="form-check-input"
            id="emailOffers"
            name="emailOffers">
        <label
            class="form-check-label"
            for="emailOffers">
                Email Special Offers  
        </label>
    </div>
</div>
```

## 



