--- 
layout: post 
name: ack-kaynak-makale 
title: Açık Kaynak Makale 
time: 2013-05-15
---

[![](http://4.bp.blogspot.com/-nrrHe3lWKpo/UYlbfMZNiEI/AAAAAAAACug/8FNz3jAgfG4/s200/Professortocat_v2.png)](http://4.bp.blogspot.com/-nrrHe3lWKpo/UYlbfMZNiEI/AAAAAAAACug/8FNz3jAgfG4/s1600/Professortocat_v2.png)

Son zamanlarda, akademik camiada açık erişim konusu sıkça tartışılır oldu. Bilmeyenler için açık erişimin tartıştığı iki ana nokta var:

İlki yayıncıları hedef alıyor: İnternetle artık insanlara ulaşmak bu kadar kolaylaşmışken, akademisyenler yayınlarını dağıtmak için hala neden aracılara (yayıncı kuruluşlara) ihtiyaç duyuyor. Üstelik bu aracılar yayınların hazırlanması ve hakem kontrolü sürecinde pek de bir emek vermezken, neden üniversiteler bu yayınlara her yıl tonla üyelik parası ödüyorlar? Bazı dergiler açık erişim şeçeneği sunuyor, anca dalga geçer gibi fahiş fiyatlar istiyor. En son bir makale için 3000\$ hesap çıkarmışlardı. Aşağıdaki video bu çıkar döngüsünü oldukça güzel özetlemiş.

![](http://3.bp.blogspot.com/-RZ-J8r0ClNM/UZLEJ7jrocI/AAAAAAAACvs/gV_Pet_71Jo/s320/acik_erisim_ucret.png) 

-   İkinci noktada ise akademisyenlere iş düşüyor. Gene internetle bilgi paylaşmak bu kadar kolaylaşmışken, neden sadece 5-6 sayfalık pdf dosyalarını paylaşıyoruz? Kullandığımız verileri, programları paylaşmadıktan sonra bir araştırma tekrarlanabilir (ve doğrulanabilir) olur mu? Ya da yaptığımız işleri paylaşırsak, birlikte çok daha güzel işler çıkmaz mı? Tekerleği tekrar tekrar icat etmenin bir mantığı var mıdır? 

Neyse bu yazıda makalelerinizi ve verilerinizi nasıl paylaşabileceğinizden bahsedeceğim. Eğer açık erişim konusunda daha fazla fikir sahibi olmak istiyorsanız, aşağıdaki güzel yazıları okuyabilirsiniz.

-   [Akademik Bahar Hareketi](http://enisden.wordpress.com/2012/05/02/akademik-bahar-kampanyasi-akademik-yayinlarin-herkese-acik-olmasi-saglanmali/)
-   [Bilimsel veri ve yazılım paylaşımı ](http://mkoz.wordpress.com/2011/11/01/bilimsel-veri-ve-yazilim-paylasimi/)
-   [Tekrarlanabilir araştırma](http://mkoz.wordpress.com/2013/05/01/tekrarlanabilir-arastirma-ve-rogoff-reinhart-olayi/)
-   [Bilimsel makalelerin ekonomisi(1)](http://www.birgun.net/writer_index.php?category_code=1186995173&news_code=1343292805&year=2012&month=07&day=26) [2.Kısım](http://www.birgun.net/writer_index.php?category_code=1186995173&news_code=1343896727&year=2012&month=08&day=02)  
-   [Açık erişim nedir?](http://www.acikerisim.net/acik-erisim-nedir-2/)
-   [Open Access Movement](http://p2pfoundation.net/Open_Access_Movement)
-   [Reinventing the Academic journal](http://www.historyworkshop.org.uk/reinventing-the-academic-journal-the-digital-turn-open-access-peer-review/)
-   [Directory of Open Access Journals](http://www.doaj.org/)
-   [Open Research Network](http://www.openresearchnetwork.org/)

Makale:
-------

Eylül ayındaki bir [konferans](http://www.ietrpg.org/) için bir makale hazırladım. Makalenin pdf haline [şu linkten](https://www.dropbox.com/s/rr625hmam6dbwun/keysan-iet-rpg-2013.pdf) ulaşabilirsiniz. Makale tez konumla doğrudan alakalı olmasa da çalıştığım projeyle ilgili, rüzgar türbinlerindeki  belli başlı parçaların ağırlık ve verimlilik hesaplamaları için birkaç denklem sunuyorum.  Tabi ne akademiden ne de şirketlerden kimse pek bilgi paylaşımı olmadığı için [verileri toplamak](https://github.com/ozank/wind-turbine-mass/blob/master/gearbox/gearbox_data.txt) biraz uğraştırdı. Sonra bu verileri,  basit bir arayüzle biraz daha kullanılabilir hale getirdim.

[![](http://1.bp.blogspot.com/-t1tzfw20_OQ/UYlcAG_SDZI/AAAAAAAACus/3OgR3J6ZDAo/s320/marina_gui1.png)](http://1.bp.blogspot.com/-t1tzfw20_OQ/UYlcAG_SDZI/AAAAAAAACus/3OgR3J6ZDAo/s1600/marina_gui1.png)

Daha sonra tez danışmanımla bu programı ve verilerimi açık kaynak olarak paylaşmak istediğimi konuştum. Önce kaşlarını kaldırarak , biraz da ne gerek var böyle işlere diyerek dinlese de sonunda ikna oldu. Hatta açık erişim olayı ilgisini çekmiş olacak ki, daha sonra diğer makalelerimizin verilerini de paylaşabileceğimi söyledi.

 Veri Paylaşımı:
----------------

Makalemi ve verilerimi paylaşmak için ilk iş [GitHub](https://github.com/)'da ayrı bir hesap açtım. GitHub ücretsiz versiyon kontrolü hizmeti veren, çok güzel bir site. Versiyon kontrolü nedir diye soruyorsanız önce şu yazılara göz atabilirsiniz:

-   [Akademisyenin İnternet Rehberi: Döküman Yönetimi](http://www.asuyatuyolar.org/2011/12/akademisyenin-internet-rehberi-dokuman.html)
-   [Versiyon kontrol sistemleri](http://blog.mustafakirimli.com/versiyon-kontrol-sistemleri-kullanimi-ve-araclari/71)
-   [Sürüm kontrolü hakkında (Git)](http://git-scm.com/book/tr/Ba%C5%9Flang%C4%B1%C3%A7-S%C3%BCr%C3%BCm-Kontrol%C3%BC-Hakk%C4%B1nda)

Bu yazılarla yeterince vurgulayabildiğimi düşünmüyorum, tekrar edeyim.

> Versiyon kontrolü sistemleri hem verilerinizi organize etmek hem de başkalarıyla paylaşmak için çok faydalı bir araçtır. Ayrıca, sizi yedekleme stresinden ve dokümanları senkronize etme derdinden de kurtarır. Şimdiye kadar kime bu sistemi gösterdiysem tepkileri değişmedi. İlk tepki: 'Ya ne gerek var buna, paylaşmak gerekince mail atıyorum, yedeklemek gerekince flash-diske kaydediyorum.'  Birkaç hafta sonra kullanmaya alışınca: 'Ya ne güzel bir şeymiş bu, ben versiyon kontrolü olmadan bu kadar vakit nasıl çalışmışım?'

Başlamak için hemen [GitHub](https://github.com/)'da hemen bir hesap açabilirsiniz, [üstelik okul mailinizi kullanarak açarsanız](https://github.com/edu) ücretsiz özel depolama alanı da oluşturabilirsiniz. GitHub hakkında bilgi için aşağıdaki yazılara göz atabilirsiniz.

-   [GitHub nedir?](http://www.kodcu.com/2012/10/github-nedir-githubta-deporepository-nasil-olusturulur/)
-   [GitHub kurulumu](http://meraklibilisimci.com/tag/github-nedir/)
-   [CodeSchool-Try Git ](http://try.github.io/levels/1/challenges/1)
-   [GitHub guide ](http://kbroman.github.io/github_tutorial/)

GitHub'ı terminal üstünden kullanmak zorunda da değilsiniz, aşağıdaki programlardan beğendiğinizi kurup, güzel bir arayüzle çalışabilirsiniz.

[Git için programlar](http://git-scm.com/downloads/guis)

[GitHub Windows](http://windows.github.com/)

[SourceTree](http://www.sourcetreeapp.com/)

[![](http://3.bp.blogspot.com/-blgfS8_0s2o/UZLGhhymHWI/AAAAAAAACwE/54twMd_SvrQ/s320/blog-github.png)](https://github.com/)

Artık istediğiniz kodu, dokümanı ya da veriyi herkesle rahatça paylaşabilirsiniz. Bilgisayarınızdaki dosyaları değiştirdikten sonra GitHub'a yükleyebilir, dosyalarınızın tüm geçmiş versiyonlarına rahatça ulaşabilirsiniz.

Yazım Süreci:
-------------

Daha sonra makalem için [GitHub'da bir alan](https://github.com/ozank/wind-turbine-mass) oluşturdum, ve makaleyi orada yazmaya başladım. Makaleyi yazarken [LaTeX](http://www.asuyatuyolar.org/search/label/latex) kullanmanızı şiddetle tavsiye ederim. Böylelikle, makalenizi düz metin dosyasıyla hazırlayabildiğiniz gibi resim ve grafiklerinizi de ayrıca paylaşabilirsiniz. Eğer LaTeX'e ısınamadıysanız [Markdown](http://daringfireball.net/projects/markdown/syntax)'a da bir göz atabilirsiniz.

[![](http://2.bp.blogspot.com/-yCafCpW9pOM/TZiwLru_M3I/AAAAAAAAA3U/deiqc4-I78Q/s320/latex_logo.jpg)](http://www.asuyatuyolar.org/search/label/latex)

Ben makalemi LaTeX ile grafiklerimi de [R](http://www.r-project.org/) ve [Rstudio](http://www.rstudio.com/) kullanarak hazırladım. Rstudio'nun bir avantajı doğrudan versiyon kontolünü desteklemesi (bakınız: [RStudio ile versiyon kontrolü](http://www.rstudio.com/ide/docs/version_control/overview) ), böylelikle başka hiçbir program kullanmadan verilerimi ve grafiklerimi R ile oluşturup, GitHub'la eşleştirebildim.

[![](http://1.bp.blogspot.com/-y6yaa9NPW9w/T86ACeTMjKI/AAAAAAAABj4/Cmx6YZkcJeU/s200/rstudio.png)](http://www.rstudio.com/)

Tabi burada R'ın harika bir eklentisinden de bahsedeyim:[Knitr](http://yihui.name/knitr/)

[![](http://4.bp.blogspot.com/-yU-BZiyxvXE/UZLFrO1oR3I/AAAAAAAACv4/YSDCveOvn6s/s320/knitr.png)](http://yihui.name/knitr/)

Knitr ile R kodlarınızı ve grafiklerinizi doğrudan LaTeX (ya da markdown) dokümanınızın içine gömebilirsiniz. Böylelikle verilerinizi güncellediğiniz zaman, grafikleriniz ve sonuçlarınız otomatik güncellendiği bir PDF (ya da html) dosyası ele edebilirsiniz. Tekrarlanabilir araştırmalar için harika bir araç. Ayrıca sizi birçok angarya işten de kurtarabilir mesela, değişik veri setleriyle aynı şablonu kullanarak, deney raporları hazırlamanız gerekiyorsa. Aşağıdaki bağlantılar daha fazla fikir verecektir:

-   [Knitr](http://yihui.name/knitr/)
-   [Interactive reports in R with knitr and RStudio](http://lamages.blogspot.co.uk/2012/05/interactive-reports-in-r-with-knitr-and.html)
-   [R Markdown ](http://www.rstudio.com/ide/docs/authoring/using_markdown)
-   [Getting started with knitr, Markdown ](http://jeromyanglim.blogspot.co.nz/2012/05/getting-started-with-r-markdown-knitr.html)
-   [Reproducible reports](http://pairach.com/2012/06/18/reproducible-reports-research-with-knitr-in-r-studio/)
-   [A love story with R, LaTeX and knitr](http://machine-master.blogspot.co.uk/2013/03/from-openoffice-noob-to-control-freak.html)

Ayrıca hazırladığınız dokümanları tek tıkla web sitesi olarak [RPubs](http://rpubs.com/) adresinde yayınlayabilirsiniz ve hatta [Shiny](http://www.rstudio.com/shiny/) eklentisiyle web uygulamaları da oluşturabilirsiniz (planım bu makale için oluşturduğum Matlab arayüzünü Shiny'e aktarmak ama henüz vakit bulamadım).
Eğer R'a ısınamayıp Python kullanıyorsanız da [IPython Notebook](http://ipython.org/notebook.html)'a göz atmanızı tavsiye ederim. Aşağıdaki linkler de LaTeX'in içine Python kodu gömmekle ilgili fikir verecektir.

-   [İlginç IPython Notebook örnekleri](https://github.com/ipython/ipython/wiki/A-gallery-of-interesting-IPython-Notebooks)
-   [IPython Notebook](http://software-carpentry.org/blog/2012/03/the-ipython-notebook.html)
-   [Embedding Python in LaTeX](http://www.texample.net/weblog/2008/oct/24/embedding-python-latex/)
-   [SympyTex](http://elec.otago.ac.nz/w/index.php/SympyTeX)
-   [Python inside LaTeX](http://thewikiblog.appspot.com/blog/python-inside-latex)
-   [IPython vs knitR](http://bayesianbiologist.com/2012/11/21/ipython-vs-rstudioknitr/)

Son Söz:
--------

'Dijital yayıncılık devrimi' lafını şu sıralar sıkça duymaya başladık, bu devrimde akademi için de çok faydalı araçlar var. Bu yazıda versiyon kontrolü sistemlerini vurguladık. Ancak verileriniz paylaşmak için bu yazıdaki araçların hiçbirine ihtiyacınız yok.
Makalelerinizde kullandığınız verileri ve modelleri web sitenize ya da Dropbox klasörünüze koyup paylaşmak, hatta yaptığınız sunumlarda kullandığınız verileri isteyenlerle paylaşabileceğinizi söylemek bile, daha açık bir bilim için payınıza düşeni yapmanızı  sağlayacaktır.
Zaten bence asıl zorluk işin teknik boyutundan ziyade, 'Paylaşırsam, verilerim çalınır!' korkusunu yenmek. Ancak bu korku hele de yıl 2013 olmuşken oldukça yersiz. Verilerinizi ve modellerinizi açık erişim yaparak, bilimsel inandırıcılığını kat be kat arttıracağınız gibi, akademik camiada hiç ummadığınız bağlantılar da kazanabilirsiniz. Üstelik açık erişim, yaptığınız yayının etki faktörünü de artırabilir.
Ben, bundan sonra yayınlayacağım hem makaleninin verilerini paylaşacağım diye kendime söz verdim, aha buraya da yazıyorum, bakalım ne kadar devam ettireceğim.
*Eğer sizin kullandığınız başka yöntemler ya da konuyla ilgili düşünceleriniz varsa, yorumlarınızı beklerim.*


