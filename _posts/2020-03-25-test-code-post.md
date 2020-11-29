---
layout: post
title: "My first test post"
description: "My first test post with code."
category: articles
tags: [sample post, readability, test]
comments: true
image:
  feature: "altai.jpg"
---


## Title


``` kotlin
private fun initMetricProcessors() {
    logger.info("Loading metrics processors")
    processors = metricsProcessorsLoader.load(pluginClasspath.toCollection(mutableListOf()))
    processors?.collectors?.forEach { collector ->
        collector.init(metricsStore, project)
    }
    logCollectorsAndDispatchers()
    project.whenBuildFinished { dispatchMetrics() }
}
```

{: .language-kotlin}

{% highlight kotlin linenos %}
private fun initMetricProcessors() {
    // comment
    logger.info("Loading metrics processors")
    processors = metricsProcessorsLoader.load(
      pluginClasspath.toCollection(mutableListOf())
    )
    processors?.collectors?.forEach { collector ->
        collector.init(metricsStore, project)
    }
    logCollectorsAndDispatchers()
    project.whenBuildFinished { dispatchMetrics() }
}
{% endhighlight %}


| Tables   |      Are      |  Cool |
|----------|:-------------:|------:|
| col 1 is |  left-aligned | $1600 |
| col 2 is |    centered   |   $12 |
| col 3 is | right-aligned |    $1 |



1. First ordered list item
2. Another item
⋅⋅* Unordered sub-list.
1. Actual numbers don't matter, just that it's a number
⋅⋅1. Ordered sub-list
4. And another item.

⋅⋅⋅You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

⋅⋅⋅To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
⋅⋅⋅Note that this line is separate, but within the same paragraph.⋅⋅
⋅⋅⋅(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses



# H1
## H2
### H3
#### H4
##### H5
###### H6

Alternatively, for H1 and H2, an underline-ish style:

Alt-H1
======

Alt-H2
------


Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~