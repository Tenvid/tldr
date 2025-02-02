# magick convert

> ImageMagick Bildkonvertierungswerkzeug.
> Weitere Informationen: <https://imagemagick.org/script/convert.php>.

- Konvertiere ein Bild von JPEG nach PNG:

`magick convert {{pfad/zu/bild.jpg}} {{pfad/zu/bild.png}}`

- Skaliere ein Bild auf 50% seiner Originalgröße:

`magick convert {{pfad/zu/bild.png}} -resize 50% {{pfad/zu/bild2.png}}`

- Skaliere ein Bild unter Beibehaltung des ursprünglichen Seitenverhältnisses auf eine maximale Größe von 640x480:

`magick convert {{pfad/zu/bild.png}} -resize 640x480 {{pfad/zu/bild2.png}}`

- Hänge Bilder vertikal/horizontal aneinander:

`magick convert {{pfad/zu/bild1.png pfad/zu/bild2.png ...}} {{-append|+append}} {{pfad/zu/bild.png}}`

- Erstelle ein animiertes GIF aus einer Serie von Bildern mit einer Verzögerung von 100 ms zwischen den Bildern:

`magick convert {{pfad/zu/bild1.png pfad/zu/bild2.png ...}} -delay {{10}} {{pfad/zu/animation.gif}}`

- Erstelle ein Bild mit nichts als einem festen Hintergrund:

`magick convert -size {{800x600}} "xc:{{#ff0000}}" {{pfad/zu/bild.png}}`

- Erstelle ein Favicon aus mehreren Bildern verschiedener Größe:

`magick convert {{pfad/zu/bild1.png pfad/zu/bild2.png ...}} {{pfad/zu/bild.ico}}`
