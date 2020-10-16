# Contributing

* Forkati orginalni repository na organizaciju (neko od administracije će obaviti ovo)
* Preimenovati forkan repository: `Naziv_Predmeta-Seminarski-Naziv_Seminarskog-Broj_Seminarskog` (broj seminarskog dodati samo u slučaju više seminarskig radova sa istim nazivom)
* Otvoriti issue `New Entry` i navesti sve informacije

# Kako prebaciti repository sa Azura DevOpsa na Github

1. Kreirati repository na githubu

2. Klonirati repository

```
git clone https://fitbaXXXX@dev.azure.com/fitbaXXXX/seminarski_rad/_git/webapp
cd webapp
```

3. Ukloniti remote na repository sa Azure DevOpsa
```
git remote remove origin
```

4. Dodati remote origin na Github repository
```
git remote add origin https://github.com/Username/Repository-Name
```

5. Push kod na github
```
git push -u origin master
```

## Opcionalno dodati dokumentaciju kao novi branch


1. Kreirati novi branch i ukloniti sve fajlove

```
git checkout --orphan dokumenti
git rm --cached .
rm -rf *
```

2. Dodati remote na repository sa dokumentacijom

```
git remote add origin https://fitbaXXXX@dev.azure.com/fitbaXXXX/seminarski_rad/_git/dokumenti
```

3. Pull dokumenti remote sa Azure DevOpsa
```
git pull dokumenti master
```

4. Push dokumenti na Github
```
git push origin dokumenti
```
