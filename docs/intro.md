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
Obsahuje základní funkcionalitu systému a řeší propojení šablon, modulů a databáze. Řeší autentizaci i autorizace (vč. systému rolí a práv.)

### Moduly
Kvůli modularitě, kterou Fjord CMS podporuje, je nutné ke všemu přistupovat dynamicky a tak i přemýšlet, aby výsledkem byl nezastaralý rozvíjející se redakční systém.
Moduly jsou samostatné části obohacující systém o další funkcionalitu. Například modul Články ; Samostatné stránky atd.

## Generate a new site

Generate a new Docusaurus site using the **classic template**.

The classic template will automatically be added to your project after you run the command:

```bash
npm init docusaurus@latest my-website classic
```

You can type this command into Command Prompt, Powershell, Terminal, or any other integrated terminal of your code editor.

The command also installs all necessary dependencies you need to run Docusaurus.

## Start your site

Run the development server:

```bash
cd my-website
npm run start
```

The `cd` command changes the directory you're working with. In order to work with your newly created Docusaurus site, you'll need to navigate the terminal there.

The `npm run start` command builds your website locally and serves it through a development server, ready for you to view at http://localhost:3000/.

Open `docs/intro.md` (this page) and edit some lines: the site **reloads automatically** and displays your changes.
