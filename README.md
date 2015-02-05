## ingress-shaper-glyphs

한글 설명 추가본
www.memrise.com에는 한글로 설명된 glyph 목록이 없어서 일본어판 크롤링 데이터를 기반으로 한글 데이터를 작성했습니다.
https://docs.google.com/spreadsheets/d/1DGZ9TuHKNSFdavcF3aNKF56mEvEgNY7hAUeQ3jFPhNM/edit?usp=sharing
이후 위 스프레드시트에 작성된 값을 적용합니다.

생각나면 할거
json 파싱하지 않고 딕셔너리로 바로 만들기..?


Source data for memrise courses on [Ingress][ingress] Shaper glyphs.

- English: http://www.memrise.com/course/368204/ingress-shaper-glyphs/
- Japanese: http://www.memrise.com/course/369242/ingress/

[ingress]: https://www.ingress.com

### Commands

- `gulp course-data`: generates `dist/*.tsv` and `dist/images/*.png` files suitable for uploading with [Uprise][uprise].
- `gulp course-logo`: generates `dist/course-logo.png`.

[uprise]: http://memrise-users.wikia.com/wiki/Uprise

### How to run locally

Clone and execute:

```
$ npm install
```

If ``node-canvas`` is having trouble finding headers from X11, try:

```
PKG_CONFIG_PATH=/opt/X11/lib/pkgconfig/ npm install --save canvas
```

### Note about the "code" column

This column unambiguously identifies a glyph. The format follows the [node numbering scheme used by Ingress glyph tools][node-numbering].

[node-numbering]: https://github.com/gm9/ingress-glyph-tools/blob/master/glyph-tools.js#L205


### Glyph and glyph name sources

- [Glyphtionary](http://glyphtionary.com/)
- [Ingress glyph tools](https://github.com/gm9/ingress-glyph-tools)
- [Glypher](https://play.google.com/store/apps/details?id=com.dmidroid.ingress.glyphs)


---- 

Niantic Labs has the authority on glyph names and imagery. Other portions of this repo are released under the MIT license.
