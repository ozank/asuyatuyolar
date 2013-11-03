--- 
layout: post 
name: excel-kullanmadan-guzel-grafik-hazrlama 
title: (Excel kullanmadan) Güzel Grafik Hazırlama 
time: 2012-06-23 23:54:00.000000000 +01:00
description: "Excel grafikleri sizce de biraz çirkin değil mi?"
category: articles
tags: [akademik, excel-word, grafik, sunum] 
---

Ne zaman aşağıdaki bir grafik içeren bir makale ya da rapor okusam, içimde bir önyargı oluşuyor. Tabi ki grafikler bir çalışmanın değerini arttırmaz ama düşünmeden edemiyorum, eğer grafikler böyle üstünkörü hazırlanmışsa, veriler de üstünkörü mü toplanmıştır acaba diye.

[![]({{site.url}}/images/excel_line_graph.png)]({{site.url}}/images/excel_line_graph.png)

Ben veri analizlerimde ve grafiklerimde [R](http://www.r-project.org/) kullanıyorum.  R'dan [bir önceki yazıda](http://www.asuyatuyolar.org/2012/06/excel-kullanmadan-hzl-grafik-hazrlama-r.html) bahsetmiştim. Hala R'ın en iyi seçeneklerden biri olduğunu düşüyorum.Çalışma alanınıza göre Excel'den kurtulmanızı sağlayacak onlarca seçenekte mevcut. 

Bu yazıda [visualcomplexity](http://www.visualcomplexity.com/vc/community/tools.cfm), [visualisingdata](http://www.visualisingdata.com/index.php/resources/) ve [datavisualization](http://selection.datavisualization.ch/) sitelerinde bahsedilen seçeneklerden bir kısmından bahsedeceğim. Aşağıdaki seçenekler kesmezse bu sitelere de göz atabilirsiniz.

[Easel.ly](http://easel.ly/)
----------------------------

[Easel.ly](http://easel.ly/) daha çok web siteleri ya da posterleriniz için estetik grafikleri kolayca hazırlamanızı sağlıyor. Sitedeki şablonları kullanabileceğiniz gibi sıfırdan kendi tasarımlarınızı yapabilirsiniz.

[![]({{site.url}}/images/easelly_visual.png)]({{site.url}}/images/easelly_visual.png)

[İnfogr.am](http://infogr.am/)
------------------------------

[İnfogr.am](http://infogr.am/) sitesi de [Easel.ly](http://easel.ly/) ile benzer özelliklere sahip, ama bence şablonlar daha teknik ve daha başarılı. Üstelik elinizdeki excel veya csv verilerini siteye yüklüyebiliyorsunuz. Hazırladığınız grafikleri web sitesi üstünden de yayınlama seçeneği var.

[![]({{site.url}}/images/infogram.jpg)]({{site.url}}/images/infogram.jpg)

[Google Fusion Tables:](http://www.google.com/fusiontables/Home/)
-----------------------------------------------------------------

Eğer [Google dokümanları](http://www.google.com/fusiontables/Home/) severek kullanıyorsanız, Google'ın [Fusion Table](http://www.google.com/fusiontables/Home/)sitesini de seveceksiniz. Datalarınızı Google dokümanı olarak kaydedip, istediğiniz grafikleri çizdirebilirsiniz. Özellikle Google haritaları ile eşleştirmeleriyle [birçok güzel iş](https://sites.google.com/site/fusiontablestalks/stories) çıkarabilirsiniz. Eğer veriler üstünde grupça çalışıyorsanız, paylaşma, düzenleme, yedekleme işleri de çok kolay. Ayrıca [Google Charts](https://developers.google.com/chart/) üstündeki grafikleri de kullanabilir, kendi formatlarınızı hazırlayabilirsiniz.

[![]({{site.url}}/images/fusion_table.png)]({{site.url}}/images/fusion_table.png)

Ancak Fusion'ın asıl gücü sitede barındırdığı milyonlarca açık kaynak veri tablosunda saklı. [Fusion search](http://www.google.com/fusiontables/search) sayfasından istediğiniz konuda arama yapıp sonuçları hemen grafik haline getirebilirsiniz. Mesela Fusion'da [kürtaj diye aratıp](http://www.google.com/fusiontables/search?hl=en&q=abortion) onbinlerce istatistiğe ulaşılabilir. Burdaki [istatistiklerin birinden](http://alaskanlibrarian.wordpress.com/2008/12/14/abortion-rates-worldwide/) aslında Türkiye'de kürtaj oranının o kadar yüksek olmadığını görebilirsiniz.
Google Fusion mantığındaki başka bir site de IBM tarafından geliştirilen [Many Eyes](http://www-958.ibm.com/software/data/cognos/manyeyes/). [Many Eyes](http://www-958.ibm.com/software/data/cognos/manyeyes/)'da da verilerinizi paylaşabilir, [başkalarının paylaştığı verileri](http://www-958.ibm.com/software/data/cognos/manyeyes/visualizations?sort=rating), grafikleri inceleyebilirsiniz.

[TikZ:](http://www.texample.net/)
---------------------------------

Eğer dokümanlarınızı LaTeX ile hazırlıyorsanız, [TikZ](http://www.texample.net/)kullanarak  hem çok güzel sonuçlar elde edebilir hem de grafikleri değiştirmek istediğinizde doğrudan latex dosyalarının üstünde değiştirebilirsiniz. Ayrıca grafik ve metinleriniz arasındaki font uyuşmazlığı, çözünürlük gibi dertleriniz de olmayacak. Özellikle tez yazarken çok ama çok faydasını göreceğinizi garanti ediyorum. Yapmanız gereken tek şey, latex kodunuza aşağıdaki satırı eklemek.

`\usepackage{tikz}`

Daha sonra [TikZ sayfasındaki onlarca örnek grafikten](http://www.texample.net/tikz/examples/) beğendiğinizin kodlarına ulaşıp, doğrudan bu örnekleri değiştirip kullanmaya başlayabilirsiniz. [GNUplot](http://www.gnuplot.info/) ile de .tex uzantılı dosyalar üretmek mümkün.

[![]({{site.url}}/images/tikZ.png)]({{site.url}}/images/tikZ.png)

[Kartograph:](http://kartograph.org/)
-------------------------------------

Eğer araştırmalarınızda haritalar üstünde verileri sunmanız gerekiyorsa, [kartograph](http://kartograph.org/) ile oldukça başarılı ve estetik şekiller oluşturabilirsiniz. Ayrıca [Polymaps](http://polymaps.org/)'e harita konusunda başarılı başka bir uygulama.

[![]({{site.url}}/images/karto.png)]({{site.url}}/images/karto.png)

[Cytoscape:](http://www.cytoscape.org/)
---------------------------------------

[Cytoscape](http://www.cytoscape.org/) karmaşık ağlar ve bunlar arasındaki ilişkileri modellemek için geliştirilmiş açık kaynak bir program. Özellikle biyologlar ve sosyal bilimciler için faydalı olabilir. Zaten sitesinde de bu alanlara yönelik örnekler var. Mesela aşağıda twitter'daki mesaj trafiği gösterilmiş.

[![]({{site.url}}/images/cytoscape.png)]({{site.url}}/images/cytoscape.png)

[D3.js](http://d3.js/):
-----------------------

D3 bir java kütüphanesi eğer java ile zaten haşır neşirseniz, web sitelerine grafik hazıramak için bence en pratik çözümlerden.

[![]({{site.url}}/images/d3js.png)]({{site.url}}/images/d3js.png)

[Matplotlib/SciPy:](http://matplotlib.sourceforge.net/index.html)
-----------------------------------------------------------------

[Matplotlib](http://matplotlib.sourceforge.net/index.html) [SciPy](http://www.scipy.org/SciPy)'ın çizimler için kullanılan modülü. Eğer Matlab kullanıyorsanız ve açık kaynak bir yazılıma geçmek istiyorsanız [SciPy](http://www.scipy.org/SciPy) en güçlü aday bence ([Octave](http://www.gnu.org/software/octave/) da başka bir alternatif). Programla işleri gözünü korkutmasın, bir kere kullanmaya alıştıktan sonra her işinizi çok daha kolay ve profosyonel bir şekilsde yapabilirsiniz. [Matplotlib galerisinde](http://matplotlib.sourceforge.net/gallery.html) yapabileceklerinize göz atabilirsiniz, gene Matplotlib'ile [şekillerinizi .eps formatında Latex'e aktarabilirsiniz](http://www.scipy.org/Cookbook/Matplotlib/LaTeX_Examples). Eğer 3-boyutlu şekiller çizdirmek istiyorsanız, [Mayavi](http://code.enthought.com/projects/mayavi/)'ye göz atabilirsiniz.

[![]({{site.url}}/images/matplotlib.png)]({{site.url}}/images/matplotlib.png)

[Processing:](http://processing.org/)
-------------------------------------

Processing görsel ve interaktif animasyonlar için tasarlanmış bir programlama dili. Ben kullanmadım, ama yapılan işlerde gerçekten sınır yok gördüğüm kadarıyla. [Processing.js](http://processingjs.org/exhibition/) adı altında web siteleri için özelleşmiş bir sürümü de var.

Bu kadar faydalı araç varken, çirkin grafikler üretmek için pek mazeret kalmıyor bence.  Bu programlara ilk başta alışmak biraz zaman alsa da emin olun uzun vadede çok vakit kazanacaksınız.

*Eğer sizin kullandığınız başka programlar varsa, yorumlara yazarsanız süper olur.*

