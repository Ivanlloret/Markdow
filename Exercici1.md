Exercici GIT 1: Creació i actualització de repositoris
=

*Indica els comandaments amb els quals resoldries els escenaris plantejats en els diferents exercicis.
Exercici 1
-

Crea un repositori nou amb el nom llibre i mostrar el seu contingut. 
mkdir llibre
git init llibre 
cd llibre

Configura Git definint el nom de l'usuari, el correu electrònic i activar l'exida en color. Mostrar la configuració final. 
git config --global ivan.name "IvanLloret"
git config --global ivan.gmail "ivanlloretbor@gmail.com"
git config --global color.ui true
git config --global --list

Exercici 2
-
Comprova l'estat del repositori.

Crea un fitxer índex.txt amb el següent contingut
nano index.txt

Comprova de nou l'estat del repositori.
git status

Afegeix el fitxer a la zona d'intercanvi temporal. 

Tornar a comprovar una vegada més l'estat del repositori.
git add index.txt
git status

Exercici 3 
-

Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i veure l'estat del repositori.
git commit -m "Afegit index al llibre"
git status

Exercici 4
-

Canvia el fitxer índex.txt perquè continga el següent:

Mostra els canvis respecte a l'última versió guardada al repositori.

Fer un commit dels canvis amb el missatge "Afegit capítol 3 sobre gestió de branques".
git diff
gitt add .
git commit -m "Afegit capitol 3 sobre gestio de branques"

Exercici 5
-

Mostrar els canvis de l'última versió del repositori respecte a l'anterior.

Canviar el missatge de l'últim commit a "Afegit capítol 3 sobre gestió de branques a l'índex." 
Tornar a mostrar els últims canvis del repositori.

git commit --amend -m "Afegit capitol 3 al index"
Exercici 6
-
Indica a Git que vols ignorar tots els fitxers que comencen per "daw", tots els que tenen l'extensió out i les imatges (jpg, png, bmp i gif).
nano .gitignore

