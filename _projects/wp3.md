---
layout: post
date: 2016-04-10
title: Tretie zadanie z webového publikovania
---
## Zadanie

Druhým projektom z webového publikovania bolo spracovanie mojej bakalárskej práce z pôvodného dokumentu do do formátu **DocBook** a vygenerovanie cieľového tvaru v **PDF**.

## Použité elementy
- elementy na štandarné členienie textu ako napr. rozdelenie do kapitol `chapter`, a podkapitol pomocou `section`
- elementy na zvýraznenie slov tučným písmom `<emphasis role="bold">Last Good</emphasis>`
- členenie textu odrážkami pomocou `<itemizedlist mark="opencircle">`
- odkazy na iné kapitoly v domumente `<xref linkend="KAP2-1" />`
- poznámka pod čiarou s linkom `<footnote><para><ulink url="https://www.java.com"></ulink></para></footnote>`
- vygenerovaný zoznam použitej literatúry a citácia zdrojov pomocou `<citation>SOCKET</citation>`
- obrázky ako napríklad

```xml
<figure id="OBR1" xreflabel="Obrázku 1">
  <title>Server MOD FMS5711</title>
  <mediaobject>
    <imageobject role="fo">
      <imagedata fileref="img/server.png" format="PNG" width="400px" />
    </imageobject>
    <textobject><phrase></phrase></textobject>
  </mediaobject>
</figure>
```

- tabuľka so zlúčenými riadkami pomocou atribútu `morerows`. Prílad: `<entry morerows="1">listdirs</entry>`
- vytvorenie indexu s dvoma úrovňami členenia. V texte som označil pojmy nasledovne:

```xml
<figure id="OBR1" xreflabel="Obrázku 1">
  <title>Server MOD FMS5711</title>
  <mediaobject>
    <imageobject role="fo">
      <imagedata fileref="img/server.png" format="PNG" width="400px" />
    </imageobject>
    <textobject><phrase></phrase></textobject>
  </mediaobject>
</figure>
```

- elementy na vytovrenie indexu pojmov. V texte som pojem označil nasledovne:

```xml
<indexterm>
  <primary sortas="adresa">adresa</primary>
  <secondary>MAC</secondary>
</indexterm>
```
