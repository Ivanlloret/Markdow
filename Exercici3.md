Exercici GIT 3: Desfer canvis
=
*Per a realitzar aquests exercicis és necessari haver realitzat prèviament els exercicis sobre l'historial de canvis.*

Exercici 1
-
1. Elimina l'última línia del fitxer índex.txt i guarda-ho.

Nano index.txt (borra ultima fila i guarda) Git add index.txt

git commit -m ‘’eliminar ultima linea index’’

2. Comprova l'estat del repositori.

Git status

3. Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del fitxer.

git checkout HEAD^ -- índex.txt

4. Torna a comprovar l'estat del repositori.

Git status

Exercici 2
-
1. Elimina l'última línia del fitxer índex.txt i guarda-ho.

Nano index.txt (borra ultima fila i guarda) Git add index.txt

git commit -m ‘’eliminar ultima linea index’’

2. Afegeix els canvis a la zona d'intercanvi temporal.

Git add index.txt

3. Comprova de nou l'estat del repositori.

Git status

4. Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de treball.

Git reset HEAD index.txt

5. Comprova de nou l'estat del repositori.

Git status

6. Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del fitxer.

Git cheackout HEAD – index.txt

7. Torna a comprovar l'estat del repositori.

Git status

Exercici 3
-

1. Elimina l'última línia del fitxer índex.txt i guardar-ho.

Nano index.txt (borra ultima fila i guarda)

Git add index.txt

git commit -m ‘’eliminar ultima linea index’’

2. Elimina el fitxer capítols/capitol3.txt.

git rm capítols/capitol3.txt

git commit -m "Eliminar capítols/capitol3.txt"

3. Afegeix un fitxer nou capítols/capitol4.txt buit.

touch capítols/capitol4.txt

git add capítols/capitol4.txt

git commit -m "Añadir capítols/capitol4.txt"

4. Afegeix els canvis a la zona d'intercanvi temporal.

git add índex.txt capítols/capitol4.txt

5. Comprova de nou l'estat del repositori.

git status

6. Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de treball. git reset HEAD índex.txt capítols/capitol4.txt
6. Comprova de nou l'estat del repositori. git status
6. Desfés els canvis realitzats per tornar a la versió del repositori. git checkout -- índex.txt capítols/capitol4.txt
6. Torna a comprovar l'estat del repositori. git status

Exercici 4
-
1. Elimina l'última línia del fitxer índex.txt i guardar-ho.

Nano index.txt (borra ultima fila i guarda)

Git add index.txt

git commit -m ‘’eliminar ultima linea index’’

2. Elimina el fitxer capítols/capitol4.txt.

git rm capítols/capitol4.txt

git commit -m "Eliminar capitol4.txt"

3. Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Borrat accidental."

git add index.txt

git commit -m "Borrat accidental."

4. Comprova l'historial del repositori.

Git log

5. Desfés l'últim commit, però mantin els canvis anteriors al directori de treball i a la zona d'intercanvi temporal.

git reset HEAD^

6. Comprova l'historial i l'estat del repositori.

Git log git status

7. Torna a fer el commit amb el mateix missatge d'abans.

git commit -c ORIG\_HEAD

8. Desfés l'últim commit i els canvis anteriors al directori de treball, tornant a la versió anterior del repositori.

git reset --hard HEAD^

9. Comprova de nou l'historial i l'estat del repositori.

git log git status
