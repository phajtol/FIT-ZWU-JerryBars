# FIT-ZWU-JerryBars

This is a project created as a homework for subject Basics of Web (BI-ZWU - Základy webu a uživatelská rozhraní) at FIT CTU.

Full assignment in Czech language is below.

Summary of the assignment: Create a static web presentation of a company that advertises product or service in order to sell.

This homework was created by hand without using any framework or similar tools.

Web presentation is available at my website: https://peter.hajtol.eu/fit/BI-ZWU/.

# Assignment

Cílem semestrální práce (dále jen SP) je firemní statická webová prezentace propagující nějaký produkt či službu za účelem prodeje. Následující seznamy obsahují požadavky na semestrální práci rozdělené do několika skupin. Aby SP prošla kontrolním automatem, musí uvedené požadavky splňovat a musí být také prosta typických nedostatků.

Perfektní SP (za plný počet bodů) by měla také obsahovat propracovaný a adekvátní design vzhledem ke svému účelu. Může také obsahovat detaily či zajímavosti k pochlubení u zkoušky, jako např. nedělitelné mezery v textu.


## Technické požadavky

- **Validní a sémantický kód XHTML 1.1 (jedině) a CSS všech stránek**.
POZOR na vkládání cizích bloků kódu (ikony sociálních sítí, odznaky validátorů) a externí knihovny (animované prohlížení obrázků).
Poznámka: z validity jazyka CSS může být ustoupeno, pokud je ustoupení zjevně vědomé (a ideálně v samostatném souboru)

- **Názvy všech souborů a adresářů se musí skládat pouze ze znaků `a-z0-9_.-`**

- **Lokální odkazy musí být relativní**.
Např. `<a href="onas.html">` místo `<a href="http://.../onas.html">`
Nevytvářejte různé odkazy (URL) na stejný soubor (zdroj)!
Např. domovskou stránku odkazujte jako kořenový adresář `<a href="/">` a nikoli jako soubor `<a href="index.html">`, neboť odkazy `www.example.com` a `www.example.com/index.html` jsou technicky vzato různé.
Pro zajištění fungování odkazu s lomítkem použijte BASE element.

- **Odkazy na neexistující stránky uvádějte bez atributu href a vizuálně je odlište!**
Nevytvářejte slepé odkazy či odkazy s prázdným atributem `href`.
Nevytvářejte stránky typu `Under Construction`.


## Informační architektura (IA)

- **Obsah musí být realistický a smysluplný (a bez duplicit)**.
Obsah může být převzatý (zkopírovaný) odkudkoli.
Kompletní odpovědnost za obsah nese autor SP (nikoli autor zdroje).
Uvádějte zdroje informací (stačí holé odkazy v kódu formou komentáře).

- **Jazyk obsahu libovolný z množiny {česky, anglicky, slovensky}.**.
POZOR: vyberte si jeden jazyk a jazyky nekombinujte!

- **Obsah jednotlivých prvků a stránek jako celku musí být vyvážený**.
Ani příliš mnoho ani příliš málo obsahu…
Pište čitelné texty, které byste sami chtěli číst :)
Každý seznam by měl obsahovat 5±2 položek. Platí i pro skupinu nadpisů atp.

- **Struktura jednotlivých stránek musí být korektní (hierarchická) a členitá**.
Jeden nadpis a pár odstavců rozhodně nevyhovuje.
Za každým nadpisem musí existovat shrnující odstavec – bez výjimky.
Odstavec by neměl být kratší, ale ani delší než 3-5 krátkých vět.
Věty či body seznamu by měly být jednoduché – o pár slovech.
POZOR: Dodržujte pravidlo obrácené pyramidy!
POZOR: Vyvarujte se singularit – jeden odstavec či jeden seznam na kapitolu, jedna věta v odstavci či jedna položka v seznamu apod.
POZOR: Více nadpisů (libovolné úrovně) nesmí následovat přímo za sebou.

- **Práce musí obsahovat média (obsahová grafika či video)**.
POZOR: Velikost, rozměry a formát médií musí být adekvátní zobrazení.
POZOR: Obrázky a další média musí patřit k (významovému) blokovému elementu. Např. jako součást věty odstavce nebo viz „figure“ (v HTML5 či LaTeX).

- **Práce musí obsahovat akci k dosažení komerčního cíle**.
Např. funkční tlačítko Koupit nebo Objednat vedoucí na stránku akce
Stránka akce může být pro všechna tlačítka stejná

- **Práce musí obsahovat jednoduchý funkční kontaktní formulář**.
Formulář musí využívat existující veřejnou externí službu pro zpracování dat z formuláře (uložení/e-mail)
POZOR: Řešení musí být robustní (nepoužívejte iframe apod.)


## Přístupnost

- **Žádné slepé či cyklické odkazy**.
POZOR na logo na úvodní stránce a odkazy nabídky menu na právě zobrazovaných stránkách!

- **Maximální používání významových prvků a adekvátní používání těch bezvýznamových (seskupovacích)**.
Nadpis jako „nadpis“ (elementy `h1`, `h2`, …), odstavec jako „odstavec“ (element `p`) atd.

- **Nepoužívejte formátovací elementy jako `b`, `i`, `font` …**.
Pozor na použití elementů `br` a `hr`.

- **Efektivní využití plochy okna prohlížeče na všech běžných zobrazeních/zařízeních**.
AKA flexibilita (liquid layout) a responsibilita
AKA stránky nemají přečnívat (horizontální posuvník) a nemají mít zbytečné okraje
POZOR na kombinaci absolutních a relativních jednotek!
POZOR: na nepřizpůsobivou podstatu elementu table…
POZOR: na malé obrazovky (telefon na výšku), aby na nich statický obsah nezabíral neúměrně velkou část (záhlaví, logo, navigace).

- **WCAG 2.0, úroveň minimálně AA**.
TIP: používejte relativní jednotky (kdekoli je to možné) a nikdy nezmenšujte písmo
[Vyhláška č. 64/2008 Sb.](http://www.mvcr.cz/clanek/vyhlaska-c-64-2008-sb-o-forme-uverejnovani-informaci-souvisejicich-s-vykonem-verejne-spravy-prostrednictvim-webovych-stranek-pro-osoby-se-zdravotnim-postizenim-vyhlaska-o-pristupnosti-10.aspx)
[\(on-line verze\)](http://www.pravidla-pristupnosti.cz/),
[Metodický pokyn k vyhlášce č. 64/2008 Sb.](http://www.mvcr.cz/clanek/metodicky-pokyn-k-vyhlasce-c-64-2008-sb-o-forme-uverejnovani-informaci-souvisejicich-s-vykonem-verejne-spravy-prostrednictvim-webovych-stranek-pro-osoby-se-zdravotnim-postizenim-vyhlaska-o-pristupnosti.aspx)
[\(on-line verze\)](http://www.pristupnost.cz/ceska-pravidla-pristupnosti/)


## Použitelnost

- **Respektování Desatera domovské stránky**.

- **Celistvost (bez sirotčích stránek) a konzistence řešení**.

- **„Dobré zvyky použitelnosti“**

- **Úspěšná Nielsonova heuristická evaluace**.
POZOR: Zejména uživatel musí vždy vědět, kde se nachází!

- **Rozdělení stránek na část záhlaví, obsah a zápatí**.
Záhlaví `<div id="header">`: drobečková navigace, případně nabídka menu, logo apod.
Obsah `<div id="content">`: obsah stránky počínaje hlavním nadpisem
Zápatí `<div id="footer">`: copyright, mapa stránek, autor, datum úprav apod.

- **Stránky musí obsahovat příslušné metainformace**.
Minimálně kódování, titulek, popis, klíčová slova a případně další
POZOR: Obsah titulku má být specifický (unikátní) a obsahovat zařazení dané stránky ve struktuře webu.


## Vzhled

- **Externí (oddělené) definování vzhledu**.

- **Styly bez absolutních jednotek (vč. px), kdekoli to je možné/vhodné**.

- **Podpora tisku (stránkování, barvy a další)**.
POZOR: na nadužívání (absolutního/relativního) pozicování a vlastnosti `!important`

- **Vzhled má odpovídat účelu a typickým návštěvníkům webu!**.
