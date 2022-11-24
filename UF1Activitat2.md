# PRACTICA AMB LLENGUATGES
Activitat 2 realitzada per Jan PLata i Sergi Camps


## Llenguatge Interpretat
Com a llenguatge interpretat ens ha tocat realitzar un dau de 6 cares utilitzant R desde la línia de comandes.

### Descripció de l'intèrpret
A l'interior del fitxer ens trobem aixó

![image](https://user-images.githubusercontent.com/113586164/194003549-84342f79-2ac4-4c91-a787-fb122bb60e77.png)

 #### El sample(1:6, 1):
 El 1:6 es el rang de nombres que surtiran aletoriament
 
 El 1 es la quantitat de nombres aleatoris que sortiran cada vegada que executem el programa,en aquest cas 1.
 
 ### L'executable
 
 En primer lloc hem de instalar el paquet
 
 ![image](https://user-images.githubusercontent.com/113586164/194004773-26fba62f-df03-4a9b-b399-1413ded59ec8.png)

El Rscript es l'executable del llenguatge R per a que fagi corre els programas

![image](https://user-images.githubusercontent.com/113586164/194005096-932d7106-2b07-4c1c-8517-2c88d49caf05.png)

### Extensions del codi font

La extensio .R es la que s'utiltza en aquest cas

![image](https://user-images.githubusercontent.com/113586164/194005703-ee088435-aac4-4601-8ad4-ca5e0aa602ef.png)

### Avantatges i desaventatges dels llenguatges interpretats

#### Avantatges

Es multiplataforma, ja que, l'interpet sol estar en varis sistemes operatius

Es pot portar a diferents plataformes

Al poder executarse en el navegador client, disminueix la carga de treball del servidor web aumentant aixiques el seu rendiment

#### Desaventatges

A la hora de l'execució del programa, quan compilam el transformam a codi màquina i això fa que baixa la velocitat de l'execució

Aunque sigui multiplataforma, si la màquina no te l'interpret no funcionara

### IDE de desenvolupament

Visual Studio code, RStudio i Geany

## Llenguatge Compilat ( Java )
Hem escollit Java com a llenguatge compilat ja que es un llenguatge amb el que no estem
familiaritzats i ens serà útil saber quant més millor sobre el seu funcionament/sintaxi.
### Compilant Java amb javac
He instalat javac, un compilador bastant senzill que s'utilitza de la següent forma:
![image](https://user-images.githubusercontent.com/96839905/194018723-727b5315-681f-4
b9d-bc60-ef6baf647cd7.png)
Per a passar el codi font a codi d'objecte només tindrem que executar l'arxiu amb javac,
cosa que creará l'arxiu class a partir del codi font.
Extensions dels fitxers de codi font i objecte:
![image](https://user-images.githubusercontent.com/96839905/194020406-b906b9cf-c92c-4
9b1-8572-a18c51b65d4f.png)
## Exemple de codi
Programa de dau de 6 cares amb Java (he fet servir nano per escriure el codi desde la
terminal)
```// Inici del programa, logica y declaració de variables:
public class java6 {
public static void main(String[] args) {
int dau = (int) Math.floor(Math.random()*6 + 1);
// math random genera un número entre 0 i 6 aquest no inclós ( per això el +1 final) i
desprès math floor s'arrodoneix els decimals del resultat a la baixa (de forma que no podem
obtenir un 7 si surt mes de 6.5).
// Output de dades
System.out.println("Resultat de la cara obtinguda: ");
;
// Switch per al resultat del math random/floor (resultat del dau)
switch (dau) {
case 1:
System.out.println("T'ha tocat el número \"un\".");
break;

case 2:
System.out.println("T'ha tocat el número \"dos\".");
break;
case 3:
System.out.println("T'ha tocat el número \"tres\".");
break;
case 4:
System.out.println("T'ha tocat el número \"quatre\".");
break;
case 5:
System.out.println("T'ha tocat el número \"cinc\".");
break;
case 6:
System.out.println("T'ha tocat el número\"sis\".");
break;
default:
System.out.println("Número no disponible al dau >:(");
}
}
}
```
## Avantatges de fer servir un llenguatge compilat
## IDE's per a desenvolupament amb java
