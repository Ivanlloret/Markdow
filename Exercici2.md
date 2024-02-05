Exercici GIT 2: Ús de l'historial de canvis
=

Per a realitzar aquests exercicis és necessari haver realitzat prèviament els **exercicis de creació i actualització de repositoris. 
Exercici 1
-
Mostra l'historial de canvis del repositori.
git log

Crea la carpeta capítols i dins d'ella crea el fitxer capitol1.txt amb el següent text:
mkdir capitols
cd capitols
nano capitol1.txt

Afegeix els canvis a la zona d'intercanvi temporal (staging area) Fes un commit dels canvis amb el missatge "Afegit capítol 1." 
git add capitol1.txt
git commit -m "Afegit cap 1"

Torna a mostrar l'historial de canvis del repositori. 
git log

Exercici 2
-

Crea el fitxer capitol2.txt a la carpeta capítols amb el següent text:
nano capitol2.txt

Afegeix els canvis a la zona d'intercanvi temporal.

Fes un commit dels canvis amb el missatge "Afegit capítol 2." 

Mostra les diferències entre l'última versió i les dues versions anteriors.
git add capitol2.txt
git commit -m "Afegit commit 2"
git diff HEAD^ HEAD
git diff HEAD^^ HEAD

Exercici 3
-

Crea el fitxer capitol3.txt a la carpeta capítols amb el següent text: 

nano capitol3.txt

Afegeix els canvis a la zona d'intercanvi temporal. 

Fes un commit dels canvis amb el missatge "Afegit capítol 3."
nano capitol3.txt
git add capitol3.txt
git commit -m "Afegit capitol 3"

Mostra les diferències entre la primera i l'última versió del repositori.
git diff HEAD^ HEAD

Exercici 4
-
Afegir al final del fitxer índex.txt la següent línia:

echo "Capitol 5: Conceptes avançats" >> index.txt

Afegir els canvis a la zona d'intercanvi temporal. 

Fer un commit dels canvis amb el missatge "Afegit capítol 5 a l'índex." Mostrar qui ha fet canvis sobre el fitxer índex.txt.
git add index.txt
git commit -m "Afegit capitol 5 a l'index"
git blame index.txt
