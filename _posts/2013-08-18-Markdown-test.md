---
layout: post
title: Markdown Deneme
description: "Markdown'in yetenekleri"
modified: 2013-08-18-31
category: articles
tags: [markdown]
---

## Denklemler

Satir ici denklemler $$ x^2+y= \int z $$


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

#Kodlar

[Pygments](http://pygments.org/) destekliyor. Tum dillere [su adresden](http://pygments.org/languages/) ulasabilirsiniz.
Isterseniz farkli renk kodlarina [Pygments demolar](http://pygments.org/demo/) kismindan ulasabilirsiniz.

### LaTeX

{% highlight tex %}
\documentclass[12pt]{article}
%	options include 12pt or 11pt or 10pt
%	classes include article, report, book, letter, thesis

\title{This is the title}
\author{Author One \\ Author Two}
\date{29 February 2004}

\begin{document}
\maketitle

This is the content of this document.

This is the 2nd paragraph.
Here is an inline formula:
$   V = \frac{4 \pi r^3}{3}  $.
And appearing immediately below
is a displayed formula:
$$  V = \frac{4 \pi r^3}{3}  $$
\end{document} 
{% endhighlight %}

### CSS

{% highlight css %}
#container {
  float: left;
  margin: 0 -240px 0 0;
  width: 100%;
}
{% endhighlight %}

### Python
{% highlight python linenos %}
from __properties__ import WithProperties

class Test(WithProperties):

    def __init__(self):
        self._test = 3

    def get_test(self):
        print 'Getting test'
        return self._test

    def set_test(self, value):
        print 'Setting test'
        self._test = value
{% endhighlight %}

### R
{% highlight r %}
Get_conduction<-function(A,l,Tmin,Nsection){
  Tamb<-298
  Tpoints<-seq(Tmin,Tamb, l=Nsection)
  kpoints<-Get_thermal_conductivity(Tpoints[-1])
  #xpoints<-l/(sum(1/kpoints)*kpoints)
  xpoints<-l*kpoints/sum(kpoints)
  #conduction<-Get_thermal_conductivity(Tav)*A*Tdiff/l
  conduction<-mean(kpoints*A*diff(Tpoints)/xpoints)
}
{% endhighlight %}

### Matlab

{% highlight matlab %}

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% (B) Creating special matrices: 1ST parameter is ROWS,
%   2ND parameter is COLS 

m = zeros(2, 3)              % Creates a 2x3 matrix of zeros
v = ones(1, 3)               % Creates a 1x3 matrix (row vector) of ones
m = eye(3)                   % Identity matrix (3x3)
v = rand(3, 1)               % Randomly filled 3x1 matrix (column 
                             % vector); see also randn

                             % But watch out:
m = zeros(3)                 % Creates a 3x3 matrix (!) of zeros
{% endhighlight %}
