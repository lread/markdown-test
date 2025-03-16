How does a relative reference work from here?

It seems we can use root relative syntax:

![image 1](/images/img1/image1.png)
![image 2](/images/img2/image2.png)

Does relative syntax also work?

![image 1](../../../images/img1/image1.png)
![image 2](../../../images/img2/image2.png)
 
 
Let's try a data uri (looks like a nogo for github)

![Hello World](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEYAAAAUCAAAAAAVAxSkAAABrUlEQVQ4y+3TPUvDQBgH8OdDOGa+oUMgk2MpdHIIgpSUiqC0OKirgxYX8QVFRQRpBRF8KShqLbgIYkUEteCgFVuqUEVxEIkvJFhae3m8S2KbSkcFBw9yHP88+eXucgH8kQZ/jSm4VDaIy9RKCpKac9NKgU4uEJNwhHhK3qvPBVO8rxRWmFXPF+NSM1KVMbwriAMwhDgVcrxeMZm85GR0PhvGJAAmyozJsbsxgNEir4iEjIK0SYqGd8sOR3rJAGN2BCEkOxhxMhpd8Mk0CXtZacxi1hr20mI/rzgnxayoidevcGuHXTC/q6QuYSMt1jC+gBIiMg12v2vb5NlklChiWnhmFZpwvxDGzuUzV8kOg+N8UUvNBp64vy9q3UN7gDXhwWLY2nMC3zRDibfsY7wjEkY79CdMZhrxSqqzxf4ZRPXwzWJirMicDa5KwiPeARygHXKNMQHEy3rMopDR20XNZGbJzUtrwDC/KshlLDWyqdmhxZzCsdYmf2fWZPoxCEDyfIvdtNQH0PRkH6Q51g8rFO3Qzxh2LbItcDCOpmuOsV7ntNaERe3v/lP/zO8yn4N+yNPrekmPAAAAAElFTkSuQmCC)

What about via html?

<img src="data:image/gif;base64,R0lGODlhAQABAIAAAAUEBAAAACwAAAAAAQABAAACAkQBADs=" alt="hello"/>

What does GitHub do when we are relative above git root? It does not block it.

![testing absolute](https://github.com/lread/rewrite-cljc-playground/raw/master/doc/rewrite-cljc-logo.svg)

![testing relative](../../../../../../rewrite-cljc-playground/raw/master/doc/rewrite-cljc-logo.svg)

Ok let's try any html, just to see that work:

<b>bold statement</b>

Let's try some embedded html samples. Can embedded html contain markup?
**am I bold?**

<table>
 <tr>
  <td>
**am I bold?**
  </td>
 </tr>
</table>

Check on various language strings for Clojure:

Clojure
```Clojure
(+ 1 2 3)
```

CLJ (checking if caps ok)
```CLJ
(+ 1 2 3)
```

cljs
```cljs
(+ 1 2 3)
```

cljc
```cljc
(+ 1 2 3)
```

ClojureScript is not recognized as Clojure
```ClojureScript
(+ 1 2 3)
```

Can I emded a definition list?
<dl>
  <dt>Lower cost</dt>
  <dd>The new version of this product costs significantly less than the previous one!</dd>
  <dt>Easier to use</dt>
  <dd>We've changed the product so that it's much easier to use!</dd>
</dl>




What about kdb in md?:
<p>Please press <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>R</kbd> to re-render an MDN page.</p>


Are spaces stripped in inline code? `testing             one           two`

How does a list of code blocks look?

- ```clojure
  hello I'm a code block
       ^
  ```
- ```clojure
  I'm another code block
               ^
  ```
  
bb badges
[![bb compatible](https://raw.githubusercontent.com/babashka/babashka/master/logo/badge.svg)](https://book.babashka.org#badges)
[![bb built-in](https://raw.githubusercontent.com/babashka/babashka/master/logo/built-in-badge.svg)](https://book.babashka.org#badges)
  
