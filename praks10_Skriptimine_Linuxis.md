**Ülesanne 3.** 
```Script
#!/bin/sh
echo "Sisesta nimi:"
read nimi
echo "Sisesta eriala:"
read eriala
echo "Sisesta matrikli number:"
read matrikkel
echo "Sisestati: $nimi $eriala $matrikkel"
```

**Ülesanne 4.** 
```
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

**Ülesanne 5.** 

```
#!/bin/bash
IFS=$'\n'
nimi=$1
for line in $(ps -A | grep -w $nimi)
do
    echo " "$line | tr -s ' ' | cut -d ' ' -f2,5
done

```

**Ülesanne 6.** 
```
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
