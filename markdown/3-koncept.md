\part{Praktická část}

# Koncept kurzu

Ve druhé části této bakalářské práce se budeme zabývat představením vlastního online kurzu zaměřeného na výuku základů datové analytiky. Ve dvou následujících kapitolách si popíšeme návrh a implementaci našeho e-learningu z hlediska dvou různých rovin, a to konceptuální a strukturální.

Našim cílem v této praktické části bude tedy jednak uvést motivaci a cíle vztahující se k tvorbě online kurzu, ale také přehledným způsobem popsat, z jakých komponent se náš kurz skládá a jaké vzdělávací prvky obsahuje. Na závěr také představíme jednotlivé obsahové moduly a podobně je jako primární cíle kurzu zarámujeme do revidované Bloomovy taxonomie vzdělávacích cílů.

## Motivace

Online kurz vznikl pod záštitou firmy Digiskills\footnote{https://www.digiskills.cz/}, která se zabývá rozvojem digitálních kompetencí primárně v korporátním prostředí. Portfolio služeb firmy Digiskills se dá vydělit do dvou hlavních částí. Jednak svým klientům nabízí takzvaný *digiskills-assessment* – jinými slovy audit digitálních dovedností, jehož cílem je zmapovat silné a slabé stránky u dané organizace a nabídnout konkrétní aktivity na zlepšení digitálních kompetencí.

Druhým a také hlavním produktem jsou pak online kurzy, které se převážně zaměřují na oblasti týkající se používání konkrétních nástrojů (jde například o, MS Teams, Office 365, Google Workspace nebo MS Power BI) a na témata spojené s digitálními kompetencemi (např. digitální produktivita, bezpečnost a soukromí nebo efektivní práce z domu). I přes to, že některé tyto kurzy problematiku datové analytiky částečně reflektují, žádný z nich ji nepojímá v širším kontextu pro úplné začátečníky.

Proto vznikla motivace vytvořit v českém prostředí takový online vzdělávací kurz, který se zabývá fundamentálními základy datové analytiky a cílovým organizacím (případně jejich interním týmům anebo jednotlivým zaměstnancům) srozumitelně vysvětluje, k čemu je datová analytika důležitá a na základě jakých potřeb si je vhodné osvojit její základy. 

Samotný kurz\footnote{V ekosystému kurzů firmy Digiskills se komplexnější online kurzy nazývají Digitální akademie – jde ale o pouhou konvenci firmy, tzn. pro účely tohoto textu není tohle označení podstatné a nebudeme jej používat.} vznikal za spolupráce s firmou Digiskills, která nám při návrhu a implementaci poskytla potřebnou infrastrukturu (primárně webové šablony a technické vybavení) a příležitostnou konzultaci, týkající se primárně charakteristiky cílové skupiny a škálování technické náročnosti. Všechna ostatní rozhodnutí týkající se designu kurzu byla ponechána na nás.

## Cíle

Při definování vzdělávacích cílů vycházíme z revidované Bloomovy taxonomie kognitivních vzdělávacích cílů, která byla představena v roce 2001 a jež se více přibližuje konstruktivistickému charakteru vzdělávání \parencite{bloom2}. Na rozdíl od svého předchůdce z roku 1956 tato revidovaná taxonomie mimo jiné popisuje dimenze kognitivních procesů prostřednictvím činných sloves (a nikoliv pomocí podstatných jmen, jak tomu bylo dříve), u nichž dále nabízí konkrétní alternativní pojmenování a vymezení. Druhou podstatnou změnou je přesun hierarchicky nejvyšší kategorie *hodnotit* (v původní taxonomii *hodnocení*) pod novou kategorii *tvořit*, která zase vychází z původní kategorie *syntéza* \parencite{vavra11}.

Níže uvádíme výčet devíti vzdělávacích cílů kurzu, které se vždy týkají jedné ze dvou hlavních oblastí.

- Teoretická část – témata diskutující základní terminologii a motivaci spojenou s datovou analytikou spolu s úvodem do problematiky týkající se dat:
	1. student je schopen ilustrovat na fiktivním příkladu důležitost datové analytiky v modelovém prostředí určité organizace – kategorie porozumět (dávat příklady);
	2. student je schopen rozlišit významy pojmů vztahující se k datové analytice a k příbuzným disciplínám – kategorie porozumět (klasifikovat);
	3. student je schopen kategorizovat jednotlivé typy dat a základní datové formáty používané v rámci tabulkových dat – kategorie porozumět (srovnávat).
- Praktická část – témata týkající se jednotlivých částí procesu datové analytiky spolu s výčtem dalších analytických nástrojů:
	4. student je schopen vysvětlit, z jakých částí se skládá proces datové analytiky a zdůvodnit existenci jednotlivých části – kategorie porozumět (interpretovat);
	5. student je schopen použít základní techniky importování dat nehledě na využívaný nástroj – kategorie aplikovat (realizovat);
	6. student je schopen identifikovat chyby v datech a dovede tyto problémy řádně opravit – kategorie analyzovat (rozlišovat);
	7. student je schopen propojit jednotlivé části dat a vytvořit na základě nich smysluplné vztahy – kategorie analyzovat (uspořádat);
	8. student je schopen vytvořit na základě analyzovaných dat novou informaci, kterou dovede komunikovat prostřednictvím jednoduché vizualizace – kategorie analyzovat (strukturovat);
	9. student je schopen vybrat konkrétní analytický nástroj na základě své informační potřeby – kategorie porozumět (srovnávat).

Jak je z výše uvedeného seznamu patrné, v kontextu revidované Bloomovy taxonomie se pohybujeme v prvních čtyřech kategoriích kognitivních procesů – *pamatovat*, *porozumět*, *aplikovat* a *analyzovat*. Hlavní důvod pro tohle rozhodnutí je vybraná cílová skupina, kterou jsou primárně úplní začátečníci, jež si pod oblastí datové analytiky nic nepředstaví nebo o ní mají pouze zdánlivou představu. Na druhou stranu spadá většina vzdělávacích cílů pod třetí kognitivní proces *aplikovat*, protože hlavním požadavkem na kurz  ze strany Digiskills měl být přesah do praktických úrovní datové analytiky.

## Kompetence

Za účelem začlenění kurzu do některého z kompetenčních rámců, můžeme využít výše popsané cíle, které jsme představili v minulé podkapitole. Odhlédneme-li od těch částí obsahu, které partikulárně vychází z výsledků přehledové studie online kurzů, můžeme náš kurz zakotvit primárně do dvou kompetenčních rámců.

První dokument, již zmíněný sylabus *ECDL / ICDL Data Analytics SYLABUS 1.0 (AM8)*, se vztahuje primárně k praktické části – tedy k cílům 4, 5, 6 a 7. Jak bylo zmíněno v teoretické částí (viz \ref{kompetenux10dnuxed-ruxe1mec}), jedná se o modul, který je zaměřen na základy práce s daty určený pro digitálně kvalifikovanou veřejnost. My z tohoto sylabu využijeme všechny oblasti kompetencí kromě kategorie *8.1 koncepce a statistická analýza*\footnote{Zde můžeme využít akorát rozsah znalostí 8.1.1.2 a 8.1.1.3, protože se jedná o kompetence spojené s chápáním hlavních přínosů datové analytiky a teoretických znalosti jednotlivých fází.}, protože ta se zabývá statistickými pojmy, které nepovažujeme pro naše účely za příliš podstatné (resp. počítáme s tím, že studenti disponují základní znalostí matematiky ze základní školy a dokážou pracovat se základními pojmy jako je například průměr, chápání složitější statistiky tedy není potřebné) \parencite{ecdl17}.

Díky tomuto vzdělávacímu sylabu máme zarámované praktické kompetence procesu datové analytiky do hlavních kategorií a jejich zanořených oblastí znalostí:

- příprava datového zdroje – tuto kategorii v našem online kurzu vydělujme do dvou částí, a to do *importu dat* a *čištění dat*, zde jsme inspirovali přístupy jiných kurzů, které začátečníkům tyto dvě fáze vysvětlují odděleně;
	- import, přizpůsobení importu;
	- filtrování;
- shrnování dat – s touto kategorií pracujeme v kurzu pod názvem *analýza dat*, terminologicky totiž lépe sedí do konceptu jiných kurzů zabývající procesem datové analytiky;
	- agregace dat v kontingenční tabulce;
	- frekvenční analýza v kontingenční tabulce;
	- filtrování kontingenční tabulky;
	- používání kontingenčního grafu;
- vizualizace dat;
	- koncepce a nastavení;
	- prvky vizualizace;
	- publikování a sdílení.