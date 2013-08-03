--- layout: post name: grafikleri-duzgun-cizmek title: Grafikleri Düzgün Çizmek time: 2012-09-17 18:53:00.000000000 +01:00 ---
Güzel grafik çizmek için kullanabileceğiniz programlardan daha önce bahsetmiştik. [Benim favorim R](http://www.asuyatuyolar.org/2012/06/excel-kullanmadan-hzl-grafik-hazrlama-r.html) olsa da, [başka başka araçlar](http://www.asuyatuyolar.org/2012/06/excel-kullanmadan-guzel-grafik-hazrlama.html) da mevcut. Ancak güzel grafikler için yapılması gerekenler üç aşağı beş yukarı aynı.
Geçenlerde, [Vis4.net sitesinde bu konuya değinen güzel bir yazı](http://vis4.net/blog/posts/doing-the-line-charts-right/) gördüm yazıdaki ana maddeleri çevirmeye çalıştım. Diğer kaynakları da yazının sonunda bulabilirisiniz.

[![](http://1.bp.blogspot.com/-1PQ7vLoMqa8/T-XVdxv8M3I/AAAAAAAABlU/WBO_BuYXrIc/s320/excel_line_graph.png)](http://1.bp.blogspot.com/-1PQ7vLoMqa8/T-XVdxv8M3I/AAAAAAAABlU/WBO_BuYXrIc/s1600/excel_line_graph.png)

Grafiğinizi Basit Tutun
-----------------------

Grafiklerde söylenegelen önemli noktalardan biri de veri/mürekkep oranıdır. Yani güzel grafikler için grafikteki bilgiyi arttırıp, grafiğin kendisini olabildiğince sadeleştirmelisiniz.Yani grafiklerinizde gereksiz, amaca hizmet etmeyen çizgiler ve detayları kullanmaktan kaçınmalısınız. Bunların başında grafik kutuları, arkaplan renkleri, gereksiz yatay-dikey çizgiler, 3 boyutlu grafikler yer alır. Ayrıca, eksenlerdeki alt ve üst değerleri grafiğin en küçük ve büyük değerlerini belirtmek için kullanabilirsiniz.

[![](http://1.bp.blogspot.com/-0CH5MHiMJnM/UFZFrciFfMI/AAAAAAAAB2Q/W8_yMFrfzUs/s1600/line-chart1.png)](http://1.bp.blogspot.com/-0CH5MHiMJnM/UFZFrciFfMI/AAAAAAAAB2Q/W8_yMFrfzUs/s1600/line-chart1.png)

 
-

 Veri Etiketlerini Grafik İçinde Gösterin
-----------------------------------------

 
-

Grafik göstergesini grafiğin altına ya da üstüne koymak hem her veriyi ayrı renklerde çizme zorunluluğu doğurur hem de okuyucu bu renkleri grafik göstergesinde tek tek eşleştimek için uğraşır. Üstelik siyah beyaz baskılarda bu iş daha da zorlaşır. En güzeli, grafik etiketlerini doğrudan verilerin yanına eklemektir.

[![](http://3.bp.blogspot.com/-ry9g7wlsR1E/UFZIYVk3nCI/AAAAAAAAB3A/uTKIi5usAuk/s1600/line-chart2.png)](http://3.bp.blogspot.com/-ry9g7wlsR1E/UFZIYVk3nCI/AAAAAAAAB3A/uTKIi5usAuk/s1600/line-chart2.png)

 
-

 Önemli Olan Veriyi Vurgulayın
------------------------------

 
-

Eğer grafiğinizde bir veri diğerlerinden daha önemliyse bunu vurgulayın. Bunun için ayrı renk kullanabilir ya da daha kalın çizgiler kullanabilirsiniz.

[![](http://4.bp.blogspot.com/-XzFZQf7g18M/UFZJBTXoHjI/AAAAAAAAB3I/tEeKvtbeXwA/s1600/line-chart3.png)](http://4.bp.blogspot.com/-XzFZQf7g18M/UFZJBTXoHjI/AAAAAAAAB3I/tEeKvtbeXwA/s1600/line-chart3.png)

Eksendeki Sıfır Noktasına Dikkat
--------------------------------

Dikey ekseni sıfırda biten grafikler verinin daha gerçekçi bir şekilde karşılaştırılmasını sağlar. Ancak, verinizdeki küçük değişiklikleri vurgulamak için grafik ekseninin aralığını küçültmek daha uygun olabilir.

[![](http://2.bp.blogspot.com/-K3s2Pp6oGP8/UFZLDaIaaCI/AAAAAAAAB3Q/4w8DgPEVQVM/s1600/line-chart4.png)](http://2.bp.blogspot.com/-K3s2Pp6oGP8/UFZLDaIaaCI/AAAAAAAAB3Q/4w8DgPEVQVM/s1600/line-chart4.png)

[![](http://2.bp.blogspot.com/-xnph1RBOUyg/UFZLJ6O49hI/AAAAAAAAB3Y/wPCWicYbOuY/s1600/line-chart5.png)](http://2.bp.blogspot.com/-xnph1RBOUyg/UFZLJ6O49hI/AAAAAAAAB3Y/wPCWicYbOuY/s1600/line-chart5.png) 

Ancak bu durumlarda dikey ve yatay eksenleri kesiştirmemek ve eksenin aralığının vurgulamak okuyucunun yanılmasını önleyecektir.

[![](http://2.bp.blogspot.com/-S1dcKy8RkhA/UFZM3DYjlZI/AAAAAAAAB3g/O4O9Z_pq2qQ/s1600/line-chart6.png)](http://2.bp.blogspot.com/-S1dcKy8RkhA/UFZM3DYjlZI/AAAAAAAAB3g/O4O9Z_pq2qQ/s1600/line-chart6.png)

 
-

En-Boy Oranı
------------

 
-

Bu [yazının orjinalinde](http://vis4.net/blog/posts/doing-the-line-charts-right/) gözün en rahat 45 derecelik açıya sahip olan grafikleri ayırt edebildiğinden bahsetmiş. Tabi bu 45 dereceyi tutturmak için grafiğinizi çok dar ya da uzun yapmanız gerekebilir. Gene aynı yazıda, bunu engellemek için metini grafiğin yanına eklemek seçeneğinden bahsedilmiş.

[![](http://3.bp.blogspot.com/-2q_mnSvtwYQ/UFZNgA37T8I/AAAAAAAAB3o/mgfE3tNBQ0Y/s1600/line-chart7.png)](http://3.bp.blogspot.com/-2q_mnSvtwYQ/UFZNgA37T8I/AAAAAAAAB3o/mgfE3tNBQ0Y/s1600/line-chart7.png)

[![](http://1.bp.blogspot.com/-pkpL6Ye5qUo/UFZNrthpFZI/AAAAAAAAB3w/hyV8ydD2cSo/s1600/line-chart8.png)](http://1.bp.blogspot.com/-pkpL6Ye5qUo/UFZNrthpFZI/AAAAAAAAB3w/hyV8ydD2cSo/s1600/line-chart8.png)

Ancak çoğu makalede grafık boyu sütun genişliğiyle sınırlı. Bu durumlarda 4:3 oranını (çoğu ekranın en boy oranı) ya da [altın oran](http://tr.wikipedia.org/wiki/Alt%C4%B1n_oran) denilen 1.61'i kullanabilirsiniz. Eğer X ekseni ve Y ekseni birimleri aynı ise (mesela ikisi de metre cinsinden ise), X ve Y ekseninde aynı ölçeği kullanmak verilerinizi daha doğru bir şekilde sunmanızı sağlayacaktır.

 
-

Diğerleri
---------

 
-

### Verilerin Sıralanması

Verilerin Sırası önemli değilse, verileri büyükten küçüğe sıralamak en güzeli.

[![](http://4.bp.blogspot.com/-Ma6Aq9bLcus/UFdNd-UZgEI/AAAAAAAAB4g/fUBgfZSICLU/s320/sirasiz.png)](http://4.bp.blogspot.com/-Ma6Aq9bLcus/UFdNd-UZgEI/AAAAAAAAB4g/fUBgfZSICLU/s1600/sirasiz.png)

[![](http://2.bp.blogspot.com/-qdJBpkIJgZc/UFdNiNhnoyI/AAAAAAAAB4o/D84cQvFrzj8/s320/sirali.png)](http://2.bp.blogspot.com/-qdJBpkIJgZc/UFdNiNhnoyI/AAAAAAAAB4o/D84cQvFrzj8/s1600/sirali.png)

### Veri Tablosu

Veri değerlerini doğrudan grafik üstünde göstermek yerine, grafiğin altında ya da ayrı bir yerde tabloda göstermek daha iyidir.

[![](http://1.bp.blogspot.com/-r9AgKpqsboA/UFdOWB_HzwI/AAAAAAAAB4w/hmNdoM4sWHM/s320/data_label.png)](http://1.bp.blogspot.com/-r9AgKpqsboA/UFdOWB_HzwI/AAAAAAAAB4w/hmNdoM4sWHM/s1600/data_label.png)

[![](http://1.bp.blogspot.com/-HL8HoqjhdjY/UFdOZfv1J4I/AAAAAAAAB44/afJhWE6jpkE/s320/data_table.png)](http://1.bp.blogspot.com/-HL8HoqjhdjY/UFdOZfv1J4I/AAAAAAAAB44/afJhWE6jpkE/s1600/data_table.png)

####  

### Pasta Grafiklerden Kaçının

Pasta grafiklerde verileri karşılaştırmak oldukça zordur. Eğer ikiden fazla veriniz varsa pasta grafiği kullanmamaya özen gösterin.

[![](http://4.bp.blogspot.com/-OuS5gy1Fjgk/UFdP8yxFYPI/AAAAAAAAB5A/G7T3_MyBfF0/s320/pasta.png)](http://4.bp.blogspot.com/-OuS5gy1Fjgk/UFdP8yxFYPI/AAAAAAAAB5A/G7T3_MyBfF0/s1600/pasta.png)

[![](http://1.bp.blogspot.com/-X0ie2MbF3pk/UFdQAb2pzKI/AAAAAAAAB5I/fSn8zJpwhj8/s320/sutun.png)](http://1.bp.blogspot.com/-X0ie2MbF3pk/UFdQAb2pzKI/AAAAAAAAB5I/fSn8zJpwhj8/s1600/sutun.png)

###  

### Vektörel Dosya Formatlarını Tercih Edin

Resimleriniz kaydederken vektörel dosya formatları (pdf, eps, svg) kullanmaya çalışın. Böylelikle resiminiz boyutu büyüse de çözüürlük ile ilgili dertleriniz olmaz. Yok illa resim olarak kaydedecekseniz de PNG formatını kullanın. Grafiklerinizi kaydetmek için kesinlikle JPEG formatı kullanmayın. Daha detaylı bilgi için [poster hazırlama](http://www.asuyatuyolar.org/2011/04/powerpoint-ile-akademik-poster-hazrlama.html) ile ilgili yazıya bakabilirsiniz.

[![](http://www.dailycupoftech.com/wp-content/uploads/2009/08/jpg-vs-png2.png)](http://www.dailycupoftech.com/wp-content/uploads/2009/08/jpg-vs-png2.png)

### Trend Çizgilerini Kullanın

Eğer verilerinizde hata payı bulunuyorsa verilerinizi çizgilerle birleştirmek yerine trend çizgilerini kullanmak daha güzel sonuçlar verebilir ve verileriniz değişimini açıkça vurgulayabilirsiniz.

[![](http://1.bp.blogspot.com/-MPpsPgKf_uc/UFdcuUYtWZI/AAAAAAAAB54/ozsqe1B2LQU/s320/trendsiz.png)](http://1.bp.blogspot.com/-MPpsPgKf_uc/UFdcuUYtWZI/AAAAAAAAB54/ozsqe1B2LQU/s1600/trendsiz.png)

[![](http://4.bp.blogspot.com/-h0OC7dJSguY/UFdcxVSaDeI/AAAAAAAAB6A/FlkJWmFuprc/s320/trendli.png)](http://4.bp.blogspot.com/-h0OC7dJSguY/UFdcxVSaDeI/AAAAAAAAB6A/FlkJWmFuprc/s1600/trendli.png)

 
-

Kaynaklar
---------

[Statistical Graphics Course](http://biostat.mc.vanderbilt.edu/wiki/Main/StatGraphCourse)
[Best Practices for Plots](http://stats.stackexchange.com/questions/396/what-best-practices-should-i-follow-when-preparing-plots)
[Reporting Quantitative Results](http://virg.vanderbilt.edu/AssessmentPlans/Results/Reporting_Results_Quantitative.aspx)
[InfoVis](http://www.infovis.net/printMag.php?lang=2&num=158)
[Ten Chart Design Principles](http://peltiertech.com/WordPress/ten-chart-design-principles-guest-post/)
