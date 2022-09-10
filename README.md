Az IP-cím (Internet Protocol-cím) egy egyedi (hálózati) azonosító, amelyet az internetprotokoll segítségével kommunikáló számítógépek egymás azonosítására használnak.


Minden egyes hálózati eszköz kap egy IP címet, tehát ha a routerünknek két interface-e van, akkor neki két IP hálózatra van kijárása, számára két szegmensen is vannak közvetlenül elérhetõ hostok.


amely később beleépük a forgalomirányitó  routing táblájába
Az útválasztónak kell eldöntenie, hogy egy adott csomagnak merre kell tovább mennie. Ebben a feladatban rendelkezésre áll a cél IP cím, ill. egy belsõ táblázat, a routing tábla.



Egy nagyon rövid összefoglaló arról, hogy mi történik a folyamatban:

Az ügyfél IP-címet kér a gazdagépről. Az ügyfél bármilyen eszköz lehet, amely elküldi a kérelmet, és a gazdagép lehet egy útválasztó.
A gazdagép megkeresi a rendelkezésre álló IP-címet, és hozzárendelte azt az ügyfélhez.
Ezen IP-cím használatával az ügyfél képes lesz kommunikálni a hálózaton.


Most nézzük meg részletesebben ezt a folyamatot. Az alább említett lépések mélyreható képet adnak róla -

A DHCP-kiszolgálóval hálózathoz csatlakoztatott eszköz által küldött kérést DHCPDISCOVER-kérelemnek hívják.
Ezt a kérést a DHCP szervernek DISCOVER nevû csomag formájában küldjük el. Amint ezt a csomagot megkapja a DHCP szerver, a szerver megkeresi az eszköz használatához egy IP címet. Miután megtalálta, a kiszolgáló válaszol, küldve egy csomagot a DHCPOFFER nevû kliensnek.
Az eszköznek vagy az ügyfélnek most válaszolnia kell a kiszolgálóra egy DHCPREQUEST nevű csomaggal, a választott IP-cím elfogadásával. Ehhez a csomaghoz a szerver nyugtázást (ACK) küld, amely megerősíti, hogy az eszköz mostantól képes használni az adott IP-címet. Azt is megadja az adott IP-cím érvényességét, hogy az eszköz pontosan tudja, mikor kell új IP-címet szereznie.
Azokban az esetekben, amikor a szerver nem akarja, hogy az eszköz megkapja az adott IP-címet, NAC elküldésével nem ismeri el az eszköz kérését.
Bár az említett lépések nagyon hosszú időt vesznek igénybe, ám ezek gyakorlatilag olyan gyorsan megtörténnek, hogy az még csak nem is valósul meg. Természetesen nincs szükség technikai részletekre a folyamatról, és még mindig elolvashatja az IP-címet a DHCP szerverről.


