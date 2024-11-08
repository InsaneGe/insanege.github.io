---
title: Black Myth
date: 2024-11-07 20:30:00 +0800 # 东八区（UTC/GMT+0800）是比世界协调时间（UTC）/格林尼治时间（GMT）快8小时的时区
categories: [杂想漫谈]
tags: [杂谈]     # TAG names should always be lowercase
authors: [Bohemian]
description: "一个轻度3A玩家玩黑神话后的碎碎念"
---



### 你怎么知道我无伤幽魂

{% include embed/bilibili.html id='BV1kJSVY3ECz' %}

### 迄今看到最优雅的识破仙人博主

{% include embed/bilibili.html id='BV1FcSyYREej' %}

### youtube测试

{% include embed/youtube.html id='Balreaj8Yqs' %}

### Links
[B站](https://www.bilibili.com)

<https://www.bilibili.com>


# H1 jekyll


## Prompts

<!-- markdownlint-capture --> 
<!-- markdownlint-disable -->

> An example showing the `tip` type prompt.
{: .prompt-tip }

> An example showing the `info` type prompt.
{: .prompt-info }

> An example showing the `warning` type prompt.
{: .prompt-warning }

> An example showing the `danger` type prompt.
{: .prompt-danger }
<!-- markdownlint-restore -->

## Images

### Default (with caption)

![Desktop View](/assets/images/avatar.jpg){: width="564" height="564" }
_Full screen width and center alignment_

### Left aligned

![Desktop View](/assets/images/avatar.jpg){: width="300" height="300" .w-75 .normal}

### Float to left

![Desktop View](/assets/images/avatar.jpg){: width="564" height="564" .w-50 .left}
乱文只是用于显示左浮效果Praesent maximus aliquam sapien. Sed vel neque in dolor pulvinar auctor. Maecenas pharetra, sem sit amet interdum posuere, tellus lacus eleifend magna, ac lobortis felis ipsum id sapien. Proin ornare rutrum metus, ac convallis diam volutpat sit amet. Phasellus volutpat, elit sit amet tincidunt mollis, felis mi scelerisque mauris, ut facilisis leo magna accumsan sapien. In rutrum vehicula nisl eget tempor. Nullam maximus ullamcorper libero non maximus. Integer ultricies velit id convallis varius. Praesent eu nisl eu urna finibus ultrices id nec ex. Mauris ac mattis quam. Fusce aliquam est nec sapien bibendum, vitae malesuada ligula condimentum.

### Dark/Light mode & Shadow

The image below will toggle dark/light mode based on theme preference, notice it has shadows.

![light mode only](/assets/images/avatar.jpg){: .light .w-75 .shadow .rounded-10 w='564' h='564' }
![dark mode only](/assets/images/avatar.jpg){: .dark .w-75 .shadow .rounded-10 w='564' h='564' }


## Footnote

Click the hook will locate the footnote[^footnote], and here is another footnote[^fn-nth-2].

## Inline code

This is an example of `Inline Code`.

## Filepath

Here is the `/path/to/the/file.extend`{: .filepath}.

## Code blocks

### Common

```text
This is a common code snippet, without syntax highlight and line number.
```

### Specific Language

```bash
if [ $? -ne 0 ]; then
  echo "The command was not successful.";
  #do the needful / exit
fi;
```

### Specific filename

```sass
@import
  "colors/light-typography",
  "colors/dark-typography";
```
{: file='_sass/jekyll-theme-chirpy.scss'}

## Mathematics

The mathematics powered by [**MathJax**](https://www.mathjax.org/):

$$
\begin{equation}
  \sum_{n=1}^\infty 1/n^2 = \frac{\pi^2}{6}
  \label{eq:series}
\end{equation}
$$

We can reference the equation as \eqref{eq:series}.

When $a \ne 0$, there are two solutions to $ax^2 + bx + c = 0$ and they are

$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$

## Mermaid SVG

```mermaid
 gantt
  title  Adding GANTT diagram functionality to mermaid
  apple :a, 2017-07-20, 1w
  banana :crit, b, 2017-07-23, 1d
  cherry :active, c, after b a, 1d
```

### Ordered list

1. Firstly
2. Secondly
3. Thirdly

### Unordered list

- Chapter
  - Section
    - Paragraph

### ToDo list

- [ ] Job
  - [x] Step 1
  - [x] Step 2
  - [ ] Step 3


## Tables

| Company                      | Contact          | Country |
| :--------------------------- | :--------------- | ------: |
| Alfreds Futterkiste          | Maria Anders     | Germany |
| Island Trading               | Helen Bennett    |      UK |
| Magazzini Alimentari Riuniti | Giovanni Rovelli |   Italy |

