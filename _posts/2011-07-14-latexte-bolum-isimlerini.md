--- 
layout: post 
name: latexte-bolum-isimlerini 
title: LaTeX'te bölüm isimlerini Türkçeleştirmek 
time: 2011-07-14 22:37:00.000000000 +01:00
description: "Abstract yerine: Özetçe"
category: articles
tags: [latex]
author: ismail
--- 

LaTeX'te Türkçe bir belge hazırlıyorsunuz. Her seferinde Türkçe'deki ş,ğ,ı gibi karakterlerin karşılıklarını uzun uzun yazmaya üşendiniz. Bunun için dosyanın karakter kodlamasını `utf8` yaptınız ve `inputenc` paketini şu şekilde yüklediniz:

{% highlight tex %}
\usepackage[utf8x]{inputenc}
{% endhighlight %}

Her şey güzel derken bir baktınız ki bazı kısımlar hâlâ İngilizce. Örneğin `\begin{abstract}` ile özetçe eklediniz veya `\tableofcontents` ile içindekiler bölümü eklediniz ve baktınız ki *Özetçe* yerine *Abstract* yazıyor, *İçindekiler* yerine *Contents* yazıyor. 

Yani, isimlendirmeler Türkçe değil. Bu yazıda bu isimlendirmeleri değiştirmeyi ele alalım. Aslında bu yöntemi Türkçe karşılığı yerine başka bir İngilizce kelime kullanmak için de kullanabilirsiniz.
LaTeX'te bu biçimdeki isimlendirmeler genelde şöyle yazılıyor:

{% highlight tex %}
\renewcommand*\XXXname{XXX için yeni isim}
{% endhighlight %}

Burada XXX diye yazdığım kısım *özetçe*, *bölüm*, *bakınız*, *kaynakça* gibi birçok anahtar sözcüğe tekabül edebilir. Kullandığınız belge sınıfına göre, bazıları tanımlı olurken bir kısmı tanımlı olmayacaktır. 

Örneğin, `\documentclass{article}` ile belge sınıfını makale olarak belirlediyseniz, makalelerde `chapter` komutu kullanılmadığı için `\renewcommand*\chaptername{Bölüm}` satırı hata verecektir.

Altta ihtiyaç duyulabilecek çoğu isimlendirmeyi ekledim. Yanlarında da nerelerde kullanılabileceği ile ilgili yorum mevcut. Belgenin sınıfına göre gerekli olanlar kullanılabilir. İsimlendirmelerin Türkçelerini ben yazdım, yanlışlıklar olabilir, çevirisinin farklı olacağını düşünüyorsanız lütfen ona göre değiştirin.

{% highlight tex %}
\renewcommand*\abstractname{Özetçe}
\renewcommand*\alsoname{ayrıca bkz.} % makeidx ile
\renewcommand*\appendixname{Ek}
\renewcommand*\bibname{Kaynakça} % 'report' ile
\renewcommand*\chaptername{Bölüm} % 'report' ve 'book' için
\renewcommand*\contentsname{İçindekiler}
\renewcommand*\figurename{Şekil}
\renewcommand*\indexname{Dizin} % makeidx ile
\renewcommand*\listfigurename{Şekil Listesi}
\renewcommand*\listtablename{Tablo Listesi}
\renewcommand*\pagename{Sayfa} % 'letter' ile
\renewcommand*\partname{Kesim}
\renewcommand*\refname{Kaynakça} % 'article' ile
\renewcommand*\seename{bkz.} % 'makeidx' ile
\renewcommand*\tablename{Tablo}
{% endhighlight %}

Bunlar dışında kullandığınız pakete göre bazı isimlendirmeler olabilir. Bunun için ilgili paketin dokümantasyonuna başvurmak iyi olacaktır.

*Bu yazının orjinaline İsmail Arı'nın bloğunda, [şu adresden](http://ismailari.com/blog/latexte-ozetce-bolum-icindekiler-vb-isimlendirmelerini-degistirmek/) ulaşabilir, teşekkürlerinizi kendisine iletebilirsiniz.*
