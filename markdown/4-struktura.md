# Obsah kurzu

V poslední kapitole si představíme vytvořený online kurz pro výuku datové analytiky. Tuto část dělíme do několika vzájemně provázaných částí, z nichž každá reflektuje odlišnou oblast návrhu a implementace online kurzu. 

## Průchod

V první částí se zaměříme na obecný průchod kurzem – popíšeme si, jak je kurz navržen po strukturální stránce a jakým způsobem student prochází jednotlivými částmi.

Hlavní část kurzu je tvořena sedmi hlavními obsahovými bloky, z nichž se každý zabývá jedním určitým tématem, které na sebe přímo navazují a představují tak hrubou strukturu online kurzu (viz Obrázek \ref{digi-bloky}). Od studenta se tedy očekává lineární postup směrem od prvního do poslední obsahového bloku, nicméně je i tak studujícímu umožněno procházet libovolný blok dle aktuálních potřeb (a to ať už ty minulé např. z důvodu ujasnění si již probraných témat nebo ty nenavštívené např. kvůli zjištění celkové časové náročnosti kurzu).

Mimo tyto ústřední bloky e-learning na začátku obsahuje úvodní text, jehož cílem je studenta navnadit ke studiu a v co největší stručnosti popsat obsah celého kurzu. Zároveň je pod touto úvodní kartou umístěn malý ukazatel progresu s počtem splněných aktivit (viz další odstavec) spolu s podkartou *Užitečný tip*, která slouží v rámci ekosystému kurzů Digiskills k nasměrování na integrovaného chatbota (viz Obrázek \ref{digi-uvod}).

\begin{figure}[h]   
    \centering
    \includegraphics[width=\textwidth]{digi-uvod}  
    \caption{Úvodní obrazovka s představením kurzu spolu s ukazatelem progresu a s podkartou týkající se užitečného tipu}
    \label{digi-uvod}
\end{figure}

Základní jednotkou kurzu jsou pak již zmíněné aktivity, jež jsou vždy zanořeny do daného obsahového bloku (viz Obrázek \ref{digi-blok}). Těchto aktivit je v celém kurzu v současné chvíli 23 a jsou do jednotlivých bloků logicky uspořádány dle následující šablony:

 - úvodní aktivita, která představuje studentovi dané téma a kontextualizuje jej v rámci aktivit minulých a následujících;
 - 1–3 aktivity zpracovávající konkrétní část tématu;
 - 1–2 závěrečné aktivity, jež shrnují dané téma a pobízí studenta k vlastní práci ať už prostřednictvím kvízů či praktických úkolů (viz Obrázek \ref{digi-aktivity}).

\begin{figure}[h]   
    \centering
    \includegraphics[width=\textwidth]{digi-bloky}  
    \caption{Nerozbalený výčet všech obsahových bloků}
    \label{digi-bloky}
\end{figure}

\begin{figure}[h]   
    \centering
    \includegraphics[width=\textwidth]{digi-blok}  
    \caption{Vnořené aktivity vztahující se ke obsahovému bloku Vizualizace a prezentace dat}
    \label{digi-blok}
\end{figure}

\begin{figure}[h]   
    \centering
    \includegraphics[width=\textwidth]{digi-aktivity}  
    \caption{Závěrečná aktivita, která obsahuje zadání praktického úkolu}
    \label{digi-aktivity}
\end{figure}

Všechny aktivity lze dále kategorizovat podle svého typu, který determinuje, jaká edukační komponenta je v dané aktivitě využita. Kromě typů *nahrát soubor* a *test typeform* (viz níže) musí student po dokončení vybrané aktivity vždy zatrhnout políčko *Označit aktivitu za splněnou*, které aktualizuje progres studenta a přesměruje ho na následující aktivitu.

V našem online kurzu využíváme výhradně těchto pět typů aktivit, které jsme pro účely tohoto e-learningu vytvořili na základě výsledků z provedené přehledové studie online kurzů:

 - *přečíst text* – student musí pro splnění tohoto typu aktivity přečíst textový materiál, který je typicky doplněn o vizualizace, jež téma obsahově doplňují, případně jej graficky člení pro větší přehlednost;
 - *zhlédnout video* – v těchto aktivitách musí student zhlédnout video, které nejčastěji vysvětluje danou problematiku prostřednictvím praktických ukázek;
 - *vložit text* – tyto aktivity rozšiřují první typ, tedy textový materiál doplňují o textové pole, do nějž musí student zadat odpověď na otázku vztahující se k tématu; 
 - *nahrát soubor* – aktivity tohoto typu jsou umístěny za výukovými videy, protože v rámci nich student odevzdává vlastní vypracovanou práci spolu s krátkou textovou reflexí\footnote{Krátkou reflexi jsme po odevzdání praktických úkolů začlenili z toho důvodu, aby měl student možnost zapřemýšlet nad nově nabytými dovednostmi a případnými nejasnostmi, které mohou spojeny buď s probíranou problematikou anebo s formátem samotného kurzu.};
 - *test typeform* – v těchto aktivitách student vypracovává krátký kvíz, jehož cílem je připomenout hlavní znalosti a dovednosti, které si v rámci minulých aktivit osvojil. Při špatné odpovědi kvíz studenta naviguje ke konkrétní aktivitě, která látku vysvětluje, student může posléze svoji odpověď změnit a znovu odpovídat (viz Obrazek \ref{digi-kviz} a \ref{digi-kviz-0}).

\begin{figure}[h]   
    \centering
    \includegraphics[width=\textwidth]{digi-kviz}  
    \caption{Příklad otázky z průběžného kvízu týkající se tématu analýza a vizualizace dat}
    \label{digi-kviz}
\end{figure}

\begin{figure}[h]   
    \centering
    \includegraphics[width=\textwidth]{digi-kviz-0}  
    \caption{Příklad otázky z průběžného kvízu týkající se tématu analýza a vizualizace dat}
    \label{digi-kviz-0}
\end{figure}

Pro úspěšný průchod celým kurzem je zapotřebí mít splněné všechny dílčí aktivity včetně kvízů a korektně odevzdané všechny praktické úkoly. Kurz byl navržen tak, aby byly všechny odevzdané úkoly zkontrolovány pověřenou osobou – chceme tak docílit k poskytnutí individuální zpětné vazby každému jednotlivému studentovi. 

##  Moduly

V této poslední podkapitole popíšeme jednotlivé obsahové bloky (dále jen moduly), které dělíme podle toho, jaký vzdělávací cíl splňují, a tedy zda spadají do teoreticky nebo prakticky zaměřené části kurzu\footnote{Prostřednictvím celkové stylizace kurzu směřujeme k co největší popularizaci tématu, proto jsou některé názvy jednotlivých obsahových bloků a aktivit pojaty méně formálním způsobem.}.

### Úvod aneb co je to vlastně datová analytika

První teoretický modul si klade za cíl uvést studenta do kontextu celého kurzu – představuje mu možnosti online prostředí, vysvětluje, jak probíhá průchod kurzem, a uvádí osnovu kurzu. Ještě před samotnou teorií týkající se úvodních témat datové analytiky je student seznámen se skutečností, že v druhé, praktické části kurzu, bude sám participovat na svém vlastním řešení, prostřednictvím kterého by si měl osahat základní techniky datové analytiky.

V dalších částech tohoto modulu je co srozumitelným způsobem vysvětleno, proč je důležité datovou analytiku v organizacích využívat a jakou přidanou hodnotu může mít při tvorbě firemních rozhodnutí. V této části jsme se také zaměřili na koncept *datově orientované organizace*, v rámci kterého jsme se snažili vztáhnout téma datové gramotnosti právě na organizační prostředí a znovu tak studenta motivovat ke studiu datové analytiky.

V poslední aktivitě jsme se pak zmínili o příbuzných pojmech, které se s datovou analytikou pojí (např. *Big Data* a *IoT*) a jasně jsme vymezili příbuzené disciplíny jako jsou *Data Science* a *Data Engineering*. Z celkového hlediska tento modul naplňuje první dva vzdělávací cíle kurzu (viz cíle \ref{1-cil} a \ref{2-cil}).

### Data, data a zase data

Druhý teoretický obsahový blok zpracovává problematiku spojenou s definicí dat – snaží se studentovi vysvětlit, co si lze pod pojmem data představit a jakým způsobem můžeme data dělit a kategorizovat podle daných potřeb. V této sekci již studenta uvádíme do tématu prostřednictvím krátkého popularizačního videa a následně pomocí stručného článku pobízíme k zamyšlení, s jakým typem dat student nejčastěji pracuje ve svém prostředí.

Na závěr modulu představujeme obsah praktické části kurzu, kterým je proces datové analytiky. Ve videu popisujeme jednotlivé fáze procesu a snažíme se akcentovat fakt, že data nejsou totéž co informace, ale že ze surových dat informace získáváme právě prostřednictvím analýzy a následné vizualizace. Tato část tak splňuje třetí a částečně čtvrtý vzdělávací cíl kurzu (viz cíle \ref{3-cil} a \ref{4-cil}).

### Získávání a import dat

V tomto modulu je studentovi představen první krok datové analytiky, jenž se zabývá importem dat. Na začátku obsahového bloku je nejprve popsána problematika týkající se formátů dat. Popisujeme základní charakteristiky textových a binárních souborů a uvádíme základní příklady souborových přípon spolu s jejich využitím. Na konci první aktivity rozlišujeme dva nejčastěji používané textové formáty pro uchovávání tabulkových dat s příponami *.csv* a *.tsv*, se kterými následně pracujeme v praktické demonstraci.

Hlavní částí tohoto modulu je demonstrační video, v rámci kterého na konkrétním modelovém datasetu\footnote{Zjednodušený dataset obsahuje fiktivní data vztahující se k provedeným objednávkám určité organizace. Každý záznam objednávky je tvořen těmito atributy: jméno prodejce, region, účet, částka, měsíc a datum (atribut datum jsme zde přidali pro účely zpracování speciálního datového typu.)} z fiktivního firemního prostředí představujeme možnosti importu dat. Ohledně výběru datasetu jsme se inspirovali přístupy z analyzovaných online kurzů, nicméně jsme jej upravili tak, aby co nejvíce vyhovoval naší cílové skupině začátečníků.

Po zhlednutí výukového videa, je pak student vyzván k aplikaci nabytých dovedností na stejném datasetu, který jsme použili v demonstraci. V tomto prvním úkolu ještě není po studujícím vyžadovaná žádná velká invence, jde primárně o testovací úkol na přípravu vlastního prostředí a na ozkoušení funkčnosti samotné *odevzdávárny*.

Na konci tohoto modulu by tak mělo být studentovi zřejmé, že jednotlivé fáze datové analytiky na sebe navazují, a je proto zapotřebí vypracovat daný úkol vždy korektním způsobem (tedy alespoň tak, jak je znázorněno v daném demonstračním videu), protože se v dalších praktických částech vychází vždy z výsledků předešlého modulu. Tento obsahový blok naplňuje pátý vzdělávací cíl kurzu\footnote{S ohledem na skutečnost, že se všechny praktické moduly týkají procesu datové analytiky, naplňují vždy současně i čtvrtý cíl kurzu viz cíl \ref{4-cil}.} (viz cíl \ref{5-cil}).

### Čištění dat

Obsahový blok zabývající se čištěním dat pokládáme za jeden z nejdůležitějších, přestože se tohle téma v jiných online kurzech neobjevuje příliš často. Vycházíme z toho, že je na tomto kroku přímo závislá kvalita vlastní analýzy dat, protože se nepřesnosti ve vstupních datech lehce propisují do jednotlivých vztahů napříč daty. Tento fakt se snažíme studentovi představit v úvodní aktivitě, která se prostřednictvím textového materiálu snaží poukázat na nejčastější chyby v datech a na způsoby jejich řešení.

V další části v demonstračním videu využíváme tyto znalosti k opravení nejdůležitějších chyb v našem modelovém datasetu. Výstupem z této části by měla být očištěná tabulková data, která lze dále efektivně zpracovávat. V tuto chvíli je již studentovi dán v rámci praktického úkolu větší prostor, protože je pobídnut k opravě většího množství chyb, než bylo vyřešeno v ukázce. Taktéž zde pracujeme s jednoduchou formou zpětné vazby, protože se zde studujícího ptáme na jeho subjektivní pohled týkající se obtížnosti problematiky.

Nakonec v tomto modulu zavádíme první kvíz, který připomíná základní otázky týkající se dat, jejich importu a čištění. Tato celá část pracuje s šestým cílem (viz cíl \ref{6-cil}).

### Analýza dat