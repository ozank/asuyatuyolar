--- layout: post name: r-ile-yapabilecekleriniz title: R ile Yapabilecekleriniz time: 2012-10-07 20:10:00.000000000 +01:00 ---
R programını güzel grafikler çizmek için kullanabilirsiniz. Ancak R'ı bir grafik çizme aracına indirmek büyük haksızlık olur.  R aslında bir data toplama ve işleme programı. Hemen hemen her iş için geliştirilmiş yüzlerce eklentisiyle eminim sizin de işinize yarayacak bir özelliği vardır.
İlk başta R zor gelebilir. R'ı öğrenmekle geçireceğiniz sürede aynı grafikleri Excel'de yapabilir, günü kurtarabilirsiniz. Açıkcası R öğrenmek (ya da linux, latex vb öğrenmek) biraz aşağıdaki karikatürdeki gibi . İlk başta kaybettiğinizi düşündüğünüz zamanları uzun vadede kazanacağınızdan emin olabilirsiniz.

[![](http://1.bp.blogspot.com/-8Snutwi04Uw/UHClOCvbggI/AAAAAAAAB64/_1AlC1cyKGI/s400/geekler_tr.png)](http://1.bp.blogspot.com/-8Snutwi04Uw/UHClOCvbggI/AAAAAAAAB64/_1AlC1cyKGI/s1600/geekler_tr.png)

Bu arada grafiği Türkçe'ye çevirirken (orjinaline [şu linkden](https://plus.google.com/102451193315916178828/posts/MGxauXypb1Y)ulaşabilirsiniz) geek için güzel bir karşılık bulamadım. Öneriniz varsa düzelteyim.
Her neyse R'ın yapabileceklerinden bazıları:

Resim İşleme
------------

Resim işleme için özelleşmiş programlar olsa da (mesela [OpenCV](http://opencv.org/)), R'ın da elinden bir şeyler geliyor. [EBImage](http://www.bioconductor.org/packages/devel/bioc/html/EBImage.html) ile basit resim işleme işlerini kolayca yapabilirsiniz.Mesela bir biyologsunuz ve bitkilerin yaprak alanlarını karşılaştırmak istiyorsunuz.  [Şu sayfada](http://ec2-184-73-106-109.compute-1.amazonaws.com/wordpress/?p=202) EBImage ile yaprakların yüzey alanını hesaplayan koda ulaşabilirsiniz. [Üstelik kod](https://github.com/tonyworld/bioImage/blob/master/LeafArea.r) sadece 40 satır. Ya da isterseniz [mikroskop görüntüsünden hücreleri](http://ec2-184-73-106-109.compute-1.amazonaws.com/wordpress/?p=186) de kolaylıkla sayabilirsiniz.  Kodlarına da [bu linkden](https://github.com/tonyworld/bioImage/blob/master/CellCount.r) ulaşabilirsiniz.

[![](http://3.bp.blogspot.com/-XoVBZhVDpLE/UEHsjn2A8KI/AAAAAAAAB1Y/Xj_XDrqWnvc/s400/yaprak_alan.jpg)](http://3.bp.blogspot.com/-XoVBZhVDpLE/UEHsjn2A8KI/AAAAAAAAB1Y/Xj_XDrqWnvc/s1600/yaprak_alan.jpg)[![](http://2.bp.blogspot.com/-0U2mH3OnWF8/UEHt2QeAywI/AAAAAAAAB1g/FVroz723cjw/s400/hucre_say.jpg)](http://2.bp.blogspot.com/-0U2mH3OnWF8/UEHt2QeAywI/AAAAAAAAB1g/FVroz723cjw/s1600/hucre_say.jpg)

Sosyal Medya Analizi
--------------------

Malesef sosyal bilimciler (Asu lafım sana) internet ve sosyal medya üstünden veri toplama işlerine yeterince girmiyorlar. Diyelim ki, twitter'dan atılan mesajların içeriğine, konumlarına bakarak bir çalışma yapmak istiyorsunuz. R ile Twitter API'sini kullanarak konu basliklarini, belirlediğiniz twitleri kimlerin attığını filan kolayca görselleştirebilirsiniz. Bunun için [TwitteR](http://cran.r-project.org/web/packages/twitteR/index.html) paketini kullanabilirsiniz. Aşağıdaki linkler daha fazla bilgi verebilir.

-   [Twitter ile Data Analizi](http://dl.dropbox.com/u/6360678/workshop.html)
-   [Twitter ile Data Analizi-2](http://franklincenterhq.org/2429/using-r-to-search-twitter-for-analysis/)
-   [Twitter'dan Metin Analizi](http://www.rdatamining.com/examples/text-mining)
-   [Müşteri Memnuniyeti Analizi](http://jeffreybreen.wordpress.com/2011/07/04/twitter-text-mining-r-slides/)
-   [Kelime Bulutu Oluşturma](http://rpubs.com/chrisbrunsdon/twitterclouds)

[![](http://3.bp.blogspot.com/-UXTag_4s2gw/UHCudx2q-_I/AAAAAAAAB7o/FL5kjwTfO-U/s320/sna-terms-2.png)](http://3.bp.blogspot.com/-UXTag_4s2gw/UHCudx2q-_I/AAAAAAAAB7o/FL5kjwTfO-U/s1600/sna-terms-2.png)

Paketi kullanması oldukça basit. Mesela dün Avcılar'da yaşanan linç olayıyla ilgili (ana-akım medyadan duyduğunuzu sanmam. Bakınız [Bianet](http://www.bianet.org/bianet/lgbtt/141312-tasinmazsaniz-sizi-zorla-atariz), [Indymedia](http://istanbul.indymedia.org/tr/haber/avc%C4%B1larda-trans-bireylere-y%C3%B6nelik-lin%C3%A7-giri%C5%9Fimi-engellendi)) \#translarirahatbirakin etiketini içeren son 1000 twiti listelemek ve bir metin dosyasına kaydetmek için gereken sadece 3 satır kod. Bu kodla oluşturduğum dosyaya [şuradan](http://dl.dropbox.com/u/2490601/for%20download/trans.txt) ulaşabilirsiniz.

> library("twitteR")
> a\<-searchTwitter('\#translarirahatbirakin', n=1000)
> capture.output(a[ ], file="trans.txt")

Ulaşabileceğiniz kaynaklar sadece twitter ile sınırlı değil. Diğer excel tablolarını, SPSS datalarını, websitelerin içeriklerini ve MYSQL gibi veritabanları da R ile kolayca okuyabilirsiniz.

-   [Tapping the Data Deluge with R](http://www.slideshare.net/jeffreybreen/tapping-the-data-deluge-with-r)
-   [How-to Extract Text From Multiple Websites with R](http://christophergandrud.blogspot.co.uk/2012/02/how-to-extract-text-from-multiple.html)

Eğer aklınıza yatan bir çalışma varsa yardım etmeye çalışırım.

İnteraktif Arayüzler Oluşturun
------------------------------

[Rook](http://cran.r-project.org/web/packages/Rook/index.html) eklentisi ile web tabanlı arayüzler oluşturabilir, Bu eklentileri [GoogleVis](https://developers.google.com/chart/interactive/docs/gallery) ile eşleştirebilirsiniz. Kendi verinizi sağlayabileceğiniz gibi [Google Public Data](http://www.google.com/publicdata/directory) sayfasından ya da [Dünya Bankası veritabanı](http://data.worldbank.org/) gibi yerlerden ulaşabilirsiniz. Aşağıdaki örnekler neler yapabileceğiniz hakkında bir fikir verir umarım.

[![](http://2.bp.blogspot.com/-gcfg3Lh-G1s/UHGwqNJZOQI/AAAAAAAAB8Y/55bH8nGz1XM/s400/google_vis.png)](http://dl.dropbox.com/u/7586336/blogger/Cambridge_R_googleVis_with_knitr_and_RStudio_May_2012.html#%288%29)

-   [Interaktif Google grafikleri](http://code.google.com/p/google-motion-charts-with-r/)
-   [R ile Dünya Bankası verilerine ulaşma](http://lamages.blogspot.co.uk/2011/09/accessing-and-plotting-world-bank-data.html)
-   [GoogleVis Örnekleri](http://code.google.com/p/google-motion-charts-with-r/#Examples)

Grafikleri Doğrudan LaTeX'e ya da Web Sitenize Ekleyin
------------------------------------------------------

R kullanmaya başladığım zaman en tav olduğum özellik grafiklerin doğrudan LaTeX içine eklenebilmesi oldu. Eklemekten kastım, .png ya da .pdf olarak kaydedip eklemek değil. [Tikz](http://www.texample.net/tikz/) dosyası olarak kaydedip eklemek de değil (ki bu özellik kendi başına bile çok faydalı). Beni asıl etkileyen, [knitr](http://yihui.name/knitr/) paketiyle R grafiği kodlarının doğrudan Latex dokümanına eklenebilmesi.
Mesela  değişik verilerle tekrar hazırlamak zorunda olduğunuz bir raporunuz var. Word ve Excel kullanarak hazırladığını düşünürsek. Her yeni veriyi Excel'e yüklemeniz, grafikleri yeniden çizdirip, Word'deki grafikleri, tabloları ve metini güncellemeniz gerekecek. Aynı işi [Knitr](http://yihui.name/knitr/) ile yaptığınız zaman yeni verilerinizi güncellediğiniz anda tüm grafikleriniz ve metniniz güncellenip raporunuz anında hazır hale gelecektir. Üstelik sadece pdf olarak değil isterseniz .html dosyası olarak da kaydedebilirsiniz. [Rstudio](http://rstudio.org/) kullanıyorsanız, [Rpubs](http://rpubs.com/) sitesinde raporunuzu doğrudan yayınlayabilirsiniz. İlk başta kullanmak biraz zor gelecektir, ama öğrendikten sonra birçok angarya işi ne kadar kolay yapabildiğine şaşıracaksınız (bakınız sayfanın başındaki karikatür). Verilerle uğraşan akademisyenlere ve yüksek lisans/doktora öğrencilerine ne kadar önersem azdır.
R ve Knitr'la neler yapılabileceğine birkaç örnek:

[Knitr Örnekleri](http://yihui.name/knitr/demo/showcase/)

-   [Knitr ile Sunumlar Hazırlayın](http://www.r-bloggers.com/how-to-make-html5-slides-with-knitr/) 
-   [İnternet üstünden knitr'ı deneyin](http://public.opencpu.org/apps/knitr/)

[Rpubs: R ile Doğrudan Web Sitesi Hazırlama](http://rpubs.com/)

-   [Yıldırım düşen yerler analizi](http://rpubs.com/jelsner/2021)
-   [Convex-Concave yüzeyler](http://rpubs.com/floswald/1969)

Büyük Datalar ve Paralel Hesaplama İşleri
-----------------------------------------

Benim henüz işim düşmedi ama eğer verileriniz veya analizleriniz tek bilgisayarın başa çıkabileceğinden büyükse R'ın paralel hesaplama paketlerini kullanarak analizinizi birçok bilgisayarda aynı anda çalıştırabilirsiniz. Hatta doğrudan [Amazon'un bulut hizmetinden](http://aws.amazon.com/ec2/) yararlanabilirsiniz. Üniversitenizin bir paralel hesaplama hizmeti varsa ne ala ama yoksa sıfırdan bir cluster oluşturmak yerine böyle hizmetlerden yararlanmak hem daha ucuz hemde daha zahmetsiz diye düşünüyorum. Gene aşağıdaki bağlantılara göz atabilirsiniz.

-   [R ile Amazon EC2'yi eşleştirme](http://decisionstats.com/2010/09/25/running-r-on-amazon-ec2/)
-   [R ile AWS'ı 15 dakikada eşleştirme](http://blog.revolutionanalytics.com/2011/01/run-r-in-parallel-on-a-hadoop-cluster-with-aws-in-15-minutes.html)
-   [R ile AWS kullanma (2.kısım)](http://jeffreybreen.wordpress.com/2011/01/10/segue-r-to-amazon-elastic-mapreduce-hadoop/)
-   [OpenCPU](http://public.opencpu.org/pages/)

Eğer R kullanmaya başlayıp da takıldığınız yerler olursa sormaktan çekinmeyin.
