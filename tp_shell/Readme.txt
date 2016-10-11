#lister les fichiers java

find  . -name \*.java

#compter combien il y a de fichier java

find  . -name \*.java | wc -l

#liste les fichiers et leurs nombres de lignes

find . -name \*.java -exec wc -l {} \;

#lister les 10 plus gros fichier

find . -name \*.java -exec wc -l {} \; | sort -n | tail

#compter le nombre total de ligne de code java

resultat=0;for f in $(find . -name \*.java); do count=$( cat $f | wc -l ) resultat=$(( $resultat + $count )); done; echo $resultat