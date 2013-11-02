--- 
layout: post 
name: kindle-ile-pdf-okumak 
title: Kindle ile PDF okumak 
time: 2011-10-06 18:45:00.000000000 +01:00
category: articles
tags: [akademik, doküman, pdf, kindle, populer]
--- 

Yakın zamanda e-kitap furyasına ben de katıldım. İlk başlarda açık kodlu `epub` formatını desteklemediği için Amazon Kindle'a soğuk bakıyordum. Ancak daha sonra uygun fiyata bir ikinci el bulunca almaya karar verdim. Gerçi neden uygun olduğunu da birkaç hafta sonra Amazon [yeni Kindle](http://www.amazon.co.uk/Kindle-Wi-Fi-6-Ink-Display/dp/B0051QVF7A/ref=amb_link_161260467_1?pf_rd_m=A3P5ROKL5A1OLE&pf_rd_s=gateway-center-column&pf_rd_r=1NS4A3HJAGFFNEHBQ703&pf_rd_t=101&pf_rd_p=255057967&pf_rd_i=468294)'ı çıkarınca anladım ya neyse.

İsmail [şu yazısında](http://ismailari.com/blog/kindle-3-degerlendirmesi-ve-idefixten-kindlea-donusum/) Kindle ile ilgili çok güzel bir değerlendirme yazısı yazmış. Eğer Kindle almayı düşünüyorsanız bir göz atın. Bu yazıda Kindle ile PDF okuma işleriyle ilgili birkaç ipucu paylaşacağım.

[![]({{site.url}}/images/kindle_kitap.jpg)]({{site.url}}/images/kindle_kitap.jpg)

 
Kindle olsun olmasın tüm e-kitap okuyucular için en kullanışlı program: [Calibre](http://calibre-ebook.com/). Calibre açık kodlu ve ücretsiz. Zaten [Calibre](http://calibre-ebook.com/) sayesinde Amazon'un kendi programını bile kurmadan idare ediyorum. Calibre'nin en büyük avantajı onlarca dosya arasında pratik bir şekilde dönüşüm yapabilmesi, ki bunlar arasında `epub`, `pdf`, `mobi`, `html`, `txt`, `rtf` var. Daha birçok güzel özelliği var ama onları da sonraki yazılara bırakalım.

[![]({{site.url}}/images/calibre.jpg) ]({{site.url}}/images/calibre.jpg)

Nerdeyse tüm e-okuyucular pdf dosyalarını doğrudan açabiliyor, ancak tabi `pdf` üstünden okuması e-kitaplar kadar rahat olmuyor. Mesela, sayfayı yakınlaştırdığınızda satırları ekrana sığacak şekilde yeniden dizemiyor ya da pdf resim şeklinde oluşturulduysa altını çizemiyorsunuz, sözlükten kelimelere bakamıyorsunuz vs.

Calibre sayesinde pdf dosyalarını kindle formatına(mobi) dönüştürebiliyorsunuz. Hele bir de önce epub'a dönüştürüp sonra mobi'ye dönüştürürseniz baya güzel sonuçlar alıyorsunuz.  Ancak, Türkçe karakterlerde genelde sorun çıkıyor. Ya da pdf dosyası düzgün oluşturulmadıysa veya sayfalar çift sütunsa sonuç malesef hüsran. Üstelik çift sütunlu pdf'leri doğrudan pdf olarak açsanız, bu sefer de vaktinizin çoğu görüntüyü ayarlamakla geçiyor. Malesef bizim alandaki çoğu dergiler de (mesela IEEE makaleleri) çift sütun formatında.

Çift sütun PDF'leri tek sütuna dönüştürüp, gereksiz boşlukları kolayca kırpabileceğiniz açık kodlu ve küçük bir program var: [Briss](http://sourceforge.net/projects/briss/). Mesela bir IEEE makalesini Kindle'a uygun hale nasıl geldiğine bakalım. [Briss](http://sourceforge.net/projects/briss/)'i açtığınızda tüm sayfalardaki yazıları üstüste bindirilmiş şekilde göstererek, PDF'yi nerelerden kesebileceğinize karar verebiliyorsunuz
.

[![]({{site.url}}/images/briss2.png)]({{site.url}}/images/briss2.png)

Mavi dikdörtgenleri ayarlayarak kesilecek yerleri  ayarlayın ya da ikinci bir dikdörtgen oluşturarak dosyayı tek sütuna dönüştürün. Kırpma işleminin dışında tutmak istediğiniz sayfaları da belirtebiliyorsunuz. Sonuç aşağıdaki gibi gayet başarılı.

[![]({{site.url}}/images/tek_sutun.png)]({{site.url}}/images/tek_sutun.png)

Bu değiştirilmiş dosyayı da Calibre ile Kindle'a attığınızda ister yan ister düz çok rahat okuyabilirsiniz. Sayfa sayfa geçme tuşlarıyla da makale içinde kolayca gezinebilirsiniz.

[![]({{site.url}}/images/kindle_dikey.JPG) ]({{site.url}}/images/kindle_dikey.JPG) 

[![]({{site.url}}/images/kindle_yatay.JPG)]({{site.url}}/images/kindle_yatay.JPG)

Gerçi çoğu makaleyi hala [Mendeley](http://asuyatuyolar.org/2009/12/mendeley-akademik-pdf-ve-referans.html) üstünden, bilgisayar karşısında okuyorum. Önceden çıktısını alıp kenarına notlar aldığım makaleleri bu yöntemle artık Kindle'da okuyorum. Daha sonra altını çizdiğim yerleri ve aldığım notları Calibre ile açıp da [Mendeley](http://asuyatuyolar.org/2009/12/mendeley-akademik-pdf-ve-referans.html)'deki notlar kısmına kopyalıyorum.
Bilmiyorum kaç kişinin ilgisini çeken bir yazı oldu da Kindle yazılarının devamı gelebilir...


**Faydalı Linkler:**

-   [Kindle için Faydalı Bilgiler:](http://kindlebilgideposu.wordpress.com/) Kindle ve e-kitap okuyucularıyla ilgili birçok güzel yazının bulunduğu Türkçe bir kaynak.
-   [The big list of free Kindle tools:](http://www.freewaregenius.com/2011/08/28/the-big-list-of-free-kindle-tools/) Kindle araçları(İngilizce).

**Detaylı okuma listesi:**

- [How to: Amazon’s Kindle 3 for Academics and Students ](http://commonsenseatheism.com/?p=11706)
- [Dear Jane: What Is the Best Way to Read PDFs on a 6 Inch Screen ](http://dearauthor.com/ebooks/dear-jane-ebooks/dear-jane-what-is-the-best-way-to-read-pdfs-on-a-6-inch-screen/)
- [Optimize PDF's for Kindle ](http://www.freewaregenius.com/2011/03/24/optimize-pdfs-for-reading-on-your-kindle-3-crop-then-convert-to-a-kindle-friendly-format/)
