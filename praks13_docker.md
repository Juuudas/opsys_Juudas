SOOVISIN TEHA ANTUD PRAKTIKUMI ENDA ISIKLIKUS ARVUTIS, MIS JOOKSEB MACOS PEAL! :) 

1. Defineerige, mis on Dockerfile, Docker Image, Docker Container. Mis on neil vahet? 

Docker can build images automatically by reading the instructions from a Dockerfile. 
A Dockerfile is a text document that contains all the commands a user could call on the command 
line to assemble an image. This page describes the commands you can use in a Dockerfile.

**Vastus:** <br>
Dockerfile: Tekstifail, milles on kõikvõimalikud käsud, mida kasutaja saab välja kutsuda käsureal, et moodustada _image_. 
Docker saab automaatselt ehitada _image_ lugedes juhised Dockerfile'st. <br>
Docker Image: Fail, et käivitada koodi Docker Containeris. <br>
Docker Container: N-ö koht, kus aplikatsioon saab vabalt joosta. <br>

2. Tehke screenshot Docker ps väljundist, nii et oleks näha teie kasutajanimi. 

**Vastus:** <img src="https://i.imgur.com/NVWvhjc.png" alt="fstab" width="1000"/>

3. Tehke screenshot, kus on näha todo app jooksmas teie arvutis ja terminali aken koos teie kasutajanimega. 

**Vastus:** <img src="https://i.imgur.com/x9l7LiT.png" alt="fstab" width="1000"/>

4. Mis on "Sharing Our App" sammu mõte? Mida see samm demonstreerib? 

**Vastus:** Antud samm õpetas meid tegema Dockerisse repo ja seda jagama. 
Nii saame jagada oma image faile teistele kasutajatele, mille läbi nad saavad sama aplikatsiooni jooksutada.
Seda näiteks Docker Playgroundis. Seal saab valida porti ja selle seal portis avada. 

5. Tehke screenshot käsu 'docker inspect volume todo-db' väljundist. 

**Vastus:** <img src="https://i.imgur.com/jUlZDoE.png" alt="fstab" width="1000"/>

6. Tehke selgeks, millist docker konteksti te parasjagu kasutate? 

**Vastus:** Parasjagu kasutan default* konteksti.

