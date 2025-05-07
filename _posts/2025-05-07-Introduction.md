---
layout: post
title: Learn more about our motivations and research questions 
subtitle: "1 - General Introduction to our subject"
gh-repo: Julienv28/Final_Decoding_Biases
date: 2025-05-07
tags: [introduction]
comments: true
mathjax: true
author: Aiza Sakieva
---

Facial recognition technology is becoming increasingly integral to everyday life in Europe. Its deployment spans a growing number of domains, including - but not limited to - the following (TrendMatrix Analytics, 2025; Vito Fabbrizio, 2025):
- Law enforcement & public safety: Used in airports (e.g., Thales Group’s identity verification systems) and in densely populated areas for suspect identification.
- Border control: Facilitating travel through biometric authentication at EU borders, thereby reducing processing times.
- Retail & finance: Enabling personalized consumer experiences (e.g., Amazon Rekognition analyzing customer emotions) and supporting contactless payment solutions.
- Consumer electronics: Used for smartphone authentication and smart home system integration.

The European facial recognition market is projected to reach €1.35 billion by 2025, driven by a compound annual growth rate of 16.7% (Statista, 2025). This growth is fueled by advances in artificial intelligence, the post-COVID digitalization of services, and the development of regulatory frameworks such as the General Data Protection Regulation (GDPR).
Given such widespread use of the technology, it is crucial to address and eliminate algorithmic bias to ensure equal access to services, fair treatment, and uphold the fundamental right to non-discrimination across the European Union.
This project focuses specifically on algorithmic discrimination against the transgender community, a population that is especially exposed to the consequences of visual misclassification. Transgender individuals are particularly vulnerable to how visual perception influences social recognition, and visual conformity with one’s affirmed gender identity has been shown to significantly affect transgender people’s mental health (To et al., 2020).

Our study addresses the following research question

{: .box-success}
Do AI facial recognition algorithms exhibit gender and age-based discrimination toward the transgender community, and if so, to what extent?

To answer this question, we are going to test the following hypotheses:
1) AI facial recognition algorithms exhibit gender-based discrimination toward the transgender community.
2) AI facial recognition algorithms exhibit age-based discrimination toward the transgender community.
3) The level of gender-based discrimination is higher for transgender individuals than for cisgender individuals.
4) The accuracy of facial recognition algorithms varies significantly across different age groups within the transgender community.

We anticipate that all four hypotheses will be supported, meaning that the AI facial recognition algorithm will systematically misgender transgender people, inaccurately assess their age; furthermore, these inaccuracies are expected to occur more frequently for transgender individuals compared to cisgender individuals, and the degree of misclassification is expected to increase with age.
  In the following sections, we present a review of the relevant literature, outline our methodological approach, and provide a detailed analysis and discussion of our empirical findings.

## References

Statista. “Facial Recognition - Europe ; Statista Market Forecast.” Statista, 2025. https://www.statista.com/outlook/tmo/artificial-intelligence/computer-vision/facial-recognition/europe.

To, Margaret, Qi Zhang, Andrew Bradlyn, Darios Getahun, Shawn Giammattei, Rebecca Nash, Ashli A. Owen-Smith, et al. “Visual Conformity with Affirmed Gender or ‘Passing’: Its Distribution and Association with Depression and Anxiety in a Cohort of Transgender People.” The Journal of Sexual Medicine 17, no. 10 (October 2020): 2084–92. https://doi.org/10.1016/j.jsxm.2020.07.019.

TrendMatrix Analytics. “Europe Facial Recognition Market Analysis the Europe Facial Recognition Market Has Experienced Significant Growth in Recent Years and Is Expected to Continue Its Upward Trajectory over the next 5–10 Years.” Linkedin.com, March 31, 2025. https://www.linkedin.com/pulse/europe-facial-recognition-market-size-regional-trends-ktkff/.

Vito Fabbrizio. “Facial Recognition for Borders and Travel: 2025 Trends and Insights.” Biometric Update. BiometricUpdate.com, January 20, 2025. https://www.biometricupdate.com/202501/facial-recognition-for-borders-and-travel-2025-trends-and-insights.

<!-- {: .box-success}
This is a demo post to show you how to write blog posts with markdown.  I strongly encourage you to [take 5 minutes to learn how to write in markdown](https://markdowntutorial.com/) - it'll teach you how to transform regular text into bold/italics/tables/etc.<br/>I also encourage you to look at the [code that created this post](https://raw.githubusercontent.com/daattali/beautiful-jekyll/master/_posts/2020-02-28-sample-markdown.md) to learn some more advanced tips about using markdown in Beautiful Jekyll.

**Here is some bold text**

## Here is a secondary heading

[This is a link to a different site](https://deanattali.com/) and [this is a link to a section inside this page](#local-urls).

Here's a table:



You can use [MathJax](https://www.mathjax.org/) to write LaTeX expressions. For example:
When \\(a \ne 0\\), there are two solutions to \\(ax^2 + bx + c = 0\\) and they are $$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

How about a yummy crepe?

![Crepe](https://beautifuljekyll.com/assets/img/crepe.jpg)

It can also be centered!

![Crepe](https://beautifuljekyll.com/assets/img/crepe.jpg){: .mx-auto.d-block :}

Here's a code chunk:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.

## Local URLs in project sites {#local-urls}

When hosting a *project site* on GitHub Pages (for example, `https://USERNAME.github.io/MyProject`), URLs that begin with `/` and refer to local files may not work correctly due to how the root URL (`/`) is interpreted by GitHub Pages. You can read more about it [in the FAQ](https://beautifuljekyll.com/faq/#links-in-project-page). To demonstrate the issue, the following local image will be broken **if your site is a project site:**

![Crepe](/assets/img/crepe.jpg)

If the above image is broken, then you'll need to follow the instructions [in the FAQ](https://beautifuljekyll.com/faq/#links-in-project-page). Here is proof that it can be fixed:

![Crepe]({{ '/assets/img/crepe.jpg' | relative_url }})

<details markdown="1">
<summary>Click here!</summary>
Here you can see an **expandable** section
</details> -->
