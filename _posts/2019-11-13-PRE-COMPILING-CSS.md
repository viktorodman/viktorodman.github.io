---
layout: post
title: Pre-compiling CSS
img: /assets/pre-css.png/
permalink: /posts/pre-compiling-css/
comments: true
---

# What do you think of pre-compiling your CSS?

#### Compare to regular CSS?

Compared to regular css I think being able to nest my css selectors is a really good feature.
It makes the code much more readable.

Mixins is also a very good feature. Mixins makes it possible to encapsulate css code. This allows us to reuse code by including it in other styles in our css documents. 

#### Which techniques did you use?

I used variables, nested css and mixins.

{% highlight SCSS %}
// VARIABLES
$text-color:       rgb(0, 0, 0) !default;
$background-color: rgb(160, 160, 160) !default;
$brand-color:      #f2b83a !default;
$footer-color: 	   #0e0e0e !default;
$content-color:    rgb(211, 211, 211) !default;
// NESTED CSS
.page-link {
    @include relative-font-size(2);
    color: $grey-color-light;
    line-height: $base-line-height;

    &:not(:last-child) {
      margin-right: 20px;
    }
    &:hover {
      color: $brand-color;
    }
  }
  // MIXINS
  @mixin relative-font-size($ratio) {
  font-size: $base-font-size * $ratio;
}
{% endhighlight %}

#### Pros and Cons?

* Pros 

  * Readability.
  * Mixins.
  * "DRY" code.

* Cons

  * Debugging.
  * You have to learn the pre-processor syntax.