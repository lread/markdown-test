# markdown-test

## Image Refs
Testing what type of image references GitHub supports

We know that relative from root works:


![image 1](images/img1/image1.png)


![image 2](images/img2/image2.png)

How do relative images behave from deeper?

[markdown](dir1/dir2/dir3/test.md)

[asciidoc](dir1/dir2/dir3/test.adoc)

## Quoted text

> Quoted text.
>
> Another paragraph in quote.

## Emojis

:adhesive_bandage:
:hatched_chick:
:pushpin:

## Svg Contrib Image Test

![svg image](/images/contrib.svg)
![svg image](/images/contrib.svg)

## details summary dropdowns
An empty line before the code block seems necessary.

<details><summary>Markdown</summary>

```markdown
[![bb compatible](https://raw.githubusercontent.com/babashka/babashka/master/logo/badge.svg)](https://babashka.org)
```
</details>

<details><summary>AsciiDoc</summary>

```asciidoc
https://babashka.org[image:https://raw.githubusercontent.com/babashka/babashka/master/logo/badge.svg[bb compatible]]
```
</details>

<details><summary>HTML</summary>

```html
<a href="https://babashka.org" rel="nofollow"><img src="https://github.com/babashka/babashka/raw/master/logo/badge.svg" alt="bb compatible" style="max-width: 100%;"></a>
```
</details>

## Stem?
https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions

$`\sqrt{3x-1}+(1+x)^2`$


<br/>

## Dashes

Two --

Three ---

## Emojis

`:people_holding_hands:` :people_holding_hands:

`:kneeling_man:` :kneeling_man:

`:atom:` :atom:

`:nope:` :nope:
