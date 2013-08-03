--- layout: post name: excel-kullanmadan-hzl-grafik-hazrlama-r title: ! '(Excel Kullanmadan) Hızlı Grafik Hazırlama : R' time: 2012-06-11 23:46:00.000000000 +01:00 ---
Excel kullanarak hızlıca grafik hazırlanabileceğini düşünüyorsanız, malesef yanılıyorsunuz. Hızlıdan kastım yarına yetişecek rapor için 5 dakikada bir grafik hazırlamak değil. Evet, belki de bu işler için en uygunu Excel. Ancak işiniz dolasıyla sürekli grafik hazırlıyorsanız, ya da önünüzde yapılacak bir yüksek lisans/doktora tezi varsa, ya da büyük veri setleriyle uğraşmak durumundaysanız Excel sadece günü kurtarır, uzun vadede süründürür.

> *Excel günü kurtarır, uzun vadede süründürür.*

[![](http://3.bp.blogspot.com/-uGDvkhXQb4Y/T9Z2MOAnLFI/AAAAAAAABkc/xanx44xLgbQ/s200/rstudio.png)](http://www.r-project.org/)

Eğer yarına yetiştirelecek bir raporunuz yoksa  gelin [R](http://www.r-project.org/) öğrenin, kullanması sandığınızdan daha kolay.
Aslında [R](http://www.r-project.org/)'ı bir grafik hazırlama programına indirgemek büyük haksızlık olur, her ne kadar ilk zamanlarda istatistikçiler arasında revaçta olsa da bugün yüzlerce eklentisiyle hemen her alanda uygulama alanı buluyor.
İnternette mevcut tonlarca veri sadece parmaklarınızın ucundayken R (ya da benzeri bir program) bilmek bence oldukça değerli.
R'ın sevdiğim özellikleri:

-   Açık kaynak kodlu, bedava.
-   Windows, Linux, Mac hepsinde çalışır.
-   İnternette örnek kodlar bolca mevcut.
-   Eklentileriyle neredeyse istediğiniz her işi yapabilirsiniz.
-   Büyük datalarla kolayca başedebilirsiniz (Paralel-computing desteği de var).
-   Datalara doğrudan internetten ulaşabilir ya da kendi datalarınızı paylaşabilirsiniz (bakınız: [OpenAccess](http://en.wikipedia.org/wiki/Open_access)).
-   Grafikleri güzel ve dışa aktarılabilir (pdf, png, eps, tikz ve daha onlarcası).
-   Doğrudan LaTeX veya html çıktısı alabilirsiniz.

Örnek R Grafikleri
==================

Dediğim gibi R'ı bir grafik hazırlama programına indirgemek aslında büyük haksızlık. Ancak R kullanarak hazırlayabileceğiniz grafiklerin çeşitliğini görmek açısından aşağıdaki linklere göz atabilirsiniz. Bazı linklerde grafiklerin kodları da mevcut, hoşunuza giden grafiği kendi datanızla birkaç dakika içinde çizdirebilirsiniz.

-   [Addicted to R](http://addictedtor.free.fr/graphiques/thumbs.php): Çeşitli R grafikleri, kodlar mevcut.
-   [Astronomi Uygulamaları:](http://www.sr.bham.ac.uk/%7Eajrs/R/r-gallery.html) Sitede grafikler, kodları ve eğitim materyalleri mevcut.
-   [R Graphics:](http://www.stat.auckland.ac.nz/%7Epaul/RGraphics/rgraphics.html) Daha basit grafikler ve kodları.
-   [R ile interaktif web grafikleri:](http://dl.dropbox.com/u/7586336/blogger/Cambridge_R_googleVis_with_knitr_and_RStudio_May_2012.html) Bu da [nasıl oluşturulduğu](http://www.r-bloggers.com/interactive-html-presentation-with-r-googlevis-knitr-pandoc-and-slidy/) (he he [Pandoc](http://www.asuyatuyolar.org/2012/06/pandoc-ile-metin-dosyalarn-donusturmek.html) kullanmış)
-   [AniWiki:](http://animation.yihui.name/) R ile animasyon hazırlama örnekleri, ister sitenize koyun ister [LaTeX ile pdf dokümanınıza](http://robjhyndman.com/researchtips/animations/) ekleyin.

R Nasıl Yüklenir?
=================

Umarım bu kadar örnek sizi ikna etmeye yetmiştir. Şimdi gelelim R'ı nasıl kullanmaya başlayabileceğinize:

R'ı indirin:
------------

-   [Windows](http://ftp.yalwa.org/cran/bin/windows/base/)

-   [Linux](http://ftp.yalwa.org/cran/bin/linux/)

-   [Mac](http://ftp.yalwa.org/cran/bin/macosx/)

  Yukarıdaki linklerden R'ın son sürümünü indirip, kurabilirsiniz.

RStudio'yu kurun:
-----------------

Aslında R'ı kendi başına çalıştırabilir ve istediğiniz metin editörünü kullanarak kodlarınızı yazabilirsiniz, ancak [Rstudio](http://rstudio.org/) işlerinizi çok kolaylaştıracak, güzel arayüzlü bir program. Aşağıdaki linkden indirebilirsiniz.

[![](http://1.bp.blogspot.com/-VGQIoDwFrPc/T9ZlMLfUpSI/AAAAAAAABkQ/kC1P18IdCI0/s400/rstudio-windows.png)](http://1.bp.blogspot.com/-VGQIoDwFrPc/T9ZlMLfUpSI/AAAAAAAABkQ/kC1P18IdCI0/s1600/rstudio-windows.png)

-   [RStudio İndir](http://rstudio.org/download/desktop)

Daha kurumsal kullanım düşünenler [server sürümünü](http://rstudio.org/download/) indirip programı tüm kullanıcılarına açabilirler.
Sadece İngilizce olsa da Rstudio'nun [yardım bölümü](http://rstudio.org/docs/) oldukça faydalı. [Şu videoda](http://rstudio.org/video.html) Rstudio'nun marifetleri kısaca anlatılmış. R ile yapabilecekleriniz hızlıca göz atmak için Rstudio'yu kurduktan sonra aşağıdaki kodları yazıverin.*
Grafikler için:              demo(graphics)
3-boyutlu grafikler:    demo(persp)*
Bir fonksiyon hakkında yardımı Rstudio'nun yardım penceresinden arayarak ya da fonksiyonun başına soru işareti koyarak alabilirsiniz (mesela, plot fonksiyonu hakkında bilgiyi *?plot* yazarak görebilirsiniz).

R Kaynakları: 
==============

Gördükleriniz sizi ikna ettiyse R öğrenmeye hemen başlayabilirsiniz. Yüzlerce İngilizce kaynak olmasına rağmen malesef hiç Türkçe kaynak bulamadım. Eğer karşılaştığınız sorunlar olursa yardımcı olmaya çalışırım. Niyetim [Yazılım Kardeşliği](http://yazilimkardesligi.org/) sitesi açılınca R desteğini oradan sürdürmek.
Aşağıdaki linklerin yardımcı olacağını ümit ediyorum. Özellikle ilk baştaki 2 dakikalık R videoları oldukça faydalı.

-   [http://www.twotorials.com/](http://www.twotorials.com/)
-   [http://www.cyclismo.org/tutorial/R/](http://www.cyclismo.org/tutorial/R/)
-   [http://scs.math.yorku.ca/index.php/R:\_Getting\_started\_with\_R](http://scs.math.yorku.ca/index.php/R:_Getting_started_with_R)
-   [http://www.ats.ucla.edu/stat/r/](http://www.ats.ucla.edu/stat/r/)
-   [http://www.nceas.ucsb.edu/scicomp/software/r](http://www.nceas.ucsb.edu/scicomp/software/r)

*Devamı gelecek...*


