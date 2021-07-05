# testgit
testgit

Una delle prime cose che uno sviluppatore deve conoscere al primo giorno di lavoro, è come fare una “pull request” usando GIT + GITHUB.

“Source control” permette a più persone di lavorare sullo stesso file da differenti postazioni, un po’ come google doc.

Creare un nuovo progetto o repository, una volta dato il nome nello step successivo andare su “Code -> HTTPS -> copiare l’URL”. A me però HTTPS non funziona, ma SSH si.

Andare tramite terminale dentro la cartella coi file.

Step:

git clone git@github.com:marcocrupi/testgit.git 
Copiare i file che erano nella cartella dentro la nuova cartella appena generata.
Andare da terminale dentro la cartella creata (nel caso del mio esempio “cd testgit”.
git status (ci dice quali file non sono inclusi nel nostro progetto online su github).
git add index.html
git commit -m “adding starting project”
git push

FINE STEP per primo upload su github.

Per copiare i file di un repository basta accedere a una cartella vuota sul nostro pc e:

git clone git@github.com:marcocrupi/testgit.git 
Una volta clonato modifichiamo il file.
git status (ci dirà che il file è stato modificato rispetto all’originale).
git add . (serve per fare l’upload di tutti i file, perché “git add nomefile” li aggiunge uno alla volta).
git commit -m "changing <p>"
git push

In questo modo ogni volta che salviamo tramite terminale modifichiamo quello comune su github, vedendo i commit si notano le modifiche che ognuno ha effettuato. In questo modo abbiamo una “storia” delle modifiche ed è sempre possibile tornare indietro quando succedono errori.

C’è un solo problema, l’utente che ha effettuato il primo upload del file non ha la sua versione modificata nel suo pc, perché ovviamente il suo pc non sa che il file su githup è stato aggiornato.

Per ovviare a ciò esiste il comando: 

git pull

Non fa altro che aggiornare i file presenti nella cartella main.
