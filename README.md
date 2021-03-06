# Automatic TEI encoding of manuscripts catalogues with GROBID-Dictionaries

## Credits

GROBID dictionaries is developed by Mohamed Khemakhem ([GitHub](https://github.com/MedKhem)).

More info on GROBID technologies can be found [here](https://grobid.readthedocs.io).

## Corpus

The corpus is based on scans of catalogues published by Auguste Laverdet, the *Revue des autographes*, directed by Gabriel Charavay ([data.bnf](http://data.bnf.fr/10429866/gabriel_charavay/)) and different auction sales catalogues published by the Maison Charavay.

## Methodology

PDF are OCRised with [Transkribus](https://transkribus.eu). 

The GROBID dictionaries model is trained on four different types of catalogues. For each type, 15 annotated pages are available : 10 as training data and 5 as evaluation data. 

The training data are extracted from the following catalogs issues:
+ Gabriel Charavay, _Revue des Autographes_, first series : 25, 35, 50, 80.
+ Gabrielle Charavay _Revue des Autographes_, second series : 24, 56.
+ Auguste Laverdet, _Catalogue de lettres autographes et manuscrits_ : 1, 22.
+ Etienne Charavay, _Catalogue d’une intéressante collection de lettres autographes…_ (14 décembre 1908).

The source of the training files are references in the file names using the following acronyms:
+ RDA_1 for Revue des Autographes, first series
+ RDA_2 for Revue des Autographes, second series
+ LAV for catalogues written by Auguste Laverdet
+ ETI for auction catalogues written by Etienne Charavay

In compliance with the 
PDF are OCRised with [recommendations of Grobid⁻Dictionaries](https://github.com/MedKhem/grobid-dictionaries/wiki/How-to-Annotate%3F), the separators, whether there are composed of one or two punctuation signs, are tagged with the neutral label <pc>.
  
Examples : 

            <entry>
                <num>350</num>
                <pc>.</pc>
                <form>
                    <name>STANISLAS</name>
                    <pc>,</pc>
                    <desc>roi de Pologne N. 1677. M. 1766</desc>
                </form>
                <pc>. -</pc>
                <sense>
                    <subSense>L. aut. sig. à madame de Boufïlers. Lunéville, 5 janvier 1741. 1 page in-4, 10</subSense>
                </sense>
            </entry>
            <pc>»</pc>
            <entry>

## Files
Training data and evaluation data are available in `ToyData`

## Licence

Regarding `GROBID`, cf. [here](https://github.com/MedKhem/grobid-dictionaries).

Regarding the corpus: extracted data is CC-BY.  

<a rel="license" href="https://creativecommons.org/licenses/by/2.0"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/2.0/88x31.png" /></a><br />

## Cite this dataset

Lucie Rondeau du Noyer, Simon Gabay, Mohamed Khemakhem, Laurent Romary. 2019. _Training and evaluation data for encoding Manuscript Sales Catalogues with GROBID dictionaries_. Retrieved from https://github.com/lairaines/grobid_TEI_2019


