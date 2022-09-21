# opsys_Juudas

1. Mitu protsessi kokku arvutis käib?



2. Milline on kõige esimesena käivitatud protsess? (lisalugemine: init vs systemd)



3. Milliste kasutajate protsesse arvutis käib? (arvesta ka süsteemiprotsesse, mitte ainult sisse logitud kasutajaid ehk teisisõnu küsime mitme erineva kasutaja õigustes protsesse arvutis käib? )



4. Kui kaua on arvuti järjest töötanud (up time) ? (Alternatiivselt võib vastata ka millal (kuupäev ja kellaaeg) arvuti viimati käima pandi?)?



5. Milline protsess käivitati kõige hiljem (viimasena)? (Mitte võtta arvesse programmi, millega seda infot otsida.)



6. Milline on kõige rohkem protsessoriaega võttev protsess?



7. Milline on kõige rohkem virtuaalmälu (aadressiruumi, commit, Virtual Size) võttev protsess?



8. Milline on kõige rohkem füüsilist mälu (working set) võttev protsess?



9. Kui palju füüsilisest mälust (Physical Memory) on vaba?



10. Kui palju on põhikettal (C:, /) vaba ruumi mahult (GB) ja protsentuaalselt?



11. Milline on kõige suurem kõvakettal olev fail ja kõige suurem kaust?



12. Võrrelge terminali käskude: sha1sum /dev/zero | sha1sum /dev/zero ja sha1sum /dev/urandom | sha1sum /dev/urandom protsessori nõudlust. Avage teine terminaliaken ja top samaaegseks käivitamiseks. Uurige millisele CPU alamtegevusele us, sy, id, wa, st jne kulub enim protsessori aega ja mitu protsenti kulub kummagi käsu korral? (Ainult Linuxis) Lisa ka ekraanipilt aruande juurde näiteks pärast tabelit.



13. Milline protsess kõige rohkem salvestusseadmele kirjutab, kõige rohkem salvestusseadmelt loeb? Millisesse faili antud protsess kõige rohkem kirjutab, millisest failist kõige rohkem loeb? (Ainult Windowsis)



14. Millise protsessi poolt tekitatud võrguliiklus on suurima mahuga? Vali antud protsessi poolt kasutatavatest ühendustest üks ning kirjuta välja järgnev: kahalik IP-aadress, kohalik port, ühenduse teise poole IP-aadress, port, latents ja antud ühenduse poolt kasutatav võrguliikluse kogumaht. (Ainult Windowsis) Lisa ka ekraanipilt aruande juurde näiteks pärast tabelit.



15. Sõber kurdab, et tema arvuti on oluliselt aeglasem kui varasemalt. Millise programmiga ja millise parameetrite abil saate tuvastada milline protsess või teenus muudab arvuti aeglaseks?
