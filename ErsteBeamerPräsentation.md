# Latech Beamer Markdown

% Präsentation in Markdown
% Referent: DylanBittner
% Date \today


---
theme: "AnnArbor"
header: includes:
colortheme: "seahorse"
fronttheme: "structorbold"
author:
![]()
---

# Erste Folie

Dies ist eine mit Markdown erstellte Präsentation und übersetzt mit Pandoc in einer Beamer Präsentation als PDF.
```bash
pandoc -t beamer <filename.md> -o <praesentationsname.pdf>
```

# Aufzählung mit Formatierung

- punkt 1 mit *kursiven Text*
- punkt 2 mit **fetter Text**
- punkt 3 mit ~~durchgestrichener Text~~

# Formeln und Quoting
>**Merke**
>Markdown und Pandoc sind coll und mächtig.

$$ \int_a\limits^\infty \frac{x^2-a}{e^(x-b)} dx $$
$$ f(x) = sqrt(2-x) $$
$$a^b $$
$$ U_eff = \frac{U^2}{\sqrt{2}} $$

# Bilder einblenden 

````
![Umlet Screenshot](UMLet_screenshot.png)
````
![Umlet Screenshot](https://images1.loopnet.com/i2/f5K0NelJ8EUes5OA6tp5TYP4pJkuQ10yaCNzE_RVVF4/112/136-W-Cotter-Ave-Port-Aransas-TX-Building-Photo-1-HighDefinition.jpg)