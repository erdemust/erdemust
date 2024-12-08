# SVG

Simple overview of use/purpose.

## Description

An in-depth paragraph about your project and overview of use.

## Getting Started

### Dependencies

* Describe any prerequisites, libraries, OS version, etc., needed before installing program.
* ex. Windows 10

### Installing

* How/where to download your program
* Any modifications needed to be made to files/folders

### Executing program

* How to run the program
* Step-by-step bullets
```
code blocks for commands
```

## Help

Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

Contributors names and contact info

ex. Dominique Pizzie  
ex. [@DomPizzie](https://twitter.com/dompizzie)

## Version History

* 0.2
    * Various bug fixes and optimizations
    * See [commit change]() or See [release history]()
* 0.1
    * Initial Release

## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details

## Acknowledgments

Inspiration, code snippets, etc.
* [awesome-readme](https://github.com/matiassingers/awesome-readme)
* [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
* [dbader](https://github.com/dbader/readme-template)
* [zenorocha](https://gist.github.com/zenorocha/4526327)
* [fvcproductions](https://gist.github.com/fvcproductions/1bfc2d4aecb01a834b46)


HTML5 ile birlikte gelen özelliklerden birisi olan SVG dili ile ilgili bilgiler SVG kullanımı ve SVG örnekleri yer alıyor.

SVG nedir
SVG açılımı Scalable Vector Graphics ( Ölçeklenebilir Vektörel Grafikler )
Web sayfalarında grafik oluşturmak için kullanılır.
HTML geliştiricileri tarafından önerilir
JavaScript kullanımına ihtiyaç yoktur.
HTML5 <svg> etiketi SVG grafikleri için taşıyıcı görevi görür.

SVG etiketi ile çizgi, dikdörtgen, çember, daire vb. çizim yöntemleri vardır.
```
code blocks for commands


SVG çember ve daire çizmek
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
```<svg width="400" height="180">
  <rect x="50" y="20" rx="20" ry="20" width="150" height="150"
  style="fill:blue;stroke:black;stroke-width:5;opacity:0.5" />
</svg>
 
```


SVG polygon yıldız
<svg width="300" height="200">
  <polygon points="100,10 40,198 190,78 10,78 160,198"
  style="fill:lime;stroke:purple;stroke-width:5;fill-rule:evenodd;" />
</svg>
SVG örnek
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
SVG ve Canvas arasındaki farklar
SVG XML tabanlı grafik çizimi için kullanılan bir dildir.

Canvas JavaScript ile grafik çizimi yapmak için kullanılan bir etikettir.

SVG XML tabanlı olduğundan SVG etiketlerine JavaScript DOM ile olay (tıklama, üzerine gelme vb.) ekleyebiliriz.

SVG ve Canvas karşılaştırması
Canvas	SVG
Sayfayı yakınlaştırınca çözünürlük bozulur.
Çizim nesnelerine JavaScript olayı eklenemez.
Çizim .png veya .jpg olarak kaydedilebilir.
Yoğun grafik işlemi olan oyunlar için uygundur.
Sayfayı yakınlaştırınca çözünürlük bozulmaz.
Çizim nesnelerine JavaScript olayı eklenebilir.
Çizim .png veya .jpg olarak kaydedilemez.
Yoğun grafik işlemi olan oyunlar için uygun değildir.



