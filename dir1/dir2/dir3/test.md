How does a relative reference work from here?

It seems we can use root relative syntax:

![image 1](/images/img1/image1.png)
![image 2](/images/img2/image2.png)

Does relative syntax also work?

![image 1](../../../images/img1/image1.png)
![image 2](../../../images/img2/image2.png)


What does GitHub do when we are relative above git root? It does not block it.

![testing absolute](https://github.com/lread/rewrite-cljc-playground/raw/master/doc/rewrite-cljc-logo.svg)

![testing relative](../../../../../../rewrite-cljc-playground/raw/master/doc/rewrite-cljc-logo.svg)

