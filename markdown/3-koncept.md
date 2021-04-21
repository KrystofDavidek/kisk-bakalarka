\part{Praktická část}

# Koncept kurzu

Ve druhé části této bakalářské práce se budeme zabývat představením vlastního online kurzu zaměřeného na výuku základů datové analytiky. Ve dvou následujících kapitolách si popíšeme návrh a implementaci našeho e-learningu z hlediska dvou různých rovin, a to konceptuální a strukturální.

Našim cílem v této části bude tedy jednak uvést motivaci a cíle vztahující se k tvorbě nového online kurzu, ale také přehledným způsobem popsat, z jakých komponent se náš kurz skládá a jaké vzdělávací prvky obsahuje. Na závěr také představíme jednotlivé obsahové moduly a zarámujeme je do Bloomovy taxonomie vzdělávacích cílů.

## Motivace

Online kurz vznikl pod záštitou firmy Digiskills\footnote{https://www.digiskills.cz/}, která se zabývá rozvojem digitálních kompetencí primárně v korporátním prostředí. Portfolio služeb firmy Digiskills se dá vydělit do dvou hlavních částí. Jednak svým klientům nabízí takzvaný *digiskills-assessment* – jinými slovy audit digitálních dovedností, jehož cílem je zmapovat silné a slabé stránky u dané organizace a nabídnout konkrétní aktivity na zlepšení digitálních kompetencí.

Druhým a také hlavním produktem jsou pak online kurzy, které se převážně zaměřují na oblasti týkající se používání konkrétních nástrojů (jde například o, MS Teams, Office 365, Google Workspace nebo MS Power BI) a na témata spojené s digitálními kompetencemi (např. digitální produktivita, bezpečnost a soukromí nebo efektivní práce z domu). I přes to, že některé tyto kurzy problematiku datové analytiky částečně reflektují, žádný z nich ji nepojímá v širším kontextu pro úplné začátečníky.

Proto vznikla motivace vytvořit v českém prostředí takový online vzdělávací kurz, který se zabývá fundamentálními základy datové analytiky a cílovým organizacím (případně jejich interním týmům anebo jednotlivým zaměstnancům) srozumitelně vysvětluje, k čemu je datová analytika důležitá a na základě jakých potřeb si je vhodné osvojit její základy. 

Samotný kurz\footnote{V ekosystému kurzů firmy Digiskills se komplexnější online kurzy nazývají *Digitální akademie* – jde ale o pouhou konvenci firmy, v tomto textu na náš kurz referujeme obyčejným výrazem *online kurz*} vznikal za spolupráce s firmou Digiskills, která nám při návrhu a implementaci poskytla potřebnou infrastrukturu (primárně webové šablony a technické vybavení) a příležitostnou konzultaci, týkající se primárně charakteristiky cílové skupiny a škálování technické náročnosti. Všechna ostatní rozhodnutí týkající se designu kurzu byla ponechána na nás. 

## Cíl

Při definování hlavního vzdělávacího cíle vycházíme z revidované Bloomovy taxonomie kognitivních vzdělávacích cílů, která byla představena v roce 2001 a jež se více přibližuje konstruktivistickému charakteru vzdělávání \parencite{bloom2}. 

Hlavní cíl kurzu se dá vydělit do dvou hlavních dílčích cílů:

 1. student si je po skončení kurzu vědom, co je to datová analytika a proč je důležité znát základní principy a metody této disciplíny;
 2. studující po skončení kurzu vědět, z čeho skládá proces datové analytiky a dokáže na základě těchto znalostí provést základní.

## Kompetence