---
layout: post
date: 2016-05-12
title: Tretie zadanie z webového publikovania
---
## Zadanie

Tretím projektom z webového publikovania bolo navrhnutie štruktúry jednoduchej prezentácie v  **XML** a vytvorenie transformácie do **XHTML**. Identifikujte základné súčasti prezentácie a navrhnite XML elementy pre ich označkovanie (metadátové, štrukturálne, inline).
Ďalej vytvorte ukážkovú prezentáciu, ktorá bude demonštrovať možnosti tvorby prezentácií podľa definície typu dokumentu.

## Použité elementy
- elementy na štandarné členienie textu ako napr. rozdelenie do kapitol `chapter`, a podkapitol pomocou `section`

```xml
<slide>
		<title>Obsah prezentácie</title>
		<toc />
</slide>
```

- tabuľka so zlúčenými riadkami pomocou atribútu `morerows`. Prílad: `<entry morerows="1">listdirs</entry>`
- vytvorenie indexu s dvoma úrovňami členenia. V texte som označil pojmy nasledovne:

```xml
<image>
	<source>img/server.png</source>
	<caption>Server MOD FMS5711</caption>
</image>
```

- elementy na vytovrenie indexu pojmov. V texte som pojem označil nasledovne:

```xml
<list type="disc">
	<item>
	  <para><bold>Dual Boot</bold> - server obsahuje záložný zavádzací program, ktorý sa spustí v prípade ak dôjde k chybe pri zavádzaní systému.</para>
	</item>
	<item>
		<para><bold>Auto Recovery - Auto Restart</bold> – ak pri prevádzke systému dôjde k závažnej chybe, systém sa automaticky reštartuje.</para>
	</item>
</list>
```
