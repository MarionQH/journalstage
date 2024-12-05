# Why are "quotes" important in tailwind.css

## Today, I discovered something silly about quotes in **tailwind.css**

While working on our Adonis6.js project, we installed **tailwind.css** to work faster on our page's style.

But, while doing the indentation, we accidently took off the **"quotes"** on this line :

 ```html
<div class=text-xl max-w-2xl mx-auto mt-6>
```

**_We didn't immediatly notice_ !**

We took 20 mins searching why only the `text-xl` was working, until we noticed unlike our other lines, the **"quotes" were missing**. Then we wondered why the first attribute was still working.

### But why are quotes mendatory in tailwind.css ?

#### Well, in our example

```html
<div class=text-xl max-w-2xl mx-auto mt-6>
```

The browser reads `class=text-xl` as **valid**, but then treats `max-w-2xl`, `mx-auto`, and `mt-6` as **separate invalid attributes**, which won't work as intended.

#### When you use quotes

```html
<div class="text-xl max-w-2xl mx-auto mt-6">
```

The entire value is grouped together properly as the value of the `class` attribute.

## So, that's why quotes in tailwind.css are important
