HTML SVG Ders_1 Tanıtım
HTML5 SVG Nedir?
Ölçeklenebilir vektörel grafikler demektir (Scalable Vector Graphics).
Web için, grafikler tasarlamak amacıyla kullanılır.
XML formatında grafikler çizer.
Çizilen grafikler, ne kadar büyütülse ya da küçültülse de görüntü kaliteleri bozulmaz.
Her SVG elemanı, animasyon ile hareketlenme özelliği kazanabilir.
W3C topluluğunun tavsiye ettiği bir standarttır.
SVG; DOM ve XSL gibi diğer W3C standartlarıyla da uyumludur.
HTML5 <svg> Elemanı
<svg> elemanı HTML5 ile birlikte gelen ve grafik çizmek için kullanılan bir html elemanıdır.

<svg>; grafikler, daireler, kutular, yörüngeler... çizmek için bir çok metoda sahiptir.

<svg> tagı, aşağıdaki tarayıcılar tarafından desteklenir:

Element					
<svg>	4.0	9.0	3.0	3.2	10.1

SVG Daire Çizimi
Aşağıda bir svg dairesinin kodları verilmiştir:

<!DOCTYPE html>
<html>
<body>

<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>

</body>
</html>

Bu kodlara göre şöyle bir daire çizilir:


SVG Dikdörtgen Çizimi
Aşağıda bir svg dikdörtgeninin kodları verilmiştir:

<svg width="200" height="100">
  <rect width="200" height="100" style="fill:rgb(0,0,255);stroke-width:10;stroke:rgb(0,0,0)" />
</svg>



Bu kodlara göre şöyle bir dikdörtgen çizilir:



SVG Oval Dörtgen Çizimi
Aşağıda oval bir dörtgenin kodları verilmiştir:

<svg width="400" height="180">
  <rect x="50" y="20" rx="20" ry="20" width="150" height="150"
  style="fill:red;stroke:black;stroke-width:5;opacity:0.5" />
</svg>

Bu kodlara göre şöyle bir dörtgen ortaya çıkar:



SVG Yıldız Çizimi
Aşağıda bir yıldızın kodları verilmiştir:

<svg width="300" height="200">
  <polygon points="100,10 40,198 190,78 10,78 160,198"
  style="fill:lime;stroke:purple;stroke-width:5;fill-rule:evenodd;" />
</svg>

Bu kodlara göre şöyle bir yıldız ortaya çıkar:



SVG Logo Çizimi
Aşağıda bir logo örneğinin kodları verilmiştir:

<svg height="130" width="500">
  <defs>
    <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <ellipse cx="100" cy="70" rx="85" ry="55" fill="url(#grad1)" />
  <text fill="#ffffff" font-size="45" font-family="Verdana" x="50" y="86">SVG</text>
  Üzgünüm, tarayıcınız SVG elemanını desteklemiyor...
</svg>

Bu kodlara göre şöyle bir logo ortaya çıkar:


SVG
Canvas ve SVG Arasındaki Farklar
SVG; XML'de, 2D çizimleri tanımlamak için kullanılan bir dildir.

Canvas; JavaScript ile çabuk bir şekilde 2D çizimleri yapmak için kullanılır.

SVG; XML tabanlıdır, yani svg elemanları, SVG DOM bünyesinde kullanılabilir, JavaScript kodları ile desteklenebilir.

SVG'de, her bir şekil, bir obje gibi tanınır. Eğer SVG objelerinin bir kısım özellikleri değişirse, tarayıcılar bu objeleri, bu değişikliklere göre tekrar düzenler. Fakat canvas elemanlarında böyle bi özellik yoktur.

Aşağıdaki tablo Canvas ve SVG arasındaki farkları özetlemektedir:

The table below shows some important differences between Canvas and SVG:
Canvas	SVG
Çözünürçük sınırlı
Event handler metotlarını desteklemezler.
Zayıf text işleme kapasitesi
 .png veya .jpg uzantılı grafikler oluşturma yeteneği
Yoğun grafik içeren oyun uygulamaları için uygundur.
Çözünürlük sınırsız
Event handler metotlarını desteklerler
Geniş alan uygulamaları için uygunluk.(Google Maps gibi)
Karmaşık grafiklerde yavaş işleme
Oyun uygulamaları için uygun değildir.
