### Treść zadania:

```js
function printFlag(input) {
    var k = uNdefined => /.{6}j.*aXp/.test(uNdefined)
    var a = (l,o,d,z) => l+z == (o+d).split('').reverse().map(x => x+"").join("")
    var v = (input) => {
        var g = input * 2
        var b = !(!(!(g)))
        b = a(input[0], input[3], input[2], input[1]) ? b : false
        var f = input + "MYK"
        if(f.length == 8)
            b = ("correct!") && k(f.split('').reverse().join('X'))
        else
            return false
        return b
    }
    if(v(input)) {
        if(this.flag == undefined)
            console.log("1753c{" + input + "}")
    }
}
```

### Rozwiązanie:

Kod trzeba było przeanalizować i zwrócić uwagę na kilka warunków jakie spełniać musi poprawna flaga, w szczególności

- musi ona spełniać określone wyrażenie regularne
- dwa pierwsze znaki muszą być takie same jak dwa kolejne znaki
- długość całego inputa po dodaniu "MYK" musi wynosić 8 znaków

Finalnie flaga spełniająca powyższe założenia to

> 1753c{papaj}

### Alternatywne rozwiązania:

Ze względu na błąd w treści zadania można było dopasować także inne ciągi które spełniały warunki przedstawione w kodzie, ale nie były poprawną flagą. W szczególności odkryć je mogły osoby które zdecydowały się po zapoznaniu z kodem, że ciąg o długości pięciu znaków moża brute-forceować.
