\part{Praktická část}

# Koncept kurzu

Ve druhé části této bakalářské práce se budeme zabývat představením vlastního online kurzu zaměřeného na výuku základů datové analytiky. Ve dvou následujících kapitolách si popíšeme návrh a implementaci našeho e-learningu z hlediska dvou různých rovin, a to konceptuální a obsahové.

Našim cílem v této praktické části bude tedy jednak uvést motivaci a cíle vztahující se k tvorbě online kurzu, ale také přehledným způsobem popsat, z jakých komponent se náš kurz skládá a jaké vzdělávací prvky obsahuje. Na závěr také představíme jednotlivé obsahové moduly a podobně je jako primární cíle kurzu zarámujeme do revidované Bloomovy taxonomie vzdělávacích cílů.

## Motivace

Online kurz vznikl pod záštitou firmy Digiskills\footnote{https://www.digiskills.cz/}, která se zabývá rozvojem digitálních kompetencí primárně v korporátním prostředí. Portfolio služeb firmy Digiskills se dá vydělit do dvou hlavních částí. Jednak svým klientům nabízí takzvaný *digiskills-assessment* – jinými slovy audit digitálních dovedností, jehož cílem je zmapovat silné a slabé stránky u dané organizace a nabídnout konkrétní aktivity na zlepšení digitálních kompetencí.

Druhým a také hlavním produktem jsou pak online kurzy, které se převážně zaměřují na oblasti týkající se používání konkrétních nástrojů (jde například o, MS Teams, Office 365, Google Workspace nebo MS Power BI) a na témata spojená s digitálními kompetencemi (např. digitální produktivita, bezpečnost a soukromí nebo efektivní práce z domu). I přes to, že některé tyto kurzy problematiku datové analytiky částečně reflektují, žádný z nich ji nepojímá v širším kontextu pro úplné začátečníky.

Proto vznikla motivace vytvořit v českém prostředí takový online vzdělávací kurz, který se zabývá fundamentálními základy datové analytiky a cílovým organizacím (případně jejich interním týmům anebo jednotlivým zaměstnancům) srozumitelně vysvětluje, k čemu je datová analytika důležitá a na základě jakých potřeb si je vhodné osvojit její základy. 

Samotný kurz\footnote{V ekosystému kurzů firmy Digiskills se komplexnější online kurzy nazývají Digitální akademie – jde ale o pouhou konvenci firmy, tzn. pro účely tohoto textu není tohle označení podstatné a nebudeme jej používat.} vznikal za spolupráce s firmou Digiskills, která nám při návrhu a implementaci poskytla potřebnou infrastrukturu (primárně webové šablony a technické vybavení) a příležitostnou konzultaci, týkající se primárně charakteristiky cílové skupiny a škálování technické náročnosti. Všechna ostatní rozhodnutí týkající se designu kurzu byla ponechána na nás.

## Cíle

Při definování vzdělávacích cílů vycházíme z revidované Bloomovy taxonomie kognitivních vzdělávacích cílů, která byla představena v roce 2001 a jež se více přibližuje konstruktivistickému charakteru vzdělávání \parencite{bloom2}. Na rozdíl od svého předchůdce z roku 1956 tato revidovaná taxonomie mimo jiné popisuje dimenze kognitivních procesů prostřednictvím činných sloves (a nikoliv pomocí podstatných jmen, jak tomu bylo dříve), u nichž dále nabízí konkrétní alternativní pojmenování a vymezení. Druhou podstatnou změnou je přesun hierarchicky nejvyšší kategorie *hodnotit* (v původní taxonomii *hodnocení*) pod novou kategorii *tvořit*, která zase vychází z původní kategorie *syntéza* \parencite{vavra11}.

Níže (viz Tabulka \ref{tab-cile}) uvádíme seznam vzdělávacích cílů kurzu, které se vždy týkají jedné ze dvou hlavních oblastí a korespondují vždy k dané kategorii kognitivního procesu. Oblasti dělíme na teoretickou část, která obsahuje témata týkající se základní terminologie a motivace spojené s datovou analytikou spolu s úvodem do problematiky dat. Druhá praktická část zpracovává témata týkající se jednotlivých částí procesu datové analytiky spolu s výčtem dalších analytických nástrojů.

\input{assets/cile.tex}

Jak je z uvedené tabulky patrné, v kontextu revidované Bloomovy taxonomie se pohybujeme v prvních čtyřech kategoriích kognitivních procesů – *pamatovat*, *porozumět*, *aplikovat* a *analyzovat*. Hlavní důvod pro tohle rozhodnutí je vybraná cílová skupina, kterou jsou primárně úplní začátečníci, jež si pod oblastí datové analytiky nic nepředstaví nebo o ní mají pouze zdánlivou představu. Na druhou stranu spadá většina vzdělávacích cílů pod třetí kognitivní proces *aplikovat*, protože hlavním požadavkem na kurz ze strany Digiskills měl být přesah do praktických úrovní datové analytiky.

\clearpage

## Kompetence

Za účelem začlenění kurzu do některého z kompetenčních rámců, můžeme využít výše popsané cíle, které jsme představili v minulé podkapitole. Odhlédneme-li od těch částí obsahu, které partikulárně vychází z výsledků přehledové studie online kurzů, můžeme náš kurz zakotvit primárně do dvou kompetenčních rámců.

Již zmíněný sylabus *ECDL / ICDL Data Analytics SYLABUS 1.0 (AM8)* se vztahuje primárně k praktické části – tedy k cílům 4, 5, 6 a 7. Jak bylo zmíněno v teoretické částí (viz sekce \ref{kompetenux10dnuxed-ruxe1mec}), jedná se o modul, který je zaměřen na základy práce s daty určený pro digitálně kvalifikovanou veřejnost. My z tohoto sylabu využijeme všechny oblasti kompetencí kromě kategorie *8.1 koncepce a statistická analýza*\footnote{Výjimku tvoří oblasti 8.1.1.2 a 8.1.1.3, které můžeme využít v teoretické části, protože se jedná o kompetence spojené s chápáním hlavních přínosů datové analytiky a teoretickou znalostí jednotlivých fází.}, protože ta se zabývá pokročilejšími statistickými pojmy, které nepovažujeme pro naše účely za příliš podstatné (postačují základní znalosti matematiky ze základní školy) \parencite{ecdl17}.

Díky tomuto vzdělávacímu sylabu máme zarámované praktické kompetence procesu datové analytiky do hlavních kategorií a jejich zanořených oblastí znalostí:

- příprava datového zdroje – tuto kategorii v našem online kurzu vydělujme do dvou částí, a to do *importu dat* a *čištění dat*, zde jsme inspirovali přístupy jiných kurzů, které začátečníkům tyto dvě fáze vysvětlují odděleně;
	- import, přizpůsobení importu;
	- filtrování;
- shrnování dat – s touto kategorií pracujeme v kurzu pod názvem *analýza dat*, terminologicky totiž lépe sedí do konceptu jiných kurzů zabývající procesem datové analytiky;
	- agregace dat v kontingenční tabulce;
	- frekvenční analýza v kontingenční tabulce;
	- filtrování kontingenční tabulky;
	- používání kontingenčního grafu;
- vizualizace dat;
	- koncepce a nastavení;
	- prvky vizualizace; 
	- publikování a sdílení.

Pro zarámování kompetencí, které se vztahují k prvním třem a také poslednímu vzdělávacímu cíli, využijeme obecnější model *The seven pillars of information literacy: The core mode*, který nám umožňuje nahlížet na problematiku teoretické povahy datové analytiky z hlediska informační gramotnosti.

Jak už bylo řečeno v první kapitole (viz sekce \ref{datovuxe1-gramotnost}), tento model se skládá ze sedmi základních pilířů, z nichž každý zastřešuje určitou sadu kompetencí, které jsou součástí informační (popřípadě datové) gramotnosti. Pro účely prvního a třetího cíle jsou relevantní primárně první dva pilíře – *identify* (identifikace informační potřeby) a *scope* (posouzení stávajících znalostí a jejich případných mezer) \parencite{sconul11}.

První cíl týkající se motivace pro využívání datové analytiky je dle našeho názoru zahrnutý v prvním a druhém pilíři, a to konkrétně v těchto kompetencích:

- zjištění nedostatku znalostí v dané oblasti;
- rozpoznání informační a datové potřeby k dosažení konkrétního cíle a definování limitů této potřeby;
- identifikování typu informace, který nejlépe vyhovuje k naplnění dané potřeby.

Aby mohl kdokoliv vykonávat činnosti spojené s datovou analytikou, musí si nejprve uvědomit určité mezery v aktuálních znalostech (ať už jde o kontext jednotlivce, týmu či celé organizace) a být si přitom vědom informační/datové potřeby, která je impulzem pro nabytí nových informací (jinými slovy výsledků ze zpracovaných dat). V praxi to tedy znamená, že by měl studující chápat důvody, kdy se vyplatí proces datové analytiky v rámci své organizace provádět a jaký typ znalostí tak může být získán.

Kompetence, které jsou součástí třetího cíle (základní charakteristika dat a datových formátů), lze částečně uchopit prostřednictvím druhého pilíře, který v sobě znalost datových formátů implicitně obsahuje (jde o kompetenci *identifikování různých formátů, ve kterých jsou poskytovány informace*). Musíme ale pracovat s obecnějším pojetím, protože význam formulace *formát informací*, tak jak je popsán ve standardu, nemusí být nutně totožný s datovým formátem, jak jej chápeme v rámci datové analytiky. 

Uvědomujeme si tedy, že zvolený model informační gramotnosti *The seven pillars of information literacy: The core mode* nebyl primárně navržen za účelem zarámování kompetencí online kurzů, které se týkají datové analytiky. Nicméně i tak jsme se pokusili některé cíle našeho kurzu propojit s navrženými kompetencemi modelu, a znovu tak poukázat na vztah tématu našeho kurzu s obecnějšími koncepty, jako jsou informační a datová gramotnost.

Poslední dva nereflektované cíle, druhý (znalost příbuzných pojmů a disciplín) a devátý (znalost různých analytických nástrojů), jsou úzce svázány s oblastí datové analytiky a souvisí s konkrétním pojmoslovím a s aktuálními trendy. Je proto značně obtížné začlenit tyto kompetence do určitého širšího rámce. Z tohoto důvodu nám dává největší smysl tato témata zpracovat v kontextu výsledků přehledové studie a inspirovat se tak z již existujících funkčních řešení.