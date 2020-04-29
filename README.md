# unison-nonempty

A simple non-empty list for Unison

```
type NonEmpty a = NonEmpty a [a]
NonEmpty.:| : a -> [a] -> NonEmpty a
NonEmpty.foldl : (b ->{𝕖} a ->{𝕖} b) -> b -> NonEmpty a ->{𝕖} b
NonEmpty.foldl1 : (a ->{𝕖} a ->{𝕖} a) -> NonEmpty a ->{𝕖} a
NonEmpty.head : NonEmpty a -> a
NonEmpty.map : (a ->{𝕖} b) -> NonEmpty a ->{𝕖} NonEmpty b
NonEmpty.singleton : a -> NonEmpty a
NonEmpty.tail : NonEmpty a -> [a]
NonEmpty.toList : NonEmpty a -> [a]
```
