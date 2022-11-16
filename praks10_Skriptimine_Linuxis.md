**Ülesanne 3.** 
```bash
#!/bin/sh
echo "Sisesta nimi:"
read nimi
echo "Sisesta eriala:"
read eriala
echo "Sisesta matrikli number:"
read matrikkel
echo "Sisestati: $nimi $eriala $matrikkel"
```
<img src="https://i.imgur.com/pSQ8WBR.png" alt="fstab" width="600"/>

**Ülesanne 4.** 
```bash
#!/bin/bash
laiend1=$1
laiend2=$2
for i in $(ls)
do
    if [ ${i##*.} = $laiend1 ]
    then
    fail=$i; mv $fail $(echo $fail | sed -e s/$laiend1/$laiend2/g)
    fi
done
```
<img src="https://i.imgur.com/xei8R8O.png" alt="fstab" width="600"/>

**Ülesanne 5.** 

```bash
#!/bin/bash
IFS=$'\n'
nimi=$1
for line in $(ps -A | grep -w $nimi)
do
    echo " "$line | tr -s ' ' | cut -d ' ' -f2,5
done

```
<img src="https://i.imgur.com/HVdl0Mg.png alt="fstab" width="600"/>

**Ülesanne 6.** 
```bash
#!/bin/bash
astenda () {
mitu=$2
a=$1
while [ $mitu -gt 1 ]
do
  let a=a*$1
  let mitu-=1
done
  echo $a
}

vastus=$(astenda 9 5)
echo "Vastus on: " $vastus

```
<img src="https://i.imgur.com/fErphZy.png" alt="fstab" width="600"/>
