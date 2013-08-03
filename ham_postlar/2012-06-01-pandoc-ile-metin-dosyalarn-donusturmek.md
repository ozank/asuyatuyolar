--- layout: post name: pandoc-ile-metin-dosyalarn-donusturmek title: Pandoc ile Metin Dosyalarını Dönüştürmek Çok Kolay time: 2012-06-01 00:48:00.000000000 +01:00 ---

[![](http://1.bp.blogspot.com/-eiuhKB4g1LQ/T8gAHWZvnEI/AAAAAAAABjs/ySelrnMDCCo/s200/T-1000.jpg)](http://1.bp.blogspot.com/-eiuhKB4g1LQ/T8gAHWZvnEI/AAAAAAAABjs/ySelrnMDCCo/s1600/T-1000.jpg)

[Pandoc](http://johnmacfarlane.net/pandoc/) ufak boyutuna rağmen çok işinize yarayabilecek açık-kaynaklı bir yazılım. Yaptığı iş onlarca metin dosyasını birbirine çevirmek. Desteklediği formatlardan bazıları:

-   LaTeX (ve beamer)
-   Html (ve html sunumları)
-   Doc, Docx, Odt
-   Epub
-   MediaWiki, Markdown vs.

Peki bu programı nasıl kullanabilirsiniz? Örneğin kolayca bir sunum hazırlayıp internete yüklemek istiyorsunuz. Hemen bir metin dosyası açıp [Markdown](http://johnmacfarlane.net/pandoc/README.html#pandocs-markdown) kullanarak sunumunuzu hazırlayabilirsiniz. Gözünüz korkmasın, mesela aşağıda örnek bir dosya var.

[ Sunum\_hazirla.txt](http://dl.dropbox.com/u/2490601/for%20download/pandoc/sunum_hazirla.txt) 

Sonra bunu Pandoc'u kullanarak [dzslides](http://paulrouget.com/dzslides/) formatına tek komutla çevirebilirsiniz. (Ya da [Slidy](http://www.w3.org/Talks/Tools/Slidy2/Overview.html#%281%29), [S5](http://meyerweb.com/eric/tools/s5/) formatına). Çevirdiğiniz dosya her yerde açılabilen doğrudan web sitenize koyabileceğiniz bir html dosyası (Mesela ben dropbox klasörüme koydum).
Sunumu aşağıdaki bağlantıdan açabilirsiniz.

[Html Sunum](http://dl.dropbox.com/u/2490601/for%20download/pandoc/sunum.html)

Gene de Beamer'dan ve pdf sunumlarından şaşmayanlardan mısınız? O halde sadece aşağıdaki komutu kullanarak ilk baştaki sade metin dosyamızı beamer sunumuna çevirebilirsiniz.

> pandoc -t beamer sunum\_hazirla.txt -o beamer.pdf

[Beamer Sunum](http://dl.dropbox.com/u/2490601/for%20download/pandoc/beamer.pdf)

Sunumlarınızın görünümünü bir şablon dosyası oluşturarak kolayca değiştirebilirsiniz.
Bu yazıda hep sunumlardan bahsettim ama aslında daha ilginç şeyler de yapılabilir. Mesela:

-   Tezinizi, makalelerinizi, ders notlarınızı e-kitap okuyucuları için .epub formatına çevirin.
-   Bir web sitesini doğrudan LaTeX formatına çevirin.
-   Kodlarınızı, grafiklerinizi, denklemlerinizi kolayca websitenizden paylaşın.
-   LaTeX dokümanlarınızı Word veya OpenOffice formatına dönüştürün.

[Pandoc sitesinde](http://johnmacfarlane.net/pandoc/demos.html) daha fazla örnek dosya ve komutlarını bulabilirsiniz. Elindeki materyalleri öğrencilerle paylaşmak isteyen ama üşenen, bahane üreten akademisyenler için  bence [Pandoc](http://johnmacfarlane.net/pandoc/) birebir. Duyurulur. Pandoc kullanmak isteyip de sorun yaşayan olursa yorum kısmına yazsın, yardımcı olmaya çalışırım.

*
*

***Not:** Asu birkaç aylığına Türkiye'ye gitti. Ben de bu sürede daha çok kendime tüyolar formatında yazılar yazacağım. Yani daha teknik konular, daha çok açık kaynak yazılımlar, daha fazla LaTeX, R, SciPy vs. *

*Umarım beğenirsiniz.*
