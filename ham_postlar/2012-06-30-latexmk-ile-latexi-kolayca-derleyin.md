--- layout: post name: latexmk-ile-latexi-kolayca-derleyin title: Latexmk ile LaTeX'i kolayca derleyin time: 2012-06-30 14:34:00.000000000 +01:00 ---

[![](http://2.bp.blogspot.com/-yCafCpW9pOM/TZiwLru_M3I/AAAAAAAAA3U/deiqc4-I78Q/s200/latex_logo.jpg)](http://2.bp.blogspot.com/-yCafCpW9pOM/TZiwLru_M3I/AAAAAAAAA3U/deiqc4-I78Q/s1600/latex_logo.jpg)

İlk olarak Latex kullanmaya başladığım zamanlarda referansları bir türlü düzgün çalıştıramamıştım. Daha sonra dokümanı oluştururken,

> latex -\> bibtex -\>latex -\> latex 

sırasıyla çalıştırmak gerektiğini öğrenince hallolmuştu ama pek de tatmin olmamıştım açıkcası, bu iş niye bu kadar karışık olmak zorunda diye.  Benim gibi düşünen birileri varmış ki  [latexmk](http://www.phys.psu.edu/~collins/software/latexmk-jcc/)'yı geliştirmiş. Latexmk bu uzun işlemi basitleştiren ve faydalı birkaç özelliğe sahip bir LaTeX derleyicisi. İşin ilginci Latexmk [Miktex](http://miktex.org/packages/latexmk) ile standart olarak geliyormuş. Yani Windows'a Latex'i daha önceki '[Latex nasıl kurulur?](http://www.asuyatuyolar.org/2011/07/latex-nasl-kurulur.html)' yazısına göre kurduysanız, Latexmk'yı kullanmaya doğrudan başlayabilirsiniz. Ya da sitesinden kurabilirsiniz (Ubuntu kullanıcıları: *sudo apt-get install latexmk*ile yükleyebilirler).
Peki ne faydası olacak bu latexmk'nın

-   Latexmk hangi programı kaç kere çalıştıracağına otomatik karar veriyor. Mesela referanslar değişmediyse, sadece bir kere latex çalıştırıyor. **Böylelikle çoğu derleme çok daha kısa sürede tamamlanıyor.**  Her seferinde 10 saniye kazanç olsa yap içler dışlar bir tez yazımında ne kadar zaman eder?
-   **.aux, .log, gibi ekstra oluşturulan dosyaları otomatik temizleyin.** Gerçi bu işi yapan programcıklarda mevcut ama dahili bir özellik olması güzel.
-   Gelelim en güzel özelliğine, **İsterseniz dosyayı her kaydettiğinizde latex dosyanızı otomatik olarak derleyebilir.  **Dosyanızın son halinin sürekli gözünüzün önünde olmasını seviyorsanız alın size gerçek zamanlı latex uygulaması. Özellikle şekillerde denklemlerde uğraşırken oldukça faydalı. Eğer latex editörünüzü değiştirmeyi düşünürseniz gerçek zamanlı latex'e bir alternatif de [gummi](http://dev.midnightcoding.org/projects/gummi)olabilir.

Her latex editörünün kendi derleme ayarları sayfası var, ama mesela TexmakerX için latexmk'yu şu şekilde kullanabilirsiniz.

[![](http://1.bp.blogspot.com/-dWCsFhr--J8/T-763s63cNI/AAAAAAAABqY/jXlrsYuAbNs/s400/texstudio_latexmk.png)](http://1.bp.blogspot.com/-dWCsFhr--J8/T-763s63cNI/AAAAAAAABqY/jXlrsYuAbNs/s1600/texstudio_latexmk.png)

Tabi istediğiniz gibi özelleştirmeler yapmanız mümkün. [Latexmk'nın kullanma klavuzu](http://www.phys.psu.edu/~collins/software/latexmk-jcc/latexmk-431.txt)oldukça detaylı ve programın da baya bir seçeneği var. İşinize yarayabilecek birkaç örnek:
*latexmk -pv makalem*        Önce derle sonra görüntüle.
*latexmk -pdf makalem*     Latex yerine Pdflatex kullanarak derle.
*latexmk -pvc makalem*      Dosya Her kaydedildiğinde otomatik olarak derle ve görüntüyü güncelle.
*latexmk -c makalem*           Derle ve sonra .aux .log gibi ekstra dosyaları sil.
tabi bu dediklerimi birleştirebilirsiniz, mesela pdf'ye çevir gereksiz dosyaları sil ve görüntüle için
*latexmk -pdf -pv -c makale*  komutunu kullanabilirsiniz.
Windows'da otomatik yenilenme işi (-pvc) .div ve .ps uzantılı dosyalarla daha sorunsuz oluyormuş. Eğer illa pdflatex kullanmak istiyorsanız *latexmk -pdf -pvc  -view=dvi* seçeneğini tavsiye ederim, pdflatexle derlenip sonra div'e çevirilir. İlla pdf olarak yenilensin diyorsanız pdf okuyucusunun dosya yenilendiğinde görüntüyü yenilemesi gerekiyor. Acrobat reader uyumlu değilmiş anladığım kadarıyla, [ghostview](http://www.asuyatuyolar.org/2011/07/latex-nasl-kurulur.html) kullanmak daha sorunsuz sanki. [Sumatra pdf](http://blog.kowalczyk.info/software/sumatrapdf/download-free-pdf-viewer.html)'de kullanabilirsiniz. Ama bunu bir konfigürasyon dosyasında belirtmeniz gerekir. Detaylar  , mesela Sumatrayı belirtmek için aşağıdaki satırı ekleyebilirsiniz.
*\$pdf\_previewer = 'start "c:/Program Files/SumatraPDF/SumatraPDF.exe" %O %S';*
Mac için skim, linux'da evince filan destekliyor. Ubuntu'da evince'le açmak için home klasörüne .latexmkrc adında bir dosya oluşturun ve aşağıdaki satırları ekleyin.
*\$pdf\_previewer = "start evince";**
**\$pdf\_update\_method = 0;*
Başka uygulamalar için aşağıdaki linklere göz atabilirsiniz. İlk başta ayarlaması zor gözükse de uzun vadede baya işinize yarayacaktır. Takıldığınız yerlerde yorumlara yazabilirsiniz.  Yardımcı olmaya çalışırım.
Latexmk ile benzer özellikte bir program da [rubber](https://launchpad.net/rubber). Her ne kadar google'a rubber latex yazarak pek faydalı sayfalara ulaşmak mümkün olmasa da, bu program da incelemeye değer ama artık pek güncellenmiyor herhalde.

### Faydalı linkler:

-   [Latexmk'yı vim ile kullanma](http://www.tjansson.dk/?p=278)
-   [Latexmk gvim](http://www.charlietanksley.net/philtex/vim-live-latex-preview/)
-   [Latexmk'yı WinEdt ve Miktex ile kullanma](http://tex.stackexchange.com/questions/33250/how-to-use-latexmk-in-windows-with-miktex-and-winedt)
-   [Latexmk Mac](http://jon.smajda.com/2008/03/08/latexmk/)
-   [Latexmk ile sürekli derleme](http://magic.aladdin.cs.cmu.edu/2007/11/06/continuous-latex-compilation-using-latexmk/)
-   [ve StackExchange'deki Latexmk soruları](http://tex.stackexchange.com/tags/latexmk/hot)

