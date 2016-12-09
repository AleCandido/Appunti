# Relatività generale - ripasso

## Richiami di relatività ristretta

- Postulato di Einstein
- Intervallo
    - invarianza intervallo: dimostrazione Landau
- Classificazione intervalli
- Tempo proprio (dilatazione dei tempi)
- Trasformazioni di Lorentz
- Trasformazioni delle velocità
    - si ricavano usando Lorentz per i differenziali
- Formalismo 4-D
    - quadritensori covarianti e controvarianti
        - rispetto alle rotazioni spaziali
    - quadrigradiente $\rightarrow$ è covariante
    - i vettori covarianti trasformano con l'inversa
        - se pensati come vettori colonna con l'inversa della trasposta, perchè in realtà sono vettori riga (si pensi al prodotto scalare che deve rimanere invariante)
            - $(\Lambda^t)^{-1} = g \Lambda g^{-1}$
            - $\Lambda = g^{-1} (\Lambda^t)^{-1} g$
            - $gv \rightarrow g \Lambda v = g \Lambda g^{-1} g v = (\Lambda^t)^{-1} (g v)$
    - l'elemento di quadrivolume è invariante sotto Lorentz
        - perchè il Jacobiano della trasformazione è 1
- quadrivelocità e quadriimpulso
    - *mass shell*
    - limiti classico e ultrarelativistico

### Teoria dei campi

- minima azione
    - lagrangiana e densità lagrangiana
- particella libera
    - unica quantità invariante che descrive il moto di una particella
    - limite classico

#### Elettrodinamica
- quadripotenziale
    - invarianza di gauge
- moto di una carica
    - lagrangiana di interazione con il campo
    *(achtung: variabili dinamiche, ora sono le coordinate!)*
        - forza di Lorentz e potenza dissipata
- equazioni omogenee di Maxwell
- equazioni non omogenee di Maxwell
    - lagrangiana dei campi
    - quadricorrente (flusso di densità di carica)
    - lagrangiana d'interazione in termini di quadricorrente
    *(achtung: variabili dinamiche, ora sono le componenti del potenziale!)*

#### Tensore energia-impulso
- parallelo con quadricorrente
    - impulso prende il posto della carica
- modello di materia
    - polvere *ferma*
    - fluido perfetto
    per entrambi i casi:
        - forma covariante
        - traccia positiva
- materia (fredda e calda)
    - nella seconda rientra anche la radiazione

## Campo gravitazionale

- principio di equivalenza
    - sistemi non inerziali:
        - hanno in generale campi che non si annullano all'infinito
        - possono essere annullati con un cambio di coordinate
            - i campi dei gravi no
- definizione della metrica
    - leggi di trasformazione dell'intervallo infinitesimo ds
        - simmetrica
    - in generale non può essere diagonalizzata globalmente con un cambio di coordinate
        - è però possibile in un punto
        - se ne deduce $g= - 1/J^2$
- le trasformazioni della teoria sono i diffeomorifismi (trasformazioni generalizzate)
    - quadrivettori controvarianti
        - il prototipo sono i differenziali delle coordinate
    - il tensore metrico è di default covariante
        - perchè i differenziali standard delle coordinate sono controvarianti
        - la versione controvariante è definita come l'inverso
    - gli indici si alzano e si abbassano con la metrica
    - il tensore unità completamente antisimmetrico non è più un tensore (neanche pseudo)
        - compare il jacobiano davanti ($1/\sqrt{-g}$)
        - così anche per il differenziale di quadrivolume, quindi moltiplicando per $\sqrt{-g}$ riottengo uno scalare

#### Principio di covarianza generale
- un'eq. è vera se:
    - è covariante rispetto alle trasformazioni generalizzate
    - ha il corretto limite per uno spazio-tempo piatto

*il senso di questo principio è che la relatività speciale è vera fino in fondo, perciò per un dato processo si può seguire l'evoluzione grazie al principio di equivalenza: intorno per intorno ci si riduce ad uno spazio-tempo piatto e si applicano le leggi note*

*perciò, se si hanno delle equazioni covarianti che sono vere per uno spazio-tempo piatto si ha che una loro soluzione in un riferimento fissato è anche una soluzione del procedimento precedente (risolvere intorno per intorno in spazi piatti), da cui il principio*

esempi: correlazione causale, intervalli luce

### Intervalli spazio-temporali
- tempo reale
    è quello misurato da un orologio fisico ancorato in un dato punto dello spazio
    - per ricondursi ad esso a partire da quello scandito dalla coordinata:
        - si prendono due eventi fissati in quel dato punto
        - se ne fa la differenza
        - si ricava l'intervallo e infine il tempo proprio (ds = dt, dove t è il tempo proprio)

si ottiene che $g_{_{00}} > 0$, se non lo fosse significa solo che il dato riferimento non può essere realizzato da un corpo fisico

- distanze spaziale
    - lancio un impulso EM, lo faccio rimbalzare e conto quanto tempo ci mette ad andare e tornare
        - la semisomma determina la distanza
        - risolvendo l'eq. si ottiene anche la merica spaziale $dl^2$

    *non ha senso integrare $dl$, perché dipendendo dal tempo la distanza fra due punti dipenderebbe dalla linea d'universo scelta per l'integrazione* (perché la metrica può dipendere dalla coordinata temporale)
    in un riferimento stazionario la metrica non dipende dalla coordinata temporale, e quindi si può anche integrare e anche le distanze finite son ben definite

- simultaneità
    sono simultanei due eventi in un dato riferimento, altrimenti non ha senso (a meno che non siano lo stesso evento); definizione:
    - si parte da un punto e si arriva in un altro (avanti e indietro nel tempo)
    - si prende il punto medio tra partenza e arrivo come simultaneo al giro di boa

    *in questo modo intorno per intorno riesco a sincronizzare i miei orologi, e spostandomi lungo dei cammini posso portare la sincronizzazione in ogni punto dello spazio, **però**: se faccio una linea chiusa trovo che la partenza non è simultanea a se stessa, assurdo*
    - non posso sincronizzare univocamente in generale
        - dipende dal percorso che seguo
    - però con una metrica statica posso farlo
        - ogni metrica si può ricondurre a statica con le trasformazioni generalizzate
        - la simultaneità non è un problema dovuto ai campi, ma ai riferimenti balordi

### Derivazione covariante
I differenziali dei quadrivettori sono differenze tra funzioni valutate in punti differenti, che perciò trasformano in modo differente: **il differenziale di un quadrivettore non è in generale un quadrivettore**
- fissato il primo vettore nel primo punto si identifica un corrispondente (covariante) del secondo vettore, sempre nel primo punto: **trasporto parallelo**
    - in tal modo la differenza fra i due è covariante
    - in un riferimento galileiano i vettori devono essere invarianti per trasporto parallelo (le loro componenti)
- sviluppando questa differenza si trova che oltre al differenziale ordinario vi è un altro termine
    - il nuovo differenziale è il **differenziale covariante**
    - il termine aggiuntivo è composto dal quadrivettore, il differenziale delle coordinate e i **simboli di Christoffel**
    - si ottengono in questo modo anche i differenziali covarianti di tensori generici (covarianti, controvarianti e misti)
        - per gli scalari non c'è differenza fra differenziali ordinari e covarianti, pocihé rimangono invariati per trasporto parallelo
        (a sua volta determinato dal fatto che rimangono invariati per trasformazioni generalizzate, si pensi alla definizione)
- simboli di Christoffel
    - sono simmetrici negli indici inferiori
    - non sono dei tensori
    - dipende solo dalla metrica e le sue derivate prime
- differenziale del determinante della metrica
- teorema di Gauss covariante generale

### Particella in campo gravitazionale
- equazioni
    - dal principio di covarianza generale
        - si ottengono le **geodetiche**
        - la quadriforza dipende dai simboli di Christoffel (e dalla quadrivelocità)
            - la metrica svolge il ruolo di potenziale del campo gravitazionale
            - coerente col principio di equivalenza: posso sempre annullare la forza in un intorno dato
    - dal principio di minima azione
    achtung: stavolta deve variare anche la metrica (ma le variabili dinamiche sono solo le coordinate)
- limite basse velocità
    implica che anche il campo deve essere debole
    - la lagrangiana coincide con quella usuale in meccanica classica

#### Campo gravitazionale costante
cioè la metrica è indipendente dalla coordinata x<sub>0</sub>, cioè è stazionaria
- per più corpi non può esservi una metrica stazionaria: moto generato per attrazione gravitazionale
- se, in una metrica stazionaria, traslo nella coordinata x<sub>0</sub> due eventi simultanei e vicini spazialmene, troverò altri due eventi ancora simultanei
    - il tempo fisico però può tranquillamente scorrere in modo diverso nei due punti dello spazio -> *redshift gravitazionale*
        - in una metrica stazionaria il tempo x<sub>0</sub> di viaggio impiegato da un segnale dipende solo dal percorso che effettua (non dall'x<sub>0</sub> a cui parte), quindi le differenze di tempo x<sub>0</sub> fra segnali consecutivi sono preservate, ma quindi non lo sono quelle di tempo fisico
        - spostamento della frequenza della radiazione EM
    - se il corpo che genera il campo è immobile non ci possono essere componenti anisotrope nella metrica (cioè le componenti miste con il tempo), perché i due versi del tempo sono identici -> metrica statica
        - dalle eq. del moto risulta che la componente 0 del quadriimpulso covariante è conservata
            - all'ordine più basso questa quantità è l'energia meccanica

    **achtung: in relatività generale gli indici si alzano e si abbassano con cautela!** (le quantità fisiche possono cambiare)

### Tensore energia-impulso
Assumendo una lagrangiana che al più è funzione di un campo e delle sue derivate prime e imponendo minima azione si ottengono le equazioni di Eulero-Lagrange con il campo al posto della coordinata come variabile dinamica

- per generalizzare l'azione si sostituisce l'elemento di quadrivolume, moltiplicandolo semplicemente per (-g)<sup>1/2</sup>, così da formare uno scalare: se la lagrangiana è uno scalare rispetto alle trasformazioni generalizzate l'azione è nuovamente uno scalare, con il giusto limite per lo spazio-tempo piatto

**achtung: prima di variare l'azione bisogna esprimere esplicitamente la metrica (ogni contrazione ne sottointende una!)**
essa va variata nella variazione dell'azione, anche se in generale non costituisce una variabile dinamica (a meno che non si voglia trovare le equazioni di Einstein)

- si ottengono di nuovo le eq. di Eulero-Lagrange, ma stavolta la lagrangiana compare moltiplicata per (-g)<sup>1/2</sup> all'interno delle derivate

Si può ricavare il tensore energia-impulso per una lagrangiana arbitraria
- si ha che la derivata covariante del tensore energia-impulso è nulla
```
    - si esegue una trasformazione delle coordinate sommando una quantità piccola
    - si ricava l'azione nelle nuove coordinate (ovviamente al prim'ordine)
        - la lagrangiana è uno scalare rispetto a trasformazioni generalizzate, quindi non varia nel passaggio alle nuove coordinate
    - si trova la variazione rispetto all'azione nelle coordinate originali (*è una variazione puramente formale, non rispetto alle variabili dinamiche*)
        - si impongono le equazioni del moto
        - si impone che la variazione sia nulla, infatti anche l'azione è invariante per trasformazioni generalizzate
    - a questo punto si definisce il tensore energia-impulso in modo naturale
        - non è nullo perché la variazione arbitraria non è quella delle coordinate, ma del termine additivo
    - si esprime la variazione della metrica in funzione di quella del termine additivo
    - si integra per parti con Gauss covariante
     *si tenga di conto che la derivata covariante della metrica è nulla*
```
la definizione del tensore energia-impulso è buona finché la lagrangiana non dipende dalle derivate della metrica
- questo però non porta a un quadriimpulso conservato
    - infatti, mentre tutte le cose covarianti funzionano bene anche con le nuove derivate, il teorema di Gauss non prevede trasporti di vettori e si applica alle derivate ordinarie

## Equazioni del campo gravitazionale

### Tensore di Riemann
- nel trasporto parallelo lungo una geodetica del vettore tangente il trasportato è ancora tangente
    - l'angolo tra due vettori rimane invariato dopo il trasporto $\rightarrow$ la componente tangente di ogni vettore rimane invariata nel trasporto
- **il trasporto parallelo non è conservativo**
    - il differenziale lo è
    - la differenza va attribuita ai simboli di Christoffel
        $\Delta A^{\mu} = - \oint \Gamma_{\alpha \beta}^{\mu} A^{\alpha} dx^{\beta}$
        - si applica Stokes e si ottiene: **il tensore di Riemann**
        - lo si ottiene considerando una variazione infinitesima

*quando si applica Stokes si deve considerare che i valori del quadrivettore all'interno della superficie non sono univocamente determinati dai valori sulla curva, ma la non univocità è al second'ordine*

- lo spazio-tempo è piatto $\rightarrow R^i_{jkl} = 0$  
    - si sceglie un sistesma in cui $\Gamma ^i _{jl} = 0$, il resto è il carattere tensoriale di $R^i_{jkl}$
- vale anche l'inverso: se $R^i_{jkl} = 0$ il trasporto parallelo è un'operazione univoca, quindi dato un'intorno galileiano trasportandolo ottengo un intero riferimento galileiano $\rightarrow$ lo spazio-tempo è piatto
- commutatività derivate covarianti seconde:
    $D_i D_j A_a - D_j D_i A_a = -A_b R^b_{aij}$
    - stessa cosa per derivate di quadrivettori controvarianti e tensori generici

---
#### Proprietà (tensore di Riemann)
- antisimettria/simmetria nelle coppie di indici
- somma ciclica
- identità di Bianchi
---
- tensore di Ricci
- tensori di Riemann in dimensione varia

esempio: moto relativo

### Equazioni di Einstein

$R_{ij} - R g_{ij}/2 = 8 \pi G T_{ij}$

#### dal principio di covarianza generale
- si parte dell'eq. di Newton (scritta come eq. di Poisson)
     - si riconosce la metrica e il tensore energia-impulso
     - sono poche le combinazioni di tensori che soddisfano
- si riconoscono le eq. per la materia dentro le eq. di Einstein

#### da una lagrangiana invariante
- si sceglie come azione la curvatura scalare $R$
    - contiene anche le derivate seconde della metrica, ma non importa perhé sono fattorizzate, e quindi vanno semplicemente a finire in un inessenziale pezzo costante
*ancora una volta: sono i campi le variabili dinamiche*
- nell'azione totale ci va messa anche la parte della materia
    - la si include con il suo tensore energia-impulso
    - contiene anche la parte elettromagnetica, se presente

**le eq. di Einstein non sono lineari**
- tracciando le eq. di Einstein si ottiene un legame tra la traccia del tensore energia-impulso e la curvatura scalare
- in uno spazio vuoto ($T_{ij} = 0$) si ha che $R_{ij} = 0$, ma questo non significa che lo spazio sia piatto

*poiché la divergenza covariante del primo membro è nulla, allora lo è anche quella del secondo membro, ma quest'ultima condizione non sono altro che le equazioni della materia, che vengono così a essere contenute in quelle del campo*

### Pseudotensore energia-impulso
poiché l'annullarsi della divergenza covariante del tensore energia-impulso non porta a una legge di conservazione occorre andare a procacciarsela

- si considera un sistema chiuso (asintoticamente galileiano)
