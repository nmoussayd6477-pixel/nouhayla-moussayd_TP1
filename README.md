# nouhayla-moussayd_TP1
mon premier projet

###EXERCICE 1:
```
ALGORITHME PIN

  VAR PIN,cont:entier
      const=2456
Debut
    cont←0
    repeter
      ecrire(" donnez un code pin" )
      lire(PIN)
      cont←cont+1
      si PIN =const alors
        ecrire("succés")
      sinon
        si const=PIN alors
         ecrire("erreurs")
        sinon
         si(cont=3 et PIN= const)alors
           ecrire("blocage")
         finsi
        finsi
      finsi
    Jusqu'à(PIN=const ou cont=3)
FIN
La complixité est 26
```

###EXERCICE 2:
```
ALGORITHME ECHANGE
  VAR NBR1,NBR2,NBR3:réels
Debut
    ecrire("saisir deux variables")
    lire(NBR1,NBR2)
    NBR3←NBR1
    NBR1←NBR2
    NBR2←NBR3
    ecrire("NBR=",NBR1,"NBR2=",NBR2)
FIN
la complixité est 9
 ```
 ###EXERCICE 3:
 ```
 1_ALGORITHME PGCD
     VAR NBR1,NBR2,REST:entier
Debut
    ecrire("donnez  deux nomdres:")
     lire(NBR1,NBR2)
    Tant que NBR2 !=0 faire:
       REST←NBR1 mod NBR2
       NBR1←NBR2
       NBR2←REST
    Fin tant que
    la complixité est 4n+5
2_ALGORITHME PGCD
    VAR NBR1,NBR2:entier
    fonction pgcd(chiff1:entier,chiff2:entier)
      si NBR2=0 alors
        retourner NBR1
      sinon
        retourner pgcd(chiff2,chiff1 mod chiff2)
      finsi
    fin fonction
Debut
     ecrire("donnez deux nombres")
     lire(NBR1,NBR2)
     ecrire("le pgcd est",pgcd(NBR1,NBR2))
FIN
la complixité est n+5
  ```
  ###EXERCICE 4
  ```
  ALGORITHME DIVESEUR
    VAR CHIFFRE:entier
    fonction affichdivm1( nbr:entier):entier
      VAR b:entier
      pour b de 1 à nbr faire
        si (nbr mod b=0) alors
          retourner b
        finsi
    fin pour
    fin fonction
    fonction affichdiv2(nbr:entier):entier
      VAR D:entier
      pour D de 1 à racincarre(nbr) faire
         si nbr mod D=0 alors
           ecrire(D)
           retourner nbr/D
         finsi
      fin pour
    fin fonction
    Debut
      ecrire(" saisir un nombre")
      lire(chiffre)
      ecrire(" les diviseurs par la premier méthode",affichdiv1(chiffre))
      ecrire(" les diviseurs par la deuxiéme méthode",affichdiv2(chiffre))
    fin
```
### EXERCICE 5
```
ALGORITHME DEVINERNOMBRE
   VAR nombre1, nombre2,tent:réels
Debut
     nombre1←47
     tent←0
     pour i de 1 à 5 faire
        ecrire(" saisir un nombre entre 0 et 100")
        lire(nombre2)
        si nombre1=nombre2 alors
           ecrire(" BRAVO!,le nombre est correct")
        sinon
           si nombre2<nombre1 alors
              ecrire("trop petite")
           sinon
              ecrire(" trop grand")
        finsi
        si tent=5 alors
           ecrire(" le nombre correct est",nombre1)
        finsi
     fin pour
FIN
la complixité est 24

```
###EXERCICE 6
```
ALGORITHME TRIANGLE 
  VAR nbr, i, j :entier
Debut
    ecrire(" choisir un nombre")
    lire(nbr)
    pour i de 1 à nbr faire
       pour j de 1 à i faire
         ecrire(nbr)
        fin pour
      ecrire( )
    fin pour
FIN

```
EXERCICE 7
```
ALGORITHME SOMME 
    VAR nbr, som: entier 
Debut
       ecrire(" donner  un nombre")
       lire(nbr)
       som←0
       pour i de 1 à nbr faire 
          som←som+i
       fin pour
       ecrire( " la somme égale à",som)
FIN
la complixité est 2n+4
```
###EXERCICE 7
```
ALGORITHME SOMME 
    VAR nbr, som: entier
    Fonction somme(nombre: entier):entier
        si (nombre= 1) alors
           retourne nombre
        sinon
           retourne n+somme(nombre-1)
        finsi
    fin fonction
Debut
   ecrire (" donner un nombre")
   lire(nbr)
   som←somme(nbr)
   ecrire("la somme est",som)
Fin
la complixité est 2n+3
```


          













   



