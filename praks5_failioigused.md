1.  Missuguseid õigusi (r,w,x) on Unixis omanikul minimaalselt vaja (`d`  - directory,  `f`  - fail)
    -   a) kataloogile  `/d`  faili  `/d/f`  lugemiseks ning <br>
		    **Vastus:** r,x
    -   b) failile  `/d/f`  faili  `/d/f`  lugemiseks <br>
		    **Vastus:** r
    -   c) kataloogile  `/d`  faili  `/d/f`  kustutamiseks <br>
		    **Vastus:** w
    -   d) failile  `/d/f`  faili  `/d/f`  kustutamiseks? <br>
		   **Vastus:** w
		   
2.  Miks  `chmod a=x skriptifail`ei ole piisav õigus shelli skriptifaili käivitamiseks? Millist õigust lisaks käivitamis-õigusele veel vaja läheb shelli skripti käivitamiseks? Põhjendage lühidalt? <br> <br>
 **Vastus:** chmod a=x skriptifail eemaldab skriptifaililt vaikimisi olevad r,w õigused, mis on vajalikul skriptifaili käivitamiseks. Õigem oleks kasutada a+x, mis lisab vaikimisi r,w juurde ka x õiguse.
 
3.  Milleks on kasulik see, et igal kasutajal on omanimeline grupp? (teema: umask lõpp) <br> <br>
**Vastus:** See suurendab turvalisust, kui saame reguleerida, kas faili saab lugeda/kirjutada ainult *owner, group* või *others*. Kasutajatel on määratud umask, mis muudab failiõigused vastavalt faili tehes. Nii saame vältida näiteks, et tiimikaaslane ei saaks muuta privaatseid faile.

4.  Milliseid on minimaalsed õigused (rwx), mis on vajalikud teie tavakasutajal (kuulub gruppi majasisene) (mitte  `root`  või  `peeter`  kasutajal, kausta ja faili omanikud)  `uusfail.txt`  sisu kuvamiseks. Esita ekraanivaade  `id`,  `ls -la`  ja  `cat uusfail.txt`  käskude väljundist tõestamaks lahendust.
<br> <br> **Vastus:** Vajalik on r
<img src="https://i.imgur.com/nO4hs0M.png" alt="Proof" width="600"/>

6.  Tehke screenshot tulemusest, kus oleks näha  `hinded.txt`  failiõigused  `ls -la hinded.txt`  ja jukuisa käivituskäsk koos väljundiga ning lisage see oma viki lehele. (teema:  `setuid`  ja  `setgid`.)
<br> <br> **Vastus:** Lisasin alguses setuid ka hinedJukul.c failile, mitte kohe hindedJukul. See tulemust ei paistnud muutvat.

<img src="https://i.imgur.com/y4bVt9g.png" alt="opetaja" width="600"/>

<img src="https://i.imgur.com/xeKqJia.png" alt="jukuIsa" width="600"/>


<br> <br> 7.  Kas  `setuid`  või  `setgid`  kasutamine võib vähendada süsteemi turvalisust? Kui  `JAH`, siis kuidas? kui  `EI`, siis miks ei vähenda?
<br> <br> **Vastus:** Jah, sest see annab teistele faili jookustamise õigused teise kasutaja alt. 
<br> <br> 8.  Kirjutage oma viki lehele kõik kasutajaid, kes saavad  `sticky bit`  õigustega  `yhiskaust`  kataloogist nüüd  `peeter`kasutaja loodud faile kustutada. (teema: sticky bit)
<br> <br> **Vastus:** Ainult õpetaja.
<br> <br> 9.  Uurige käsuga  `ls -la`  faili  `hinded.txt`  õigusi - mida märkate? Seejärel uurige õigusi täpsemalt, kasutades käsku  `getfacl`  ning kopeerige see tulemus oma vikilehele. (teema: ACL)
<br> <br> **Vastus:** # file: hinded.txt
owner: opetaja
group: opetaja
user::rw-
group::---
group:direktor:rw-
mask::rw-
other::---

<br> <br> 10.  Kes saab  `chattr +i`  parameetriga faili sisu modifitseerida (kirjutada)? Milliste käskudega saate kustutada  `testfail-2`nimelise  `+i`  parameetriga faili.
<br> <br> **Vastus:** `chattr +i` parameetriga ei saa mitte keegi faili sisu modiftiseerida. M Kustutamiseks on vaja samamoodi kõigepealt eemalda chattr *immutable* atribuut käsuga `sudo chattr -i testfail-2`. Seejärel kustutamiseks `rm testfail-2`.
