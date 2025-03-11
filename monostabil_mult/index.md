# Jegyzőkönyv

## Kísérlet címe
Monostabil multivibrátor építése NI myDAQ és breadboard segítségével

## Kísérlet célja
Az 555-ös időzítő IC felhasználásával egy monostabil multivibrátor áramkör építése, amely egy LED-et kapcsol be egy gombnyomás hatására meghatározott időtartamra.

## Felhasznált eszközök és alkatrészek
- NI myDAQ
- Breadboard
- 555 időzítő IC
- LED
- Nyomógomb
- Ellenállások:
  - 12 kΩ (2-es láb és gomb között)
  - 1 MΩ (7-es és 4-es láb között)
  - 220 Ω (LED védelmére)
- Kondenzátor:
  - 10 µF (6-os lábra kötve)
- Tápfeszültség:
  - 5V a 8-as lábra kötve

## Kapcsolási rajz:

[A kapcsolási rajz](https://www.falstad.com/circuit/e-555monostable.html)  

---

## Kapcsolási rajz megvalósítása:

![IMG_6808](https://github.com/user-attachments/assets/54bcad00-9667-4acf-9a86-2059294a268e) 
![IMG_6806](https://github.com/user-attachments/assets/01162248-b344-4987-9343-cc0ed0f6ce77)

---

## Működés leírása
A nyomógomb lenyomásakor az 555-ös IC 3-as kimenete magas szintre vált, és a LED világítani kezd. A LED körülbelül 22 másodpercig világít, majd automatikusan kikapcsol. Az időzítést a 10 µF-os kondenzátor és az 1 MΩ-os ellenállás** határozza meg a következő képlet alapján:
A mért érték 22 másodperc, ami a komponensek tűréshatárából adódhat.

## Mérések és tapasztalatok
- A LED megfelelően működött, és a kapcsolási idő közel állt az elméletileg számított értékhez.
- Az áramkör stabilan üzemelt, nem tapasztaltunk jelentős feszültségeséseket vagy kapcsolási hibákat.
- A myDAQ segítségével az áramkör bemeneti és kimeneti feszültségeit mértük és dokumentáltuk.
