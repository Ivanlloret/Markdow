Exercici GIT 4: Gestió de branques
=
*Per a realitzar aquests exercicis és necessari haver realitzat prèviament els exercicis sobre desfer canvis.*

Exercici 1
-
Crea una nova branca bibliografia i mostrar les branques del repositori. Git branch bibliografia

git checkout bibliografia

git branch

Exercici 2
-
1. Crear el fitxer capítols/capitol4.txt i afegir el següent text

nano capitols/capitol4.txt

2. Afegir els canvis a la zona d'intercanvi temporal.

git add capítols/capitol4.txt

3. Fer un commit amb el missatge "Afegit capítol 4. git commit -m "Afegit capítol 4"
3. Mostrar la història del repositori incloent totes les branques. git log --all --graph --decorate --oneline


Exercici 3
-
1. Canvia a la branca bibliografia. git checkout bibliografia
1. Crea el fitxer bibliografia.txt i afegir la següent referència: nano bibliografia.txt
1. Afegeix els canvis a la zona d'intercanvi temporal.

Git add bibligradia.txt

4. Fes un commit amb el missatge "Afegida primera referència bibliogràfica."

Git commit -m ‘Añadida pagina principal’

5. Mostra la història del repositori incloent totes les branques.

git log --all --graph --decorate --oneline

Exercici 4
-
1. Fusiona la branca bibliografia amb la branca master.

git checkout master

git merge bibliografia

2. Mostra la història del repositori incloent totes les branques.

git log --all --graph --decorate --oneline

3. Elimina la branca bibliografia.

git branch -d bibliografia

4. Mostra de nou la història del repositori incloent totes les branques.

git log --all --graph --decorate --oneline

Exercici 5
-
1. Crea la branca bibliografia.

Git branch bibliografia

2. Canvia a la branca bibliografia.

Git checkout bibliografia

3. Canvia el fitxer bibliografia.txt perquè continga les següents referències

nano bibliografia

4. Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica."

   git add bibliografia.txt

git commit -m "Afegida nova referència bibliogràfica."

5. Canvia a la branca master.

Git checkout master

6. Canvia el fitxer bibliografia.txt perquè continga les següents referències:

nano bibliografia

7. Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica."

   git add bibliografia.txt

git commit -m "Afegida nova referència bibliogràfica."

8. Fusiona la branca bibliografia amb la branca master.

Git merge bibliografia

9. Resol el conflicte deixant el fitxer bibliografia.txt amb les referències:

nano bilbliografia

10\.Afegeix els canvis a la zona d'intercanvi temporal i fes un commit amb el missatge "Resolt 

conflicte de bibliografia."

git add bibliografia.txt

git commit -m «Resolt conflicte»

11\.Mostra la història del repositori incloent totes les branques.

git log --all --graph --decorate --oneline

