# Obsah kurzu

V poslední kapitole si představíme vytvořený online kurz pro výuku datové analytiky. Tuto část dělíme do několika vzájemně provázaných částí, z nichž každá reflektuje odlišnou oblast návrhu a implementace online kurzu. 

## Průchod

V první částí se zaměříme na obecný průchod kurzem – popíšeme si, jak je kurz navržen po strukturální stránce a jakým způsobem student prochází jednotlivými částmi.

Hlavní část kurzu je tvořena sedmi hlavními obsahovými bloky, z nichž se každý zabývá jedním určitým tématem, které na sebe přímo navazují a představují tak hrubou strukturu online kurzu (viz Obrázek \ref{digi-bloky}). Od studenta se tedy očekává lineární postup směrem od prvního do poslední obsahového bloku, nicméně je i tak studujícímu umožněno procházet libovolný blok dle aktuálních potřeb (a to ať už ty minulé např. z důvodu ujasnění si již probraných témat nebo ty nenavštívené např. kvůli zjištění celkové časové náročnosti kurzu).

Mimo tyto ústřední bloky e-learning na začátku obsahuje úvodní text, jehož cílem je studenta navnadit ke studiu a v co největší stručnosti popsat obsah celého kurzu. Zároveň je pod touto úvodní kartou umístěn malý ukazatel progresu s počtem splněných aktivit (viz další odstavec) spolu s podkartou *Užitečný tip*, která slouží v rámci ekosystému kurzů Digiskills k nasměrování na integrovaného chatbota (viz Obrázek \ref{digi-uvod}).

\begin{figure}[ht]   
    \centering
    \includegraphics[width=\textwidth]{digi-uvod}  
    \caption{Úvodní obrazovka s představením kurzu spolu s ukazatelem progresu a s podkartou týkající se užitečného tipu}
    \label{digi-uvod}
\end{figure}

Základní jednotkou kurzu jsou pak již zmíněné aktivity, jež jsou vždy zanořeny do daného obsahového bloku (viz Obrázek \ref{digi-blok}). Těchto aktivit je v celém kurzu v současné chvíli 23 a jsou do jednotlivých bloků logicky uspořádány dle následující šablony:

 - úvodní aktivita, která představuje studentovi dané téma a kontextualizuje jej v rámci aktivit minulých a následujících;
 - 1–3 aktivity zpracovávající konkrétní část tématu;
 - 1–2 závěrečné aktivity, jež shrnují dané téma a pobízí studenta k vlastní práci ať už prostřednictvím kvízů či praktických úkolů (viz Obrázek \ref{digi-aktivity}).

\begin{figure}[ht]   
    \centering
    \includegraphics[width=\textwidth]{digi-bloky}  
    \caption{Nerozbalený výčet všech obsahových bloků}
    \label{digi-bloky}
\end{figure}

\begin{figure}[ht]   
    \centering
    \includegraphics[width=\textwidth]{digi-blok}  
    \caption{Vnořené aktivity vztahující se ke obsahovému bloku Vizualizace a prezentace dat}
    \label{digi-blok}
\end{figure}

\begin{figure}[ht]   
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

\begin{figure}[ht]   
    \centering
    \includegraphics[width=\textwidth]{digi-kviz}  
    \caption{Příklad otázky z průběženého kvízu týkající se tématu analýza a vizualizace dat}
    \label{digi-kviz}
\end{figure}

\begin{figure}[ht]   
    \centering
    \includegraphics[width=\textwidth]{digi-kviz-0}  
    \caption{Příklad otázky z průběženého kvízu týkající se tématu analýza a vizualizace dat}
    \label{digi-kviz-0}
\end{figure}

Pro úspěšný průchod celým kurzem je zapotřebí mít splněné všechny dílčí aktivity včetně kvízů a korektně odevzdané všechny praktické úkoly. Kurz byl navržen tak, aby byly všechny odevzdané úkoly zkontrolovány pověřenou osobou – chceme tak docílit k poskytnutí individuální zpětné vazby každému jednotlivému studentovi. 

##  Moduly

V této poslední podkapitole popíšeme jednotlivé obsahové bloky (dále jen moduly), které dělíme podle toho, jaký vzdělávací cíl splňují, a tedy zda spadají do teoreticky nebo prakticky zaměřené části kurzu.

### Úvod aneb ‚‚Co je to vlastně datová analytika

První modul spadá do teoretické části, protože si klade za cíl (viz cíl \ref{1-cil}) uvést studenta do tématu prostřednictvím...