

HTML5 ile birlikte gelen özelliklerden birisi olan SVG dili ile ilgili bilgiler SVG kullanımı ve SVG örnekleri yer alıyor.

SVG nedir
SVG açılımı Scalable Vector Graphics ( Ölçeklenebilir Vektörel Grafikler )
Web sayfalarında grafik oluşturmak için kullanılır.
HTML geliştiricileri tarafından önerilir
JavaScript kullanımına ihtiyaç yoktur.
HTML5 <svg> etiketi SVG grafikleri için taşıyıcı görevi görür.

SVG etiketi ile çizgi, dikdörtgen, çember, daire vb. çizim yöntemleri vardır.
code blocks for commands


SVG çember ve daire çizmek
```

<!DOCTYPE HTML>
<html lang="tr">

<head>
  <meta charset="UTF-8">
  <title>SVG Örnekleri</title>
</head>

<body>

<svg width="200" height="200">
  <circle cx="50" cy="50" r="40" stroke="black" stroke-width="4" fill="white" />
  <circle cx="150" cy="50" r="40" stroke="black" stroke-width="4" fill="blue" />
</svg>

</body>

</html>
```
SVG dikdörtgen

```
<svg width="400" height="100">
  <rect width="400" height="100" stroke="black" fill="blue" stroke-width="10" />
</svg>
```

SVG yuvarlak dikdörtgen
```
<svg width="400" height="180">
  <rect x="50" y="20" rx="20" ry="20" width="150" height="150"
  style="fill:blue;stroke:black;stroke-width:5;opacity:0.5" />
</svg>
 
```


SVG polygon yıldız

 ```
<svg width="300" height="200">
  <polygon points="100,10 40,198 190,78 10,78 160,198"
  style="fill:lime;stroke:purple;stroke-width:5;fill-rule:evenodd;" />
</svg>
 
```
```
 
 
```



SVG örnek
 ```
<svg height="130" width="500">
  <defs>
    <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <ellipse cx="100" cy="70" rx="85" ry="55" fill="url(#grad1)" />
  <text fill="#ffffff" font-size="45" font-family="Verdana" x="50" y="86">SVG</text>
</svg>
```

```
 <html>
<h1> son</h1>
 <svg width="200" height="200" viewBox="-100 -100 200 200">
  <clipPath id="ball">
    <circle cx="0" cy="20" r="70" />
  </clipPath>

  <circle cx="0" cy="20" r="70" fill="#D1495B" />

  <polyline
    clip-path="url(#ball)"
    points="-120 40 -80 0 -40 40 0 0 40 40 80 0 120 40"
    fill="none"
    stroke="#9C2D2A"
    stroke-width="20"
  />

  <circle
    cx="0"
    cy="-75"
    r="12"
    fill="none"
    stroke="#F79257"
    stroke-width="2"
  />
  <rect x="-17.5" y="-65" width="35" height="20" fill="#F79257" />
</svg>
</html>
 
```





#SVG ve Canvas arasındaki farklar

##SVG XML tabanlı grafik çizimi için kullanılan bir dildir.

##Canvas JavaScript ile grafik çizimi yapmak için kullanılan bir etikettir.

#SVG XML tabanlı olduğundan SVG etiketlerine JavaScript DOM ile olay (tıklama, üzerine gelme vb.) ekleyebiliriz.

 
#Canvas	 
Sayfayı yakınlaştırınca çözünürlük bozulur.
Çizim nesnelerine JavaScript olayı eklenemez.
Çizim .png veya .jpg olarak kaydedilebilir.
Yoğun grafik işlemi olan oyunlar için uygundur.
#SVG
Sayfayı yakınlaştırınca çözünürlük bozulmaz.
Çizim nesnelerine JavaScript olayı eklenebilir.
Çizim .png veya .jpg olarak kaydedilemez.
Yoğun grafik işlemi olan oyunlar için uygun değildir.



