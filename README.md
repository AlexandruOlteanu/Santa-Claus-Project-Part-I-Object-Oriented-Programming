<Copyright Alexandru Olteanu, grupa 322CA, alexandruolteanu2001@gmail.com>

    In aceasta prima etapa a proiectului am ales sa parsez
input-ul prin aceleasi metode folosite de echipa de POO la 
tema 1. Am creat un InputLoader ce face acest lucru si un Input 
in care sa stochez datele parsate. De asemenea am construit clase 
separate pentru fiecare din datele mentionate la input (Copii, 
Schimbari Anuale, etc). Odata create aceste clase am creat clasa 
pentru crearea fisierelor de output corespunzatoare.
    De aici flow-ul rezolvarii a mers destul de usor, am folosit 
Singleton Pattern la toate clasele unde acest lucru a fost posibil
si de asemenea pentru crearea tuturor copiilor ce fac parte din mai
multe categorii de varsta am folosit Design-ul de Factory Patern.
In acest mod am putut avea o clasa abstracta ce contine tipuri 
diferite de copii pentru care average score-ul se calculeaza in mod 
diferit. Am urmarit reprezentarea proceselor si functiilor intr-un mod 
cat mai bine organizat pentru viitore adaugari de functionalitati in 
cadrul claselor.
    Din punct de vedere al solutiei propriu zise am trecut prin fiecare 
test, am parsat datele de input si apoi am inceput desfasurarea rundelor.
Fiecare runda a fost mai intai updatata (cu exceptia rundei 0) si apoi 
rezolvata. Update-urile le-am facut prin functii separate, din nou, pentru
eficienta si mai usoara intelegere a codului. In urma schimbarilor 
corespunzatoare aplicate copiilor in urma fiecarei runde am calculat 
bugetul oferit fiecaruia si apoi lista de cadouri cumparate in anul respectiv
dupa instructiunile cerintei. Pentru fiecare runda am adaugat datele intr-un 
JSONObject pe care l-am clonat folosind DeepCopy (In caz contrar datele actuale 
schimbau valori la rundele anterioare daca nu erau scrise direct). Aceste obiecte
JSON au fost puse intr-un JSONArray ce la final a fost afisat in intregime. Astfel, 
fiecare test a fost rezolvat intr-un mod optim si folosind eficient Design Patterns.
    Per total dificultatea acestei prime etape nu a fost in partea de implementare
a cerintei ci mai mult in citire, scriere si atentia sporita pentru DeepCopy si 
usurarea implementarii folosind Design Patterns.

     

