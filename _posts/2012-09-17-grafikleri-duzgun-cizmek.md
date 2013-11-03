--- 
layout: post 
name: grafikleri-duzgun-cizmek 
title: Grafikleri Düzgün Çizmek 
time: 2012-09-17 18:53:00.000000000 +01:00
description: "Grafik çizdirirken nelere dikkat etmek gerekir"
category: articles
tags: [excel-word, grafik]
---

Güzel grafik çizmek için kullanabileceğiniz programlardan daha önce bahsetmiştik. [Benim favorim R](http://www.asuyatuyolar.org/2012/06/excel-kullanmadan-hzl-grafik-hazrlama-r.html) olsa da, [başka başka araçlar](http://www.asuyatuyolar.org/2012/06/excel-kullanmadan-guzel-grafik-hazrlama.html) da mevcut. Ancak güzel grafikler için yapılması gerekenler üç aşağı beş yukarı aynı.
Geçenlerde, [Vis4.net sitesinde bu konuya değinen güzel bir yazı](http://vis4.net/blog/posts/doing-the-line-charts-right/) gördüm yazıdaki ana maddeleri çevirmeye çalıştım. Diğer kaynakları da yazının sonunda bulabilirisiniz.

[![]({{site.url}}/images/excel_line_graph.png)]({{site.url}}/images/excel_line_graph.png)

Grafiğinizi Basit Tutun
-----------------------

Grafiklerde söylenegelen önemli noktalardan biri de veri/mürekkep oranıdır. Yani güzel grafikler için grafikteki bilgiyi arttırıp, grafiğin kendisini olabildiğince sadeleştirmelisiniz.Yani grafiklerinizde gereksiz, amaca hizmet etmeyen çizgiler ve detayları kullanmaktan kaçınmalısınız. Bunların başında grafik kutuları, arkaplan renkleri, gereksiz yatay-dikey çizgiler, 3 boyutlu grafikler yer alır. Ayrıca, eksenlerdeki alt ve üst değerleri grafiğin en küçük ve büyük değerlerini belirtmek için kullanabilirsiniz.

[![]({{site.url}}/images/line-chart1.png)]({{site.url}}/images/line-chart1.png)

 Veri Etiketlerini Grafik İçinde Gösterin
-----------------------------------------

Grafik göstergesini grafiğin altına ya da üstüne koymak hem her veriyi ayrı renklerde çizme zorunluluğu doğurur hem de okuyucu bu renkleri grafik göstergesinde tek tek eşleştimek için uğraşır. Üstelik siyah beyaz baskılarda bu iş daha da zorlaşır. En güzeli, grafik etiketlerini doğrudan verilerin yanına eklemektir.

[![]({{site.url}}/images/line-chart2.png)]({{site.url}}/images/line-chart2.png)

 Önemli Olan Veriyi Vurgulayın
------------------------------

Eğer grafiğinizde bir veri diğerlerinden daha önemliyse bunu vurgulayın. Bunun için ayrı renk kullanabilir ya da daha kalın çizgiler kullanabilirsiniz.

[![]({{site.url}}/images/line-chart3.png)]({{site.url}}/images/line-chart3.png)

Eksendeki Sıfır Noktasına Dikkat
--------------------------------

Dikey ekseni sıfırda biten grafikler verinin daha gerçekçi bir şekilde karşılaştırılmasını sağlar. Ancak, verinizdeki küçük değişiklikleri vurgulamak için grafik ekseninin aralığını küçültmek daha uygun olabilir.

[![]({{site.url}}/images/line-chart4.png)]({{site.url}}/images/line-chart4.png)

[![]({{site.url}}/images/line-chart5.png)]({{site.url}}/images/line-chart5.png) 

Ancak bu durumlarda dikey ve yatay eksenleri kesiştirmemek ve eksenin aralığının vurgulamak okuyucunun yanılmasını önleyecektir.

[![]({{site.url}}/images/line-chart6.png)]({{site.url}}/images/line-chart6.png)

En-Boy Oranı
------------

Bu [yazının orjinalinde](http://vis4.net/blog/posts/doing-the-line-charts-right/) gözün en rahat 45 derecelik açıya sahip olan grafikleri ayırt edebildiğinden bahsetmiş. Tabi bu 45 dereceyi tutturmak için grafiğinizi çok dar ya da uzun yapmanız gerekebilir. Gene aynı yazıda, bunu engellemek için metini grafiğin yanına eklemek seçeneğinden bahsedilmiş.

[![]({{site.url}}/images/line-chart7.png)]({{site.url}}/images/line-chart7.png)

[![]({{site.url}}/images/line-chart8.png)]({{site.url}}/images/line-chart8.png)

Ancak çoğu makalede grafık boyu sütun genişliğiyle sınırlı. Bu durumlarda 4:3 oranını (çoğu ekranın en boy oranı) ya da [altın oran](http://tr.wikipedia.org/wiki/Alt%C4%B1n_oran) denilen 1.61'i kullanabilirsiniz. Eğer X ekseni ve Y ekseni birimleri aynı ise (mesela ikisi de metre cinsinden ise), X ve Y ekseninde aynı ölçeği kullanmak verilerinizi daha doğru bir şekilde sunmanızı sağlayacaktır.

Diğerleri
---------

### Verilerin Sıralanması

Verilerin Sırası önemli değilse, verileri büyükten küçüğe sıralamak en güzeli.

[![]({{site.url}}/images/sirasiz.png)]({{site.url}}/images/sirasiz.png)

[![]({{site.url}}/images/sirali.png)]({{site.url}}/images/sirali.png)

### Veri Tablosu

Veri değerlerini doğrudan grafik üstünde göstermek yerine, grafiğin altında ya da ayrı bir yerde tabloda göstermek daha iyidir.

[![]({{site.url}}/images/data_label.png)]({{site.url}}/images/data_label.png)

[![]({{site.url}}/images/data_table.png)]({{site.url}}/images/data_table.png)

### Pasta Grafiklerden Kaçının

Pasta grafiklerde verileri karşılaştırmak oldukça zordur. Eğer ikiden fazla veriniz varsa pasta grafiği kullanmamaya özen gösterin.

[![]({{site.url}}/images/pasta.png)]({{site.url}}/images/pasta.png)

[![]({{site.url}}/images/sutun.png)]({{site.url}}/images/sutun.png)

### Vektörel Dosya Formatlarını Tercih Edin

Resimleriniz kaydederken vektörel dosya formatları (pdf, eps, svg) kullanmaya çalışın. Böylelikle resiminiz boyutu büyüse de çözüürlük ile ilgili dertleriniz olmaz. Yok illa resim olarak kaydedecekseniz de PNG formatını kullanın. Grafiklerinizi kaydetmek için kesinlikle JPEG formatı kullanmayın. Daha detaylı bilgi için [poster hazırlama](http://www.asuyatuyolar.org/2011/04/powerpoint-ile-akademik-poster-hazrlama.html) ile ilgili yazıya bakabilirsiniz.

[![]({{site.url}}/images/jpg-vs-png2.png)](http://www.dailycupoftech.com/wp-content/uploads/2009/08/jpg-vs-png2.png)

### Trend Çizgilerini Kullanın

Eğer verilerinizde hata payı bulunuyorsa verilerinizi çizgilerle birleştirmek yerine trend çizgilerini kullanmak daha güzel sonuçlar verebilir ve verileriniz değişimini açıkça vurgulayabilirsiniz.

[![]({{site.url}}/images/trendsiz.png)]({{site.url}}/images/trendsiz.png)

[![]({{site.url}}/images/trendli.png)]({{site.url}}/images/trendli.png)

Kaynaklar
---------

- [Statistical Graphics Course](http://biostat.mc.vanderbilt.edu/wiki/Main/StatGraphCourse)
- [Best Practices for Plots](http://stats.stackexchange.com/questions/396/what-best-practices-should-i-follow-when-preparing-plots)
- [Reporting Quantitative Results](http://virg.vanderbilt.edu/AssessmentPlans/Results/Reporting_Results_Quantitative.aspx)
- [InfoVis](http://www.infovis.net/printMag.php?lang=2&num=158)
- [Ten Chart Design Principles](http://peltiertech.com/WordPress/ten-chart-design-principles-guest-post/)
