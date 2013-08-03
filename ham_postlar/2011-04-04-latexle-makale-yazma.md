--- layout: post name: latexle-makale-yazma title: Latex'le Makale Yazma time: 2011-04-04 01:05:00.000000000 +01:00 ---

Latex'le aslında mastır yaparken tanışmıştım ama mastır tezimi Word'le hazırlamak daha kolayıma gelmişti, şu yazımızda ([Word ile tez yazma](http://asuyatuyolar.blogspot.com/2010/09/microsoft-word-ile-tez-yazma.html)) anlattığım tüm yöntemleri uygulamama rağmen, şimdi dönüp baktığımda Word'e harcadığım vakitlere acıyorum. Peki ya ben Latex öğrenmeli miyim diye soranlara,
'*eğer akademik kariyer düşünüyorsanız, Latex'i vakit geçirmeden öğrenin.'*

derim. Yok akademik kariyer düşünmüyorsanız o zaman Word'le idare edebilirsiniz.

[![](http://2.bp.blogspot.com/-yCafCpW9pOM/TZiwLru_M3I/AAAAAAAAA3U/deiqc4-I78Q/s200/latex_logo.jpg)](http://www.google.com/search?client=ubuntu&channel=fs&q=latex&ie=utf-8&oe=utf-8)

Geçen hafta bir makale gönderdik, bu süreçte öğrediklerimi sıcağı sıcağına sizinle de paylaşayım dedim. Yani bu yazı Latex'e giriş yazısı değil, Latex kullananlara makale yazma sürecini anlatan bir yazı olacak. Ama yeni başlayanlar için Latex konulu bir yazıyı da vakit bulduğumda hazırlayacağım.
Giriş
Biri işte biri evde olmak üzere iki bilgisayar üstünden çalıştım. Okuldaki bilgisayar Windows, evdeki Ubuntu. Makalemiz [IEEE Trans. on Industrial Electronics](http://tie.ieee-ies.org/). Eğer siz de IEEE dergi ya da konferansına makale yollayacaksanız işiniz çok kolay çünkü oldukça kullanışlı bir Latex şablonu var ([IEEE Digital Toolbox](http://www.ieee.org/publications_standards/publications/authors/authors_journals.html)). Özellikle bu şablonun [kullanma klavuzunun](http://ctan.sqsol.co.uk/macros/latex/contrib/IEEEtran/IEEEtran_HOWTO.pdf) çıktısını alıp, bir yere koymanızı tavsiye ederim, baya işinize yarayacak.
Ama başka birçok dergi ve konferans için de Latex şablonları mevcut. İlk yapmanız gereken bu şablonu indirmek olsun.
Eşleştirme
İki bilgisayardan çalışıyorsanız ve tüm dosyalarınızı eşleştirmiyorsanız işiniz oldukça zor. Tek bilgisayardan çalısıyorsanız ya da dosyalarınızı usb-hafıza üzerinden taşıyorsanız iyi güzel ama ya kaybolursa, ya bilgisayarınız bozulursa? Bence en güzel çözüm [Dropbox kurmak.](http://asuyatuyolar.blogspot.com/2009/12/dropbox.html)

[![](http://1.bp.blogspot.com/-1Tdkg5zprUQ/SyzsDWe1RdI/AAAAAAAAAZk/7cqGEcm6uQo/s1600/logo.png)](https://www.dropbox.com/referrals/NTkxMjU3Mjk?src=global9)

Ayrıca, Dropbox'da [ortak bir klasör oluşturarak](http://asuyatuyolar.blogspot.com/2011/02/ileri-dropbox-teknikleri.html) diğer yazarlarla aynı dosyalar üstünde rahatlıkla çalışabilirsiniz. Makaleniz için bir klasör oluşturun ve ilgili olabilecek her şeyi (resimler, datalar, referanslar) alt klasörler halinde bu klasöre kopyalayın.
Bu arada, eğer çalıştığınız arkadaşlarınızdan birisi Latex kullanmaya yanaşmıyosa, [Latex2Rtf](http://en.wikipedia.org/wiki/LaTeX2RTF) programıyla .rtf formatına çevirebilirsiniz.
Latex Editörü
Eğer alıştığınız bir latex editörünüz varsa sorun yok ama yeni bir editör aramaktaysanız ben [TexmakerX](http://texmakerx.sourceforge.net/) kullanıyorum, tavsiye ederim.

[![](http://2.bp.blogspot.com/-yi9ZmBrVteY/TZddfqjMjFI/AAAAAAAAA2w/t5EdCQ1MVuI/s320/texmakerx.png)](http://texmakerx.sourceforge.net/)

Programın Linux, Windows ve Mac versiyonları mevcut. Latex'e yeni başlayanlar için birçok güzel özelliği mevcut (kod tamamlama, geniş denklem editörü, yazım klavuzu vs.) Programı aşağıdaki resimden indirebilirsiniz.

[![](http://people.umass.edu/phil513-klement/editors/texmaker.gif)](http://texmakerx.sourceforge.net/)

Ayrıca son zamanlarda [Gummi](http://gummi.midnightcoding.org/) adlı programı da sevmeye başladım. Ama daha fazla editör hakkında bilgi almak istiyorsanız. [Şu linkde](http://www.charlietanksley.net/philtex/editors/)en yaygın olan 8 tanesi karşılaştırılmış.
**
**
Referanslar
Referanslar için [Mendeley](http://www.mendeley.com/) programını kullanıyorum (daha önce [şu yazımızda](http://asuyatuyolar.blogspot.com/2009/12/mendeley-akademik-pdf-ve-referans.html)değinmiştik.)

[![](http://2.bp.blogspot.com/-fp_X6wNHxlo/SzABJscyDZI/AAAAAAAAAZs/84EAs_0sEhs/s200/Mendeley.png)](http://www.mendeley.com/)

 Mendeley'in makale yazarken iki yönden çok avantajını gördüm.
1-Bilgisayarların herhangi birinde eklediğim makaleler ve aldığım notlar otomatik olarak eşleniyor.
2-Latex'de kullanacağım .bib dosyalarını otomatik olarak yaratabiliyorum. Eğer bu bibtex dosyasını da dropbox'a koyarsanız bilgisayarlar arasında otomatik olarak eşleştirlecektir.
Bunun için bence en pratik yol, Mendeley'de makalenizde referans vereceğiniz tüm kaynakları bir klasörde toplayın.

[![](http://1.bp.blogspot.com/-XEnv4lh0YVk/TZdgCAHiOjI/AAAAAAAAA20/nlT3tDN7FRg/s320/mendeley1.png)](http://asuyatuyolar.blogspot.com/2009/12/mendeley-akademik-pdf-ve-referans.html)

Sonra Mendeley ayarlarından, her klasör için bir bibtex dosyası oluşturun ve kayıt yeri olarak da dropbox'da bir klasör seçin. Bu işin güzelliği diğer yazarlar Mendeley kullanmasa bile .bib dosyaları onların bilgisayarlarına da eşleştirilecektir.

[![](http://3.bp.blogspot.com/-RM2WcpEJOn8/TZdglZ3WfEI/AAAAAAAAA24/R06lyru2HCQ/s320/mendeley_bib.png)](http://3.bp.blogspot.com/-RM2WcpEJOn8/TZdglZ3WfEI/AAAAAAAAA24/R06lyru2HCQ/s1600/mendeley_bib.png)

Referansları Latex'de atmak için Mendeley'den CTRL + K komutunu kullanabilirsiniz. Bu makalenin citation key'ini  yazar soyadı ve yılı olarak aşağıdaki şekilde kopyalayacaktır. İsterseniz makalerinizi Mendeley'de başka türlü de tanımlayabilirsiniz.
\\cite{Li2008}
Yada buna gerek kalmadan Texmakerx'de  komutu doğrudan yazabilirsiniz. Texmakerx .bib dosyasındaki referanslara göre otomatik tamamlayacaktır.
****
****
Grafikler - Şemalar:
Eğer makalenizde bol bol grafik veya şema kullanıyorsanız, sonradan iş çıkarmamak için derginin kabul ettiği dosya formatlarını mutlaka kontrol edin. IEEE dergileri grafikler için vektörel dosya formatlarını istiyor (.eps veya .pdf dosyalarını). Peki nedir vektörel resimle normal pixel formatlı resmin farkı? Pixel tabanlı dosyalarda (.jpg, .png, .tiff) resim piksellerden oluşturularak yaratılır, ve resim büyütüldükçe noktalar daha belirgin hale gelir. Vektörel resimlerde ise resim büyütüldüğü zaman yeniden oluşturulur ve kalite düşmez. Mesela bir örnekle gösterelim. Aşağıdaki resim normal boyutlarda iken bir sorun gözükmüyor.

[![](http://4.bp.blogspot.com/-uKQiZ9KkCXQ/TZdrDCdK5jI/AAAAAAAAA28/jnr9NLUmxEU/s320/fig1.png) ](http://4.bp.blogspot.com/-uKQiZ9KkCXQ/TZdrDCdK5jI/AAAAAAAAA28/jnr9NLUmxEU/s1600/fig1.png)

Mesela bu dosya normal resim olarak kaydedilseydi, resmi yakınlaştırdığınızda aşağıdaki gibi görünecekti.

[![](http://1.bp.blogspot.com/-Ki7wsrRmnH8/TZdrXhTxR1I/AAAAAAAAA3A/00EOHkl272Y/s400/pixel_zoom.png) ](http://1.bp.blogspot.com/-Ki7wsrRmnH8/TZdrXhTxR1I/AAAAAAAAA3A/00EOHkl272Y/s1600/pixel_zoom.png)

Ama vektörel dosyada ne kadar yakınlaştırsanız da resminiz kalitesinden birşey kaybetmeyecek.

[![](http://1.bp.blogspot.com/-Xmemn4PYiQc/TZdrxPJZgYI/AAAAAAAAA3E/ELJfkUB1b3g/s320/eps_pdf_zoom.png)](http://1.bp.blogspot.com/-Xmemn4PYiQc/TZdrxPJZgYI/AAAAAAAAA3E/ELJfkUB1b3g/s1600/eps_pdf_zoom.png)

Peki bu şekilde elde etmenin yolları nelerdir? Ben şemalarımın hepsini [OpenOffice Draw](http://www.openoffice.org/) ile hazırladım.

[![](http://3.bp.blogspot.com/-H5cJ-E7mMHM/TZdua0LWjDI/AAAAAAAAA3I/4xcaFU9APaQ/s200/open_office_draw.png)](http://www.openoffice.org/)

[OpenOffice](http://www.openoffice.org/)'in güzel bir özelliği, resimleri PDF olarak doğrudan kaydedebilmesi. Eğer çizim yaptığınız sayfanın da boyutlarını şemanıza göre ayarlarsanız. Bu pdf dosyasını pdflatex kullanarak doğrudan makalenizde kullanabilirsiniz. Gene OpenOffice'den .eps olarak da kaydetmeniz mümkün. Eps dosyalarınızla pdflatex'i bir arada kullanmak için de [epstopdf](http://www.ctan.org/pkg/eps2pdf)paketini kullanmanızı öneririm. Grafiklerinizi de Excel'in OpenOffice versiyonu olan [Calc](http://www.openoffice.org/) ile hazırlamanızı öneririm. Excel'e göre renk ve font ayarları oldukça başarılı. Calc'den grafiklerinizi pdf değil de eps olarak kaydetmek isterseniz [şu sitede anlatılan](http://www.oooforum.org/forum/viewtopic.phtml?t=60155) makro işinizi baya kolaylaştırabilir.**

[![](http://4.bp.blogspot.com/-5c2pAqYPu3s/TZdyI2geraI/AAAAAAAAA3Q/nlcayjTJ2pA/s200/openoffice-calc.png)](http://www.openoffice.org/)

Ancak, daha kompleks grafikler hazırlamak istiyorsanız ve okulunuzun da lisansı varsa MATLAB kullanabilirsiniz (ya da zaten kullanıyorsunuzdur).  MATLAB'da grafiklerinizin okunaklı olması için bir kaç ayarı değiştirmenizde fayda var. Mesela sayfa fontlarını biraz büyütmek gibi,

`set(0,'DefaulttextFontSize', 16);set(0,'DefaultaxesFontSize', 16);`

Bu ayarlar [şu sayfada](http://www.agmonim.com/2009/05/making-better-eps-figures-with-matlab-for-texlatex-papers/) gayet güzel açıklanmış. Ayrıca, MATLAB'den grafikleri pdf veya eps olarak kaydetme çok başarılı değil, özellikle fontlarla ilgili birkaç sıkıntı yaşadım. Ancak [Matlab Central'daki SaveFig eklentisini](http://www.mathworks.com/matlabcentral/fileexchange/10889-savefig) indirerek, bir çok formatta, istediğiniz çözünürlükte rahatlıkla kaydedebilirsiniz. Ayrıca [şu sayfadaki](http://www.mathworks.com/matlabcentral/fileexchange/?dir=desc&sort=downloads&term=tag%3A%22latex%22) eklentilerden de ilginizi çeken olabilir.

Resimler

Eğer resimleriniz varsa önerim son aşamaya kadar .tiff olarak saklamanız. Dosya boyutu oldukça büyüktür ama  jpeg gibi her dosyayı kaydedişinizde resmin kalitesi düşmez. Eğer .pdf ya da .eps olarak kaydedemediğiniz şemalarınız varsa onları da PNG formatıyla kaydedin. IEEE jpeg ve png dosyalarını da kabul etmiyor. Ama png bazı konularda jpeg e göre daha avantajlıdır, aşağıdaki karikatür png ve jpeg farklarını güzel açıklamış (sağ ve soldaki yazıların kalitesine dikkat).

[![](http://www.dailycupoftech.com/wp-content/uploads/2009/08/jpg-vs-png2.png)](http://www.dailycupoftech.com/wp-content/uploads/2009/08/jpg-vs-png2.png)

Eğer resimleriniz üstünde kesme biçme, yazı ekleme, çözünürlüğü ayarlama, renkleri düzenleme gibi işler yapmanız gerekiyorsa [GIMP](http://www.gimp.org/) programını kullanabilirsiniz. GIMP, Photoshop'un ücretsiz versiyonu, tavsiye ederim.

[![](http://4.bp.blogspot.com/-aR00WZltzn4/TZdxL_USUuI/AAAAAAAAA3M/EOrNbU1kNkE/s200/gimp.png)](http://www.gimp.org/)

Makalenin İçeriği
Tabi ki en zor kısım gene makalenin kendisini yazma, sonra yazım hatalarınızı düzeltme kısmı filan. Belki işinize yarayabilecek bir kaç link.
[Asu'ya Tüyolar - İngilizce Yazma](http://asuyatuyolar.blogspot.com/2010/11/ingilizce-yazma.html) (Özellikle yazıdaki PhraseBank'a dikkat)
[Purdue OWL - İngilizce Dil bilgisi ve imla ](http://owl.english.purdue.edu/owl/resource/607/02/)
[Yazım Hatalarını Bulma](http://www.englishproofreading.co.uk/free-resources)
[Latex Yazım Tüyoları](http://web.science.mq.edu.au/%7Erdale/resources/writingnotes/latexstyle.html)
Final Dosyaları Teslim
Makaleyi yazdınız, hakem yorumları geldi onları düzelttiniz, sonra başka değişiklikler istediler onları da düzelttiniz ve tebrikler makaleniz yayınlanmak için kabul edildi. Ancak daha çileniz bitmedi çünkü sırada tüm resim formatlarını istenen formatlara çevirmek, dosya adlandırmalarını filan yapmak gerekecek. Şu ana kadar anlattıklarımı uyguladıysanız bu çok da zor olmayacak. Mesela IEEE tüm resimleri hem kendi formatında hem de pdf formatında istiyor, ayrıca figür ve tablo listesini de istiyor. Tüm resim ve tablolarınızı tek dosyada her sayfada bir resim olacak şekilde göndermeniz isteniyorsa, aşağıdaki linkteki yöntem işinize yarayabilir. Ayrıca verilen programı kendi ihtiyaçlarınıza göre değiştirebilirsiniz.

[Preparing Final Submissions for IEEE](http://www.shawnlankton.com/2008/08/preparing-final-submissions-for-ieee-journal-articles/)
----------------------------------------------------------------------------------------------------------------------------------

İşinize Yarayabilecek Linkler
[LatexWiki:](http://en.wikibooks.org/wiki/LaTeX) Latex konusunda birçok bilgiyi bulabileceğiniz kapsamlı bir wiki.
[Getting Started with Latex:](http://www.maths.tcd.ie/%7Edwilkins/LaTeXPrimer/) Yeni başlayanlar için latex bilgilerinin derlendiği bir site.
[Latex Tools:](http://www.dm.ufscar.br/%7Esadao/latex/tex-linux.php?lang=en)Yukarda anltattığımız yardımcı programları ve daha fazlasını anlatan bir site.
[İsmail Arı/Blog:](http://ismailari.com/etiket/latex/) Bu blogdaki latex yazıları da oldukça faydalı.
Eğer sorularınız varsa yardımcı olmaya çalışırım. Eklenmesini istediğiniz site ya da tüyo varsa onları da paylaşabilirsiniz.

**İlginizi Çekebilecek Diğer Yazılar**

-   [İntihal Tespit Programları](http://asuyatuyolar.blogspot.com/2011/03/intihal-tespit-programlar.html)
-   [Akademik Poster Hazırlama](http://asuyatuyolar.blogspot.com/2010/06/akademik-poster-hazirlama.html)
-   [Latex'de Türkçe Karakterler](http://asuyatuyolar.blogspot.com/2011/05/latexde-turkce-karakter-kodlar.html)

