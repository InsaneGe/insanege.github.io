---
title: How to write a new post
date: 2024-11-10 06:21:00 +0800 # 东八区（UTC/GMT+0800）是比世界协调时间（UTC）/格林尼治时间（GMT）快8小时的时区
categories: [tutorials]
tags: [tutorial]     # TAG names should always be lowercase
authors: [githubio]
description: "a simple demonstration to supported formats in a post"
comments: true
toc: true
pin: true
math: true
mermaid: true
image:
  path: /assets/images/anime.jpg
  alt: a photo embedded in the title
---

## Headings

<!-- markdownlint-capture -->
<!-- markdownlint-disable -->
# H1 — heading
{: .mt-4 .mb-0 }

## H2 — heading
{: data-toc-skip='' .mt-2 .mb-2 }

### H3 — heading
{: data-toc-skip='' .mt-3 .mb-4 }

#### H4 — heading
{: data-toc-skip='' .mt-4 .mb-6 }
<!-- markdownlint-restore -->

## Four kinds of prompts 

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

## Code blocks

### Inline code

This is an example of `Inline Code`.

### Common

```text
This is a common code snippet, without syntax highlight and line number.
```

### Specific Language

```bash
if [ $? -ne 0 ]; then
  echo "The command was not successful.";
  #exit
fi;
```

### Specific filename

```sass
@import 'addon/commons';
```
{: file='_sass/main.scss'}

### Jekyll Liquid Codes
{% raw %}
```liquid
{% if product.title contains 'Pack' %}
  This product's title contains the word Pack.
{% endif %}
```
{% endraw %}

### code blocks without line number
```c++
cout<<"hello world"<<endl;
```
{: .nolineno }


## Video 

### Bilibili

{% include embed/bilibili.html id='BV1Th411x7ii' title='【8K】来自宇宙深处的未知与震撼' %}

### Youtube(a VPN is required to load it successfully)

{% include embed/youtube.html id='GWGbOjlJDkU' title="Who are you?" start=240 %}

## Audio
{%
  include embed/audio.html
  src='assets/audio/sample-3s.mp3'
  title='audio demo'
%}

## Image

### Image with specific width and height

![](/assets/images/avatar.jpg){: width="250" height="250" }
_a caption for photo: killua_

### Left aligned image

<!-- .normal 起到的左对齐效果 -->
![](/assets/images/avatar.jpg){: width="150" height="150" .w-70 .h-70 .normal} text in the right

text below

### Float to left

![](/assets/images/avatar.jpg){: width="200" height="200" .w-70 .left}
ramdom text for showing the effect of float: Praesent maximus aliquam sapien. Sed vel neque in dolor pulvinar auctor. Maecenas pharetra, sem sit amet interdum posuere, tellus lacus eleifend magna, ac lobortis felis ipsum id sapien. Proin ornare rutrum metus, ac convallis diam volutpat sit amet. Phasellus volutpat, elit sit amet tincidunt mollis, felis mi scelerisque mauris, ut facilisis leo magna accumsan sapien. In rutrum vehicula nisl eget tempor. Nullam maximus ullamcorper libero non maximus. Integer ultricies velit id convallis varius. Praesent eu nisl eu urna finibus ultrices id nec ex. Mauris ac mattis quam. Fusce aliquam est nec sapien bibendum, vitae malesuada ligula condimentum.

### Dark/Light mode & Shadow

The image below will toggle dark/light mode based on theme preference, notice it has shadows.

<!-- .rounded-10 用于设置元素的圆角效果 -->
![light mode only](/assets/images/avatar.jpg){: .light .w-20 .shadow .rounded-10 w='200' h='200' }
![dark mode only](/assets/images/avatar.jpg){: .dark .w-20 .shadow .rounded-10 w='200' h='200' }

## Math powered by [**MathJax**](https://www.mathjax.org/)

### inline math
<!-- Inline math in lines, NO blank lines -->

both $LaTeX-math-expression$ and $$ LaTeX-math-expression $$" are fine.

<!-- Inline math in lists, escape the first `$` -->

1. \$$ LaTeX-math-expression $$
2. \$$ LaTeX-math-expression $$

### centered matrix and left aligned matrix

$$
\begin{pmatrix}
  1 & 2 & 3 \\
  4 & 5 & 6 \\
  7 & 8 & 9
\end{pmatrix}
\cdot
\begin{pmatrix}
  9 & 8 & 7 \\
  6 & 5 & 4 \\
  3 & 2 & 1
\end{pmatrix}
=
\begin{pmatrix}
  30 & 24 & 18 \\
  84 & 69 & 54 \\
  138 & 114 & 90
\end{pmatrix}
$$

<!-- left aligned matrix, escape the first `$` -->

\$$
\begin{bmatrix}
  1 & 2 & 3 \\
  4 & 5 & 6 \\
  7 & 8 & 9
\end{bmatrix}
$$

\$$
\begin{Bmatrix}
  1 & 2 & 3 \\
  4 & 5 & 6 \\
  7 & 8 & 9
\end{Bmatrix}
$$

### equation

$$
\begin{equation}
  \sum_{n=1}^\infty 1/n^2 = \frac{\pi^2}{6}
  \label{eq:series1}
\end{equation}
$$

$$
\begin{equation}
  \lim_{x \to 0} \frac{x}{\sin x}=1
  \label{eq:series2}
\end{equation}
$$

We can reference the equation as \eqref{eq:series1}.
We can reference the equation as \eqref{eq:series2}.


$$
\begin{cases}
  x + y = 5 \\
  x - y = 1
\end{cases}
$$

<!-- left aligned matrix, escape the first `$` and \ \quad is used to add a space -->

\$$
f(x)=\begin{cases}
  x \quad (x>0) \\
  0 \quad (x<=0)
\end{cases}
$$

\$$
f(x)=\begin{cases}
  x \ (x>0) \\
  0 \ (x<=0)
\end{cases}
$$


When $a \ne 0$, there are two solutions to $ax^2 + bx + c = 0$ and they are

$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$


## Graphs supported by [Mermaid](https://mermaid.js.org/intro/getting-started.html)

```mermaid
 gantt
  title  GANTT diagram of mermaid
  sleep :a, 2024-06-20, 8h
  sleep more :crit, b, after a, 12h
  sleep much more :active, c, after b a, 1d
```

```mermaid
xychart-beta
    title "Sales Revenue"
    x-axis [jan, feb, mar, apr, may, jun, jul, aug, sep, oct, nov, dec]
    y-axis "Revenue (in $)" 4000 --> 11000
    bar [5000, 6000, 7500, 8200, 9500, 10500, 11000, 10200, 9200, 8500, 7000, 6000]
    line [5000, 6000, 7500, 8200, 9500, 10500, 11000, 10200, 9200, 8500, 7000, 6000]
```

```mermaid
sequenceDiagram
    participant 客户
    participant 服务器
    客户->>服务器: 发送请求
    服务器-->>客户: 返回响应
    客户->>服务器: 请求数据
    服务器-->>客户: 发送数据
```

## Lists

### Ordered list

1. Firstly
2. Secondly
3. Thirdly

### Unordered list

- Chapter
  - Page
    - Paragraph

### ToDo list

- [ ] Job
  - [x] Step 1

### Description list

Sun
: the star around which the earth orbits

## Quote and bold and italic

> This line shows the __block quote__ and _block quote_.

## Filepath

Here is the `/path/to/the/file.extend`{: .filepath}.

## Links

[B站](https://www.bilibili.com)

<https://www.bilibili.com>

## Tables

| Company                      | Contact          | Country |
| :--------------------------- | :--------------- | ------: |
| Alfreds Futterkiste          | Maria Anders     | Germany |
| Island Trading               | Helen Bennett    |      UK |

## Footnote

Click the hook will locate the footnote[^footnote], and here is another footnote[^fn-nth-2].

## other formats
Any other format supported by markdown is also supported.

<br>
<br>
<br>

[^footnote]: The footnote source
[^fn-nth-2]: The 2nd footnote source


