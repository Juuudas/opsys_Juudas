1. Võrrelge Administrator ja SYSTEM privileege ning kirjutage vähemalt üks tegevus mille jaoks on vaja SYSTEM õigusi. <br>
**Vastus:** SeSystemProfilePrivilege <br>

2. Ekraanivaade turvalise kausta seadetest (ainult üks kasutaja saab teha kõike ja Ülemus ainult lugeda). <br>

<img src="https://i.imgur.com/icvFO3K.png" alt="oigused" width="1000"/>

3. Kirjuta praktikumi aruandesse vähemalt 3 soovitust (muudatust), mida Microsoft soovitab Windowsi turve seadete juures parandada, suurendamaks Windows operatsioonisüsteemi turvalisust. Vastus kirjutage võimalikult täpselt, kuid muudatusi endid pole vaja seadistada, sest osad neist pole laboritingimustes virtualiseeritud arvutis- võimalikud või mõistlikud. <br>
**Vastus:** Windows soovitab häälestada Lunavaratõrje Onedrives. Windows soovitab isoleerida tuumad. Veel soovitab windows turvalisuse huvides ja muude eeliste nägemiseks sisse logida Microsofti kontoga. <br>

4. Vali ise sobiv turvalisusaste ning põhjenda valikut praktikumi aruandes. <br>
**Vastus:** Valisin teavita mind alati, kuid ilma töölaua hämardamiseta, sest pean teavitusi siiski olulisteks, et säilitada arvuti turvalisus. 
Lisaks tahan, et saaksin teavitusi ka Windowsi sätete muutmisel, et olla veendunud siiski muudatuse läbiviimises. Töölaua hämardamine ei ole minu jaoks
vajalik. 

5. Vali veel vähemalt 3 Local Security Policy seadistust, mida tuleks muuta või üle vaadata, et tagada arvutis olevate andmete ja kasutajate isikuandmete kaitse. Põhjenda oma valikuid. <br>
**Vastus:** <br>
1. Password must meet complexity requirements - Enabled. Selleks, et kasutaja parool oleks turvaline ja teine töötaja seda hõöpsalt ära ei arvaks. <br>
2. Minimum password length - 8 characters. Sama põhjendus mis eelmisel. <br>
3. Interactive logon: Message text for users attempting to log on -	YOUR ACTIONS MAY BE AUDITED!. See on Selleks, et hoiatada/hirmutada töötajaid, et nende tegevus arvutis võib olla jälgitud. See tagaks turvalisema ja töökama keskkonna. <br>

6. Lisa vähemalt 2 ekraanivaatet erinevatest keeluteavituste ja Kasutajakonto kontrolli teavituste kohta. Pildiallkirjas märgi ära, mis kasutajana mis toimingut proovisid teha. <br>
Proovisin avada faili, mis kuulub teisele kasutajale.
<img src="https://i.imgur.com/QbM6YFA.png" alt="txt" width="1000"/>
Proovisin alla laadida Teamviewerit, mis polnud lubatud.
<img src="https://i.imgur.com/McBbbq5.png" alt="download" width="1000"/>
Proovisin alla laadida Teamvieverit, nüüd küsis Administraatori parooli.
<img src="https://i.imgur.com/95nagk4.png" alt="download_prompt" width="1000"/>

7.Esita ekraanivaade Event Vieweri aknast, kus on selgelt näha logikirje ebaõnnestunud sisselogimiskatse kohta. <br>
<img src="https://i.imgur.com/iRMuFMW.png" alt="download_prompt" width="1000"/>

8. Tehke ekraanivaade DisplayLastLogonInfo registrivõtmest koos väärtusega 1.
<img src="https://i.imgur.com/ibdEiAV.png" alt="download_prompt" width="1000"/>
