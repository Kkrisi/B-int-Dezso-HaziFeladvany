Az IP-cím (Internet Protocol-cím) egy egyedi (hálózati) azonosító, amelyet az internetprotokoll segítségével kommunikáló számítógépek egymás azonosítására használnak.



Röviden:

Az eszküzönk ip címet kér, mert addig semmi másra nem képes amig nem rendelkezik ip címmel. 
Ezt a kérést a forgalomirányítónak küldi tovább. 
Ami keres egy rendelkezésre álló IP-címet, majd hozzárendeli a kért eszközhöz. 
Így a kapott ip címmel az eszköz képes lesz kommunikálni a hálózaton.
(amely cím később beleépül a forgalomirányitó  routing táblájába)


Hosszabban:

A kliens kiküld egy DISCOVER csomagot amivel a DHCP szervert keresi.
Ha a DHCP szerver megkapta a DISCOVER csomagot, akkor visszajelez egy OFFER csomaggal, amivel ugymond ajánlatot tesz a kliensnek.
Az eszköznek most válaszolnia kell a kiszolgálóra egy REQUEST nevű csomaggal, a választott IP-cím elfogadásával. Ehhez a csomaghoz a szerver nyugtázást (ACK) küld, amely megerősíti, hogy az eszköz megkapta és használja a kapott címet.


