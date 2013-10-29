--- 
layout: post 
name: terminaliniz-renklensin 
title: Terminaliniz renklensin 
time: 2012-10-16 17:43:00.000000000 +01:00
description: " "
category: articles
tags: [mac]
author: htss
---

Mac kullanıcılarının terminal üzerinden çalışmaları sırasında eksikliğini hissettiğinden emin olduğum bir şey var; renkler! Özellikle de Linux deneyimi olan kullanıcılar klasör ve diğer dosyaların özelliklerine göre farklı renklerde listelenmesinin getirdiği kolaylığı mutlaka arıyorlardır.
Neyse ki devasız bir dert değil. Yapmanız gereken `~/.cshrc` dosyanıza birkaç eklemeden ibaret:

[![]({{site.url}}/images/terminal.png)]({{site.url}}/images/terminal.png)


{% highlight bash %}
setenv CLICOLOR 1
setenv LSCOLORS ExexcxdxbxegedbxbxExEx 
{% endhighlight %}


**bash** kullanıcılarının `.bashrc` dosyasına yukardaki satırları `setenv` yerine `export=` olarak yazması yeterli olacaktır.

LSCOLORS'ı takip eden renk kodları neyin ne renkle gösterileceğini belirliyor. Ama hepsi bu kadar değil. Renkleri kendi zevkinize ve/veya alışkanlıklarınıza göre düzenlemek isterseniz; dilediğiniz dosya türünün dilediğiniz fon ve renkte görünmesini ayarlayıp, hatta önizlemesine de bakabileceğiniz şu adrese mutlaka uğramalısınız: [http://geoff.greer.fm/lscolors/](http://geoff.greer.fm/lscolors/)

Rengarenk ve keyifli çalışmalar dileğiyle!
