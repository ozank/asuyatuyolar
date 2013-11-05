---
layout: post
title: Yeniden Merhaba
description: "Yeni tasarım ve durum güncellemesi"
modified: 2013-11-04-21-00
category: articles
---

Uzun bir aradan sonra tekrar merhaba! Yaklaşık 6 aydır yeni yazı yazamadım ama mazeretim büyük: [tezimle](http://dl.dropboxusercontent.com/u/2490601/Ozan_Thesis.pdf) boğuşuyordum. Artık rahatladım sayılır ve tekrar Asuya Tüyolar'la yeniden ilgilenmeye başlayabilirim.

## Yeni Tasarım

Ne zamandır blogu Blogger ve Google'dan kurtarmak istiyordum ancak kafama göre de birşey bulamamıştım. Geçenlerde [Github](http://github.com)`ın web sitelerini yayınlamak için [Github Pages](http://pages.github.com/) servisini başlattığını görünce aklım çelindi. Böylece blogu ücretsiz, reklamsız ve açık kaynak olarak yayınlamak mümkün oldu. 

## Açık Kaynak

Benim en çok hoşuma giden özelliği, sitenin herşeyinin açık kaynak olarak paylaşabilmesiydi. Mesela, bu sitenin yazılarına açık kaynak olarak aşağıdaki adresten ulaşabilirsiniz.

- [Asu'ya Tüyolar Kaynak Kodu](https://github.com/ozank/asuyatuyolar/tree/gh-pages/_posts)

Eğer yeni yazı eklemek ya da mevcut yazılara eklemeler yapmak isterseniz, tek yapmanız gereken GitHub'daki kodlar üstünde değişiklik yapmak, detaylar için [hakkında]({{site.url}}/about) sayfasına göz atabilirsiniz.

## Markdown

Blogger'ın yıllardır geliştirilmeyen arayüzü ile yazmak bazen gerçekten eziyete dönüşüyordu. Şu anda site arka planda [Jeykll](http://jekyllrb.com/) ve [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) kullanıyor. Böylece blog yazılarını artık düz metin dosyası olarak hazırlayacağım (Markdown hakkında önceden [şu yazımızda]({{site.url}}/2012/06/pandoc-ile-metin-dosyalarn-donusturmek.html) bahsetmiştik). 

Markdown ile içerik ve tasarımı tamanen ayırabiliyorsunuz (tıpkı LaTeX gibi), ayrıca internet yokken metin dosyası üstünde yazımı hazırlayıp Github'a yayınlamak üzere gönderebileceğim.

Markdown'ın işimi kolaylaştıran birçok özelliği daha var:

### Denklemler

Markdown ve [MathJax](http://www.mathjax.org/) kullanarak doğrudan LaTeX denklemlerini yazının içine gömebiliyorum. 
Mesela: satır içi denklemler $$ \oint_C {E \cdot d\ell } = - \frac{d}{dt} \int_S {B_n dA}$$  ya da uzun denklemler:


$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

### Kodlar

Artık programlama üstüne daha çok yazmak istiyorum. Yeni site [Pygments](http://pygments.org/) destekliyor. Tüm dillere [su adresden](http://pygments.org/languages/)  ve 
farklı renk kodlarına [Pygments demolar](http://pygments.org/demo/) kısmından ulaşabilirsiniz. Birkaç örnek:

#### LaTeX

{% highlight tex %}
\documentclass[12pt]{article}

\title{This is the title}
\author{Author One \\ Author Two}
\date{29 February 2004}

\begin{document}
\maketitle
This is the content of this document.
\end{document} 
{% endhighlight %}


#### Python

{% highlight python linenos %}
from __properties__ import WithProperties

class Test(WithProperties):

    def __init__(self):
        self._test = 3

    def get_test(self):
        print 'Getting test'
        return self._test
{% endhighlight %}

#### Matlab

{% highlight matlab %}
m = zeros(2, 3)   % Creates a 2x3 matrix of zeros
v = ones(1, 3)    % Creates a 1x3 matrix (row vector) of ones
m = eye(3)        % Identity matrix (3x3)
{% endhighlight %}
