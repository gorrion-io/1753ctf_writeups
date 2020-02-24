### Treść zadania:

```js
function printFlag(input) {
    var xd = "javascripty"
    var xd = "||y|||t|p|||i|r||c|s||a|v|a|j|_||||"
    var _ = String.fromCharCode(117, 109, 105, 101, 109)
    var flg = "1753c{" + _ + "_" + `i
    n
    t
    o`.split('\n').map(x => x.trim()).join('') + xd.split('|').reverse().join('') + "}"
    
    if(flg == input)
        console.log(flg)
}
```
### Rozwiązanie:

Kod wystarczyło wrzucić do dowolnego parsera JavaScript, np. do okienka konsoli w narzędziach deweloperskich Chrome usuwając z niego if'a i uruchomić, tak aby bez względu na wynik porównania wypisał poprawną flagę

> 1753c{umiem_into_javascripty}
