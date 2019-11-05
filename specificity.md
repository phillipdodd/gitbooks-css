# Specificity

**Credit:** [Introduction to CSS by Scott Allen](https://app.pluralsight.com/course-player?clipId=ff013ba8-5365-4a19-9aa7-8eeaed56dbdd)\*\*\*\*

**CSS rules** are applied in a **certain order** and this order is largely determined by **specificity.**

{% hint style="success" %}
There are **three categories** of **specificity** that together represent a **"three digit"** number.
{% endhint %}

For a number **ABC**, 

**A -** Count of **ID Selectors**

**B -** Count of **class** and **attribute** selectors

**C** - Count of **type** selectors

An illustration can be seen here:

```css
*            /* a=0 b=0 c=0 -> specificity = 0   */
LI           /* a=0 b=0 c=1 -> specificity = 1   */
UL LI        /* a=0 b=0 c=2 -> specificity = 2   */
LI.red       /* a=0 b=1 c=1 -> specificity = 11  */
#content     /* a=1 b=0 c=0 -> specificity = 100 */ 
```

