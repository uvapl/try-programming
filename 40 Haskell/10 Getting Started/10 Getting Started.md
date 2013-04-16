# Haskell

## Introductie

Haskell is een functionele taal, waar de nadruk ligt op functies en de
applicatie hiervan en 

Kijk dan eens naar de volgende zeer compacte Haskell voorbeelden
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

Voor de wat ervaardere programmeurs, die zich afvragen of ze Haskell in de
praktijk kunnen gebruiken is dit een goed [overzicht van de sterke punten van
Haskell](http://amtal.github.io/2011/08/25/why-haskell-is-kinda-cool.html).


## Aan de slag!

Het is tijd om zelf eens te gaan spelen met Haskell. Dat kan geheel online (je
hoeft niks te installeren!) bij de introductie [Basics of
Haskell](https://www.fpcomplete.com/school/basics-of-haskell) van FP Complete.

En om af te sluiten een link naar de offciële Haskell site:
<http://www.haskell.org/haskellwiki/Haskell>.

