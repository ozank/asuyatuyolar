--- layout: post name: latexte-bolum-isimlerini title: LaTeX'te bölüm isimlerini Türkçeleştirmek time: 2011-07-14 22:37:00.000000000 +01:00 --- Daha önceki, [LaTeX'de Türkçe karakterlerle ilgili bir yazı](http://asuyatuyolar.blogspot.com/2011/05/latexde-turkce-karakter-kodlar.html) paylaşmıştık. Bu sefer de İsmail, LaTeX'de bölüm isimlerini dönüştürmekle ilgili faydalı bir yazı yazmış. Buyrun:

[![](http://2.bp.blogspot.com/-yCafCpW9pOM/TZiwLru_M3I/AAAAAAAAA3U/deiqc4-I78Q/s200/latex_logo.jpg)](http://2.bp.blogspot.com/-yCafCpW9pOM/TZiwLru_M3I/AAAAAAAAA3U/deiqc4-I78Q/s1600/latex_logo.jpg)

LaTeX'te Türkçe bir belge hazırlıyorsunuz. Her seferinde Türkçe'deki ş,ğ,ı gibi karakterlerin karşılıklarını uzun uzun yazmaya üşendiniz. Bunun için dosyanın karakter kodlamasını **utf8** yaptınız ve **inputenc**paketini şu şekilde yüklediniz:

`\usepackage``[utf8x]{inputenc}`

Her şey güzel derken bir baktınız ki bazı kısımlar hâlâ İngilizce. Örneğin `\begin{abstract}` ile özetçe eklediniz veya `\tableofcontents` ile içindekiler bölümü eklediniz ve baktınız ki *Özetçe* yerine *Abstract* yazıyor, *İçindekiler* yerine *Contents* yazıyor. Yani, isimlendirmeler Türkçe değil. Bu yazıda bu isimlendirmeleri değiştirmeyi ele alalım. Aslında bu yöntemi Türkçe karşılığı yerine başka bir İngilizce kelime kullanmak için de kullanabilirsiniz.
LaTeX'te bu biçimdeki isimlendirmeler genelde şöyle yazılıyor:

`\renewcommand``*``\XXXname``{XXX iç``in` `yeni isim}`

Burada XXX diye yazdığım kısım *özetçe*, *bölüm*, *bakınız*, *kaynakça* gibi birçok anahtar sözcüğe tekabül edebilir. Kullandığınız belge sınıfına göre, bazıları tanımlı olurken bir kısmı tanımlı olmayacaktır. Örneğin, `\documentclass{article}` ile belge sınıfını makale olarak belirlediyseniz, makalelerde `chapter` komutu kullanılmadığı için `\renewcommand*\chaptername{Bölüm}` satırı hata verecektir.
Altta ihtiyaç duyulabilecek çoğu isimlendirmeyi ekledim. Yanlarında da nerelerde kullanılabileceği ile ilgili yorum mevcut. Belgenin sınıfına göre gerekli olanlar kullanılabilir. İsimlendirmelerin Türkçelerini ben yazdım, yanlışlıklar olabilir, çevirisinin farklı olacağını düşünüyorsanız lütfen ona göre değiştirin.

> \\renewcommand\*\\abstractname{Özetçe}
> \\renewcommand\*\\alsoname{ayrıca bkz.} % makeidx ile
> \\renewcommand\*\\appendixname{Ek}
> \\renewcommand\*\\bibname{Kaynakça} % 'report' ile
> \\renewcommand\*\\chaptername{Bölüm} % 'report' ve 'book' için
> \\renewcommand\*\\contentsname{İçindekiler}
> \\renewcommand\*\\figurename{Şekil}
> \\renewcommand\*\\indexname{Dizin} % makeidx ile
> \\renewcommand\*\\listfigurename{Şekil Listesi}
> \\renewcommand\*\\listtablename{Tablo Listesi}
> \\renewcommand\*\\pagename{Sayfa} % 'letter' ile
> \\renewcommand\*\\partname{Kesim}
> \\renewcommand\*\\refname{Kaynakça} % 'article' ile
> \\renewcommand\*\\seename{bkz.} % 'makeidx' ile
> \\renewcommand\*\\tablename{Tablo}

Bunlar dışında kullandığınız pakete göre bazı isimlendirmeler olabilir. Bunun için ilgili paketin dokümantasyonuna başvurmak iyi olacaktır.
*Bu yazının orjinaline İsmail Arı'nın bloğunda, [şu adresden](http://ismailari.com/blog/latexte-ozetce-bolum-icindekiler-vb-isimlendirmelerini-degistirmek/) ulaşabilir, teşekkürlerinizi kendisine iletebilirsiniz.*
