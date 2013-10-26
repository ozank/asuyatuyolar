--- 
layout: post 
name: latexde-turkce-karakter-kodlar 
title: LaTeX'de Türkçe Karakter Kodları 
time: 2011-05-02 14:36:00.000000000 +01:00
description: "ö,ş,ğ yazarken sorn mu çıkıyor?"
category: articles
tags: [latex]
author: htss
---

Her ne kadar LaTeX kullanımı Türkiye'de yeterince yaygın olmadığı için LaTeX'i çoğunlukla yabancı dillerdeki metinler için kullansak da, Türkçe karakter sorunuyla karşılaşmayacağımız anlamına gelmiyor bu. Sonuçta nereye gidersek gidelim adlarımızdaki Türkçe karakterler de bizimle birlikte geliyor ve çoğunlukla onlardan vazgeçmek istemiyoruz.

LaTeX ile binlerce çeşit aksan ve sembolü oluşturmak mümkün ama gene de Türkçe karakterleri oluşturmak karmaşık bir iş olabilir çünkü bir kere o nüansları aramaya başladınız mı tahmin ettiğinizden fazla imla işareti ile karşı karşıya kalabilirsiniz. Keza ben uzunca bir süre `ğ` harfinin tepesindeki çizgiyi farklı bir aksan çizgisiyle karıştırmış ve `\~` işaretini kullanmıştım. Doğru Türkçe karakterleri oluşturmak için kullanmanız gereken kodlar ise şu şekilde:

![]({{site.url}}/images/Screenshot2011-05-02.png)

Bu kodlarla uğraşmak istemezseniz, yazdığınız Türkçe metni LaTeX'e dönüştüren pratik bir site mevcut [bu adreste](http://turkishtolatex.appspot.com/).

Tabii oluşturduğunuz metin tamamen Türkçe de olabilir. Bu durumda her Türkçe karakteri tek tek bu şekilde girmeniz pek de pratik olmayacaktır ki zaten Türkçe dil kodlamasını halleden bazı temel paketler var. LaTeX'in kendiliğinden ürettiği Kaynaklar, İçindekiler gibi başlıklar için `\documentclass` komutunun ardından `\usepackage[turkish]{babel}` komutunu eklemelisiniz. Türkçe harfler için kullanmanız gereken paketin komutu da şöyle: `\\usepackage[utf8]{inputenc}`. Eğer metin içinde heceleme yapmak istiyorsanız bunun da Türkçe'ye uygun olması için `\usepackage[T1]{fontenc}` komutunu girmenizde fayda var. Bu üç temel komut, Türkçe metin desteği için yeterli olacaktır. Aşağıda test için kullanabileceğiniz basit bir doküman var:

{% highlight tex %}
\documentclass{report}
\usepackage[turkish]{babel} %Türkçe bölüm isimleri
\usepackage[utf8]{inputenc} %Türkçe karakterler
\usepackage[T1]{fontenc} %Türkçe heceleme
  
\title{Belge İsmi - A B C Ç D E F G Ğ H I İ J K L M N O Ö P R S Ş T U Ü V Y Z}
\author{Yazar Adı - a b c ç d e f g ğ h ı i j k l m n o ö p r s ş t u ü v y z}

\begin{document}

\maketitle

\end{document}
{% endhighlight %}


Ayrıca bunlar gibi birçok pratik LaTeX bilgisi içeren "İnce bir LATEX 2ε Elkitabı"na da [bu adresten](http://akgul.bilkent.edu.tr/Yunus/lshort.pdf) ulaşabilirsiniz.
Türkçe karakterlerin yanısıra LaTeX'te kullanmak isteyeceğiniz başka birçok sembol ve biçimlendirme için pratik bir başvuru kağıdına (önlü arkalı bir A4 sayfası ancak bu kadar işe yarar olabilir sanırım) [bu adresten](http://www.google.co.uk/url?sa=t&source=web&cd=2&ved=0CCMQFjAB&url=http%3A%2F%2Fwww.tex.ac.uk%2Ftex-archive%2Finfo%2Flatexcheat%2Flatexcheat%2Flatexsheet.pdf&ei=r6a-TeXHDoXA8QPM0PDHBQ&usg=AFQjCNHu3mMsx_KPa861fTeGbjH1_9U45A) erişebilirsiniz.

Ben denk gelmedim ama bu kodlara rağmen İÇİNDEKİLER yerine ICINDEKILER yazıyorsa: dokümana,

{% highlight tex %}
\uccode `\i='235
\lccode `\I='031
{% endhighlight %}

kodlarını ekleyince hiçbir sorun kalmıyormuş.
