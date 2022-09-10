Az IP-cím (Internet Protocol-cím) egy egyedi (hálózati) azonosító, amelyet az internetprotokoll segítségével kommunikáló számítógépek egymás azonosítására használnak. Minden, az internetre kapcsolt számítógépnek van IP-címe, de egy-egy konkrét cím nem kötődik feltétlenül egy-egy géphez.



Az útválasztónak kell eldöntenie, hogy egy adott csomagnak merre kell tovább mennie. Ebben a feladatban rendelkezésre áll a cél IP cím, ill. egy belsõ táblázat, a routing tábla.

Minden egyes hálózati eszköz kap egy IP címet, tehát ha a routerünknek két interface-e van, akkor neki két IP hálózatra van kijárása, számára két szegmensen is vannak közvetlenül elérhetõ hostok.

Így a routerünk meg tudja címezni mindkét IP szegmenst valamelyik eszközén  keresztül. A megfelelõ eszköz keresése valahogy úgy zajlik, hogy az elsõ olyan routing bejegyzés eszköz mezõje hivatkozik a keresett eszközre, aminek a tartományába a célcím beleesik.
Van egy harmadik oszlop, ami a fenti két bejegyzésnél üres. Ezt az oszlopot használhatjuk fel annak megjelölésére, hogy a célcím nem lokálisan elérhetõ, de az adott szegmensen található gateway már tudja az utat a cél felé. Ilyen módon a gateway-ek összeláncolhatók.

Ilyen módon épül fel az egész internet, minden kis helyi hálózat továbbitja a nem helyi packeteit egy olyannak, aki már tudja merre kell azt továbbítani.

A hálózaton nem csak a host-okat (számítógépeket, munkaállomásokat) azonosítják IP címmel, hanem a hálózatokat is. Egy IP szegmenst a network címe azonosít. Egy host neve úgy áll össze, hogy a cím elején levõ bitek határozzák meg a hálózat címét, a fennmaradó bitek pedig a host-ot azonosítják a hálózaton belül. Az, hogy melyik rész a network cím, és melyik azonosítja a host-ot a netmask határozza meg.
A címnek azon bitjei, amiken a netmask bitjei 1-et tartalmaznak, a network címet határozzák meg, a fennmaradó bitek pedig a network-ön belüli hostcímet adják meg.
