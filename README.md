
# Table of Contents

1.  [Introduzione](#orgb961887)
2.  [Struttura Cartella](#org354f547)



<a id="orgb961887"></a>

# Introduzione

Questa cartella nasce con l'idea di creare un singolo luogo in cui
inserire tutto il materiale di studio relativo alla laurea di
informatica all'università di Tor Vergata.

Questa libreria vuole dunque contenere due diverse tipologie di dati:

-   I dati "ufficiali", ovvero quelli caricati dai professori e
    presenti nel sito di informatica.

-   I dati "non-ufficiali", ovvero quelli generati e trovati dagli
    studenti.

Per quanto riguarda lo scaricamento dei dati "ufficiali", rimando al
seguente link ([TorVergataCSWebAPI](https://github.com/LeonardoE95/TorVergataCSWebAPI)), in cui discuso lo script
utilizzato per scaricarli.


<a id="org354f547"></a>

# Struttura Cartella

La struttura delle cartelle che contengono i vari dati è così
descritta:

-   Tutti i dati relativi alla triennale si trovano nella cartella
    `./bachelor`.

-   Tutti i dati relativi alla triennale si trovano nella cartella
    `./master`.

Sia per quanto riguarda i dati della triennale e sia per quanto
riguarda i dati della magistrale, entrambe le cartelle seguono poi
la seguente strutturazione:

-   Per ogni anno scolastico abbiamo una particolare cartella della
    forma `18-19`, `19-20`, `20-21` e via dicendo, che contiene tutti i dati
    per quello specifico anno scolastico.

-   All'interno della cartella di uno specifico anno invece troviamo
    le seguenti cartelle
    -   `courses`, che contiene i dati relativi ai vari corsi.
    -   `exams`, che contiene i dati relativi ai vari esami delle varie sessioni.
    -   `schedule`, che contiene i dati relativi agli orari delle lezioni dei vari semestri.
    -   `teachers`, che contiene i dati relativi ai professori.
    -   `news`, che contiene i dati relativi agli ultimi annunci.

-   La cartella `courses` in particolare poi contiene un file generale
    `all.csv` che contiene tutti i particolari insegnamenti relativi
    allo specifico anno scolastico, e per ogni materia contiene una
    cartella il cui nome corrisponde con il codice del corso della
    materia. Ad esempio la cartella `courses` della triennale dell'anno
    `19-20` contiene i seguenti files/cartelle
    
        AE       AM   ASD2  CN  FI  GA  IS    LMP  MD   PJDM  PW  SOR
        all.csv  ASD  BDC   CP  FO  IA  LING  LRL  MLS  PR    RO

-   All'interno delle varie cartelle relative alle materie dei vari
    corsi, sia per i corsi della triennale che per quelli della
    magistrale, troviamo poi un file `.json` che contiene le varie
    informazioni del corso e due cartelle:
    -   `professor`, che contiene il materiale caricato dal professore sul
        sito.
    
    -   `students`, che idealmente dovrebbe contenere il materiale
        caricato da ciascun studente.

