--- layout: post name: terminaliniz-renklensin title: Terminaliniz renklensin time: 2012-10-16 17:43:00.000000000 +01:00 ---
Mac kullanıcılarının terminal üzerinden çalışmaları sırasında eksikliğini hissettiğinden emin olduğum bir şey var; renkler! Özellikle de Linux deneyimi olan kullanıcılar klasör ve diğer dosyaların özelliklerine göre farklı renklerde listelenmesinin getirdiği kolaylığı mutlaka arıyorlardır.
Neyse ki devasız bir dert değil. Yapmanız gereken **\~/.cshrc** dosyanıza birkaç eklemeden ibaret:
[![](http://4.bp.blogspot.com/-9c27-AnQCnE/UH2QMRPGTsI/AAAAAAAAAEw/OC7bEbCulSk/s200/terminal.png)](http://4.bp.blogspot.com/-9c27-AnQCnE/UH2QMRPGTsI/AAAAAAAAAEw/OC7bEbCulSk/s1600/terminal.png)
*setenv CLICOLOR 1 *
*setenv LSCOLORS ExexcxdxbxegedbxbxExEx *
**bash** kullanıcılarının **.bashrc** dosyasına yukardaki satırları *setenv* yerine *export* olarak yazması yeterli olacaktır.
LSCOLORS'ı takip eden renk kodları neyin ne renkle gösterileceğini belirliyor. Ama hepsi bu kadar değil. Renkleri kendi zevkinize ve/veya alışkanlıklarınıza göre düzenlemek isterseniz; dilediğiniz dosya türünün dilediğiniz fon ve renkte görünmesini ayarlayıp, hatta önizlemesine de bakabileceğiniz şu adrese mutlaka uğramalısınız: [http://geoff.greer.fm/lscolors/](http://geoff.greer.fm/lscolors/)
Rengarenk ve keyifli çalışmalar dileğiyle!
