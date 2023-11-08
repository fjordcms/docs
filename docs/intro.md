---
sidebar_position: 1
---

# Začínáme s FjordCMS

Webový systém určený pro tvoření originálních webů rychleji, efektivněji.  Disponuje modularitou a výsledkem jsou weby s libovolnou šablonou a různorodým zaměřením.

**Použité backend technologie:** PHP (Nette), MySQL, JSON

### Co je cílem?
-   Vytvoření webového systému s rychlým nasazením na weby různorodých zájmů a funkcionalit
-   Webový systém s podporou aktualizací a rozšíření
-  Webový systém s možností tvorby virtuální databáze pro uchovávání různých dat na základě aktuálního uživatele webového systému (viz EAV)
-   Webový systém s podporou multijazyčnosti

### Co je potřeba?

- [PHP with version >7.4](https://www.php.net/downloads.php)
- webserver supporting PHP (Apache, Nginx) and administration of .htaccess
- [MySQL/MariaDB database](https://mariadb.org/)

## Logika a návrh systému
Fjord CMS je postaven tak, aby se mohl přizpůsobit náročným webům a zhotovením různého typu (eshop, ale zároveň i třeba blog či portfolio). 
Systém je rozdělen na tři logické celky (jádro, šablony, moduly).

### Jádro
Obsahuje základní funkcionalitu systému a řeší propojení šablon, modulů a databáze. Řeší problematiku, která je společná pro weby různého spektra.
- [Autentizace do systému](ddas)
  - vč. backendového řešení zapomenutého hesla
  - společné pro administrátory i uživatele
-  [Autorizace a systém permissí a rolí](das)
-  [Nastavení globálních proměnných pro SEO](das) (google-analytics, meta proměnné)
- [Nastavení emailových serverů (SMTP)](das)

### Moduly
Kvůli modularitě, kterou Fjord CMS podporuje, je nutné ke všemu přistupovat dynamicky a tak i přemýšlet, aby výsledkem byl nezastaralý rozvíjející se redakční systém.
Moduly jsou samostatné open-source části obohacující systém o další funkcionalitu.
Určité moduly jsou v systému zakomponovány a nemusí být instalovány externě. [Seznam předem nainstalovaných modulů](dasd)

**Například pro blogový systém můžeme mít základnu modulů:**
- Články 
- Komentáře
- Stránky

> **V příštích verzích bude spuštěna i podpora větvení modulů (vytváření sub-modulů) kdy pro modul můžeme vytvářet funkční přídavky.`**

### Šablona
Šablona je logická část popisujicí web a design. V nynější verzi systému nejsou dostupné žádné základní šablony a tak pro každý web musí být využita externě nainstalovaná šablona. 
- [Vytvoření externí šablony](dd)
- [Instalace externí šablony](dd)
- [API v šabloně](dd)