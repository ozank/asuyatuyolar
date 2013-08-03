--- layout: post name: latex-nasl-kurulur title: LaTeX nasıl kurulur? time: 2011-07-24 22:39:00.000000000 +01:00 ---

[](http://1.bp.blogspot.com/-l3zlYAQpubU/Tix9C7LfjNI/AAAAAAAAA_o/LIHWWE3RsJs/s1600/texmakerx.jpg)

Şimdiye kadar LaTeX'le ilgili baya yazı yazdık ama LaTeX'in nasıl kurulacağın -dan hiç bahsetmedik. Bu yazımızda (şimdilik) sadece Windows kullanıcıları için LaTeX kurmayı anlatmaya çalışacağım.
Aslında LaTeX kullanmaya başlamak sanıldığından daha kolay:
1-MikTeX kurulumu:
İlk önce Miktex programını kurmalısınız. Bu program yazdığınız latex dosyalarını derleyip .dvi ya da .pdf formatına dönüştüren asıl programdır. Miktex'i aşağıdaki linkden indirebilirsiniz.
[http://www.miktex.org/2.9/setup](http://www.miktex.org/2.9/setup)
Eğer harddiskinizde yer sıkıntınız yoksa, tüm sürümünü kurmanız daha iyi olabilir. Basit paketi kurduğunuzda da, ilerde lazım olan paketleri internet üstünden kolayca yükleyebilirsiniz.

[![](http://1.bp.blogspot.com/-nKIZngB5pPU/TiwP7oY3F7I/AAAAAAAAA_c/1WMHcqij_sI/s1600/miktex_kur.jpeg)](http://1.bp.blogspot.com/-nKIZngB5pPU/TiwP7oY3F7I/AAAAAAAAA_c/1WMHcqij_sI/s1600/miktex_kur.jpeg)

2-Ghostscript kurulumu:

[![](http://1.bp.blogspot.com/-3AKrVLP8iGk/TiwR9NsYD0I/AAAAAAAAA_g/ES7Dzvkrs9M/s1600/ghost64.gif)](http://1.bp.blogspot.com/-3AKrVLP8iGk/TiwR9NsYD0I/AAAAAAAAA_g/ES7Dzvkrs9M/s1600/ghost64.gif)

LaTeX kullanırken .eps ve .dvi dosyalarıya haşır neşir olacaksanız -ki çok büyük bir ihtimalle olacaksınız-, Ghostscript programını da [şu linkden](http://sourceforge.net/projects/ghostscript/files/GPL%20Ghostscript/9.02/) indirip kurmalısınız. Windows sürümünize göre (32bit, 64bit) ilgili dosyayı indirin.
Eğer .eps dosyalarını görüntülemek istiyorsanız [GSview](http://pages.cs.wisc.edu/%7Eghost/gsview/index.htm) programını da kuruverin.

[![](http://4.bp.blogspot.com/-ND5xpI4-d2U/TiwSiIxKL7I/AAAAAAAAA_k/oQRmpLuNTbI/s320/parabolagv.png)](http://4.bp.blogspot.com/-ND5xpI4-d2U/TiwSiIxKL7I/AAAAAAAAA_k/oQRmpLuNTbI/s1600/parabolagv.png)

Ya da GSview yerine [GIMP](http://www.gimp.org/) kurup ghostscriptle de eşleştirebilirsiniz. Bunun nasıl yapıldığına bu yazıda değinmiyorum ama ilgilenen varsa yorumlara yazabilir.

3-LaTeX Editörü: TeXstudio

Belki de en kafa karıştırıcı seçenek, LaTeX dosyalarını hangi editörle yazacağınıza karar vermek olacak. Oldukça fazla ücretsiz program ve birkaç tane de paralı editör var. İlk önce benim kullandığım editörden başlayalım. Sonra diğer seçeneklere de bakarız. Ben [TeXmakerX](http://texstudio.sourceforge.net/)(gerçi yeni ismiyle [TeXstudio](http://texstudio.sourceforge.net/) demek lazım) kullanıyorum.

[![](http://1.bp.blogspot.com/-l3zlYAQpubU/Tix9C7LfjNI/AAAAAAAAA_o/LIHWWE3RsJs/s400/texmakerx.jpg)](http://1.bp.blogspot.com/-l3zlYAQpubU/Tix9C7LfjNI/AAAAAAAAA_o/LIHWWE3RsJs/s1600/texmakerx.jpg)

Bu programın sevdiğim özellikleri:

-   Windows, Linux ve Mac sürümlerinin olması.
-   LaTeX kodlarında ve referanslarda otomatik tamamlama özelliği
-   Dahili yazım denetleyicisi, thesaurus ve versiyon kontrol sistemi.
-   Sol tarafta doküman haritasını ve bulunduğunuz yeri göstermesi 
-   Ayrıca bence yeni başlayanlar için en güzel yanı, birçok tanımlanmış tuş sayesinde LaTeX kodlarını aramak zorunda kalmıyorsunuz.

Programı kurduktan sonra, MikTeX'le sorunsuz bir şekilde çalışması lazım, yok çalışmıyorsa, karşılaştığınız sorunları yorumlara yazarsanız yardımcı olmaya çalışırım.
Diğer Editörler:
Madem konu açıldı, diğer editörlerden de kısaca bahsedelim. Eğer TeXstudio size göre değilse, daha birçok seçeneğiniz var.
[TeXworks](http://tug.org/texworks/):
Nispeten basit arayüzlü ve kullanışlı bir program. Özellikle büyük ekranda pdf ve tex dosyası ile yanyana çalışmaktan hoşlanıyorsanız bir göz atın. Üstelik SyncTex eklentisi ile kod ve pdf arasında çift yönlü aramalar yapabilirsiniz. LaTeX dosyalarını derlemesi oldukça kolay. Sevmediğim özelliği ise renk ayarlarını yapmasının biraz zahmetli olması.

[![](http://3.bp.blogspot.com/-WWqCR_Y1WMs/TiyBcioBqaI/AAAAAAAAA_s/oVUOzoltRn4/s400/texworks.gif)](http://3.bp.blogspot.com/-WWqCR_Y1WMs/TiyBcioBqaI/AAAAAAAAA_s/oVUOzoltRn4/s1600/texworks.gif)

[LyX:](http://www.lyx.org/)
Bu program aslında .tex editörlüğünden biraz daha farklı. Editörlük ve Microsoft Word arasında bir yerde. LyX ile kodlarla uğraşmadan ve dokümanınızı derlemeden formatlamayı yapabiliyorsunuz. Bunlar denklemler ve resimler içinde geçerli.Eğer uzun karışık denklemlerle haşır neşirseniz LyX'in bu özelliği işinizi kolaylaştırabilir. LaTeX'e yeni başlayanlar için kodları hatırlama derdi olmadan LaTeX kullanma açısından güzel bir seçenek olabilir. Ancak bu biraz denize girmeden yüzme öğrenmeye çalışmak gibi bence.

[![](http://4.bp.blogspot.com/-FpN2cOlCWhE/TiyHhWsOmnI/AAAAAAAAA_w/iZNJTz685UM/s400/lyx.png)](http://4.bp.blogspot.com/-FpN2cOlCWhE/TiyHhWsOmnI/AAAAAAAAA_w/iZNJTz685UM/s1600/lyx.png)

LyX'in sevmediğim bir özelliği ise dosyaları .tex formatında değil .lyx formatında kaydetmesi, bu açıdan farklı editörler kullanmanızı kısıtlıyor. Dosyaları .tex formatına da çevirebiliyorsunuz ama uzun ve karışık dokümanlarda ne derece başarılı bilemiyorum.
[TeXnic Center: ](http://www.texniccenter.org/)
Ofisteki arkadaşlarımın favori tercihi olmasına rağmen ben pek ısınamadım. Bunda en büyük pay Windows dışında versiyonlarının olmaması, görünüm ve eklentiler bakımından TeXmaker'ı andırıyor, bir göz atabilirsiniz.

[![](http://3.bp.blogspot.com/-nGf6qVDM1ag/TiyJ7W_XNwI/AAAAAAAAA_0/zcXEBYx4PW8/s400/texnic.jpg)](http://3.bp.blogspot.com/-nGf6qVDM1ag/TiyJ7W_XNwI/AAAAAAAAA_0/zcXEBYx4PW8/s1600/texnic.jpg)

ve Diğerleri:
Konuyu sadece Windows ve yeni başlayanlarla kısıtlı tuttuğumuz için bir çok editöre değinmedim. Ama hardcore LaTeX'ciler için [Gedit](http://www.michaels-website.de/gedit-latex-plugin/), [Emacs](http://www.gnu.org/software/emacs/)  ve Vim var. Sonra gerçek zamanlı LaTeX derlemek isteyenler için [Gummi](http://gummi.midnightcoding.org/) var. Hangi editörün daha iyi olduğuna karar vermek zor. Ama birine alıştıktan sonra hepsi hemen hemen aynı işi yapıyor ve bence o kadar da kritik bir seçim değil. Gerçi [xkcd](http://xkcd.com/378/)'nin aşağıdaki karikatürü öyle demiyor.

[![](http://2.bp.blogspot.com/-bt7GLwhjXq0/TiyMR7XdIkI/AAAAAAAAA_4/EBIWzjZbSFY/s640/emacs.png)](http://xkcd.com/378/)

LaTeX öğrenmek isterseniz, internette birçok kaynak bulabilirsiniz. Bu konudaki bence en güzel Türkçe kaynak, Bekir Karaoğlu'nun çevirdiği:
**[İnce Bir LaTeX El Kitabı.](http://akgul.bilkent.edu.tr/Yunus/lshort.pdf)**
*Bu yazı özet bir anlatım oldu, atladığımız yerler varsa ya da bu konuda yazıların devamının gelmesini istiyorsanız, yorumlarınızı beklerim.*
