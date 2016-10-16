LE COURS
coursIUT IntroGIT.pdf

HELP CMD GIT
http://ndpsoftware.com/git-cheatsheet.html

SIMULATEUR GRAPHIQUE GIT POUR MIEUX COMPRENDRE
http://onlywei.github.io/explain-git-with-d3/

CHANGER CMD LOG EN LG MIEUX PRESENTEE
https://coderwall.com/p/euwpig/a-better-git-log

mkdir tpgit
cd tpgit
git init
ls -a
.git/config
cat >file1.txt
coucou
CTRL-C
git add file1.txt OU git add *
git commit -m "init"
git config --global user.name "tbalastegui"
git config --global user.email tbalastegui@iut.univ-paris.fr

echo "add" >>file1.txt
git add .
git commit -m "added"
git status
git log

REVERT DU GIT AU LOCAL
git checkout file1.txt

git diff

Basculement entre branche
GIT CHECKOUT MASTER

git branch color
gedit
git add .
git commit

git checkout master
git branch size
gedit
git add .
git commit

RESULTAT
* 82968f6 - (HEAD, master) cs (il y a 2 minutes) <tbalastegui>
*   ec07933 - c (il y a 5 minutes) <tbalastegui>
|\  
| * 8dfe541 - (color) change color (il y a 19 minutes) <tbalastegui>
* | b05725a - add (il y a 15 minutes) <tbalastegui>
|/  
* 53e5125 - added (il y a 2 heures) <tbalastegui>
* 6c3f539 - init (il y a 2 heures) <Thomas BALASTEGUI>

tbalastegui@a205-03:~/prive/CSID/ArN/tpgit$ git merge b1 -m "a"
Mise à jour 82968f6..ef34589
Fast-forward (no commit created; -m option ignored)
 file.txt   | 3 +++
 file1.txt~ | 5 +++++
 2 files changed, 8 insertions(+)
 create mode 100644 file.txt

RESULTAT
tbalastegui@a205-03:~/prive/CSID/ArN/tpgit$ git lg
*   ef34589 - (HEAD, master, b1) e (il y a 3 minutes) <tbalastegui>
|\  
| * 82968f6 - cs (il y a 14 minutes) <tbalastegui>
| *   ec07933 - c (il y a 17 minutes) <tbalastegui>
| |\  
| | * 8dfe541 - (color) change color (il y a 31 minutes) <tbalastegui>
| * | b05725a - add (il y a 27 minutes) <tbalastegui>
| |/  
* | b08043f - new commit (il y a 77 minutes) <tbalastegui>
* | fa98bf0 - tutu (il y a 79 minutes) <tbalastegui>
* | 499161b - new (il y a 82 minutes) <tbalastegui>
* | de15420 - added (il y a 85 minutes) <tbalastegui>
|/  
* 53e5125 - added (il y a 2 heures) <tbalastegui>
* 6c3f539 - init (il y a 2 heures) <Thomas BALASTEGUI>