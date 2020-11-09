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
