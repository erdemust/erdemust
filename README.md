

## HTML5 SVG Nedir?

-   Ölçeklenebilir vektörel grafikler demektir (Scalable Vector Graphics).
-   Web için, grafikler tasarlamak amacıyla kullanılır.
-   XML formatında grafikler çizer.
-   Çizilen grafikler, ne kadar büyütülse ya da küçültülse de görüntü kaliteleri bozulmaz.
-   Her SVG elemanı, animasyon ile hareketlenme özelliği kazanabilir.
-   W3C topluluğunun tavsiye ettiği bir standarttır.
-   SVG; DOM ve XSL gibi diğer W3C standartlarıyla da uyumludur.

## HTML5 <svg> Elemanı

<_svg_> elemanı HTML5 ile birlikte gelen ve grafik çizmek için kullanılan bir html elemanıdır.

  

<_svg_>; grafikler, daireler, kutular, yörüngeler... çizmek için bir çok metoda sahiptir.

  Aşağıdaki örnekle kırık çizgiler oluşturabilirsiniz:


<svg height="250" width="450">
    <polyline points="20,25 40,45 60,70 90,125 127,145 205,190"
    style="fill:blue;stroke:blue;stroke-width:5" />
</svg>


<!DOCTYPE html>  
<html>  
<body>  
  
<svg width="300" height="200">  
<polygon points="100,10 40,180 190,60 10,60 160,180"  
style="fill:lime;stroke:purple;stroke-width:5;fill-rule:evenodd;" />  
</svg>  
  
</body>  
</html>
  

## SVG Daire Çizimi

 _svg_ dairesinin kodları 

  

<!DOCTYPE  html>  
<html>  
<body>  
  
<svg  width="100"  height="100">  
<circle  cx="23"  cy="20"  r="20"  stroke="green"  stroke-width="4"  fill="yellow"  />  
</svg>  
  
</body>  
</html>


  

  

## SVG Dikdörtgen Çizimi

Aşağıda bir _svg_ dikdörtgeninin kodları verilmiştir:

  

<svg  width="200"  height="100">  
<rect  width="200"  height="100"  style="fill:rgb(0,0,255);stroke-width:10;stroke:rgb(0,0,0)"  />  
</svg>

  


  
  

  

## SVG Oval Dörtgen Çizimi

Aşağıda oval bir dörtgenin kodları verilmiştir:  
  
<svg  width="400"  height="180">  
<rect  x="50"  y="20"  rx="20"  ry="20"  width="150"  height="150"  
style="fill:blue;stroke:Blue;stroke-width:5;opacity:0.5"  />  
</svg>  
  
  
  
  

## SVG Yıldız Çizimi


<!DOCTYPE html>  
<html>  
<body>  
  
<svg width="300" height="200">  
<polygon points="100,10 40,180 190,60 10,60 160,180"  
style="fill:lime;stroke:purple;stroke-width:5;fill-rule:evenodd;" />  
</svg>  
  
</body>  
</html>
  
  

## SVG Logo Çizimi

Bu kodlara göre şöyle bir logo ortaya çıkar:  
  
<svg  height="130"  width="500">  
<defs>  
<linearGradient  id="grad1"  x1="0%"  y1="0%"  x2="100%"  y2="0%">  
<stop  offset="0%"  style="stop-color:rgb(255,25,0);stop-opacity:1"  />  
<stop  offset="100%"  style="stop-color:rgb(25,0,0);stop-opacity:1"  />  
</linearGradient>  
</defs>  
<ellipse  cx="100"  cy="70"  rx="85"  ry="55"  fill="url(#grad1)"  />  
<text  fill="#aff"  font-size="45"  font-family="Verdana"  x="50"  y="86">SVG</text>  
Üzgünüm, tarayıcınız SVG elemanını desteklemiyor...  
</svg>  
  
Bu kodlara göre şöyle bir logo ortaya çıkar:  
  
   

## Canvas ve SVG Arasındaki Farklar

<b>SVG; XML'de, 2D çizimleri tanımlamak için kullanılan bir dildir.</b>

  

Canvas; JavaScript ile çabuk bir şekilde 2D çizimleri yapmak için kullanılır.

  

SVG; XML tabanlıdır, yani svg elemanları, SVG DOM bünyesinde kullanılabilir, JavaScript kodları ile desteklenebilir.

  

SVG'de, her bir şekil, bir obje gibi tanınır. Eğer SVG objelerinin bir kısım özellikleri değişirse, tarayıcılar bu objeleri, bu değişikliklere göre tekrar düzenler. Fakat canvas elemanlarında böyle bi özellik yoktur.

  

Aşağıdaki tablo Canvas ve SVG arasındaki farkları özetlemektedir:

  

The table below shows some important differences between Canvas and SVG:
Canvas

SVG

-   Çözünürçük sınırlı
-   Event handler metotlarını desteklemezler.
-   Zayıf text işleme kapasitesi
-   .png veya .jpg uzantılı grafikler oluşturma yeteneği
-   Yoğun grafik içeren oyun uygulamaları için uygundur.

-   Çözünürlük sınırsız
-   Event handler metotlarını desteklerler
-   Geniş alan uygulamaları için uygunluk.(Google Maps gibi)
-   Karmaşık grafiklerde yavaş işleme
-   Oyun uygulamaları için uygun değildir.
