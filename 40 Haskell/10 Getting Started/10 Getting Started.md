# Leer functioneel programmeren met Haskell

Haskell is een luie, functionele taal. Functioneel programmeren een totaal
ander paradigma dan imperatief programmeren, wat je in talen als C en Java
doet. Maar in plaats van de precieze verschillen uit te leggen, laten we je ze
gewoon ondervinden.

Om te beginnen even wat indrukwekkende, zeer compacte voorbeelden in Haskell
([bron](http://blog.fogus.me/2011/06/03/10-haskell-one-liners-to-impress-your-friends/)):

* Multiply each item in a list by 2:

      map (*2) [1..10]

* Sum a list of numbers:

      foldl (+) 0 [1..1000]

* Read a file:

      let fileLines = fmap lines $ readFile "data.txt"

* Split a list of numbers:

      let (passed, failed) = partition (>60) [49, 58, 76, 82, 88, 90]

* Prime number generation

      let pgen (p:xs) = p : pgen [x|x <- xs, x `mod` p > 0]
      take 40 (pgen [2..])

Bedenk ook dat veel niet-functionele programmeertalen wel functionele concepten
in zich hebben, bijvoorbeeld Python, Ruby en Java 8.


## Aan de slag!

Het is tijd om zelf eens te gaan spelen met Haskell. Dat kan geheel online (je
hoeft niks te installeren!) bij FP Complete. [Maak hier eerst een account
aan](https://www.fpcomplete.com/auth/page/email/register).

Lees dan eventjes [hoe je moet leren aan de *School of
Haskell*](https://www.fpcomplete.com/school/how-to-use-the-school-of-haskell/learning-haskell-at-the-soh).
Daarna kun je aan de slag met de [tutorials](https://www.fpcomplete.com/), wij
raden je aan om te beginnen met:

["Basics of Haskell"](https://www.fpcomplete.com/school/basics-of-haskell) 



## Hongerig naar meer?

Voor iedereen die zich af vraagt of ze Haskell ook in de praktijk kunnen
gebruiken is dit een goed [overzicht van de sterke punten van
Haskell](http://amtal.github.io/2011/08/25/why-haskell-is-kinda-cool.html).

Als je meer Haskell wil, kijk dan op de [officiële Haskell
site](http://www.haskell.org/haskellwiki/Haskell).

