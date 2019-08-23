Školení GIS v R pro začínající uživatele
========================================

Kapitoly s R kódem, který ve výsledném textu chceme mít vyhodnocený (
výsledek, graf), je třeba napsat ve formátu `.Rrst` a pomocí R funkce
`knitr::knit` vytvořit výsledný `.rst` soubor.

funkci můžeme spustit v R instanci

    knitr::knit("foobar.Rrst")

nebo přímo z terminálu

    Rscript -e 'knitr::knit("foobar.Rrst")'

Funkce vytvoří `.rst` se názvem zdrojového dokumentu.

Možný zápis kódu:

    .. {r rst-example}
    1+1
    rnorm(10)

    x <- 44
    y <- 55
    x + y
    .. ..

nebo

    .. {r rst-example}
    .. 1+1
    .. rnorm(10)
    .. 
    .. x <- 44
    .. y <- 55
    .. x + y
    .. ..


Dokumentace **knitr**
---------------------

[Dokumentace **knitr**](https://yihui.name/knitr)

[Dokumentace **knitr** - plot options](https://yihui.name/knitr/options/#plots)




Licence
-------

http://creativecommons.org/licenses/by-sa/4.0/
