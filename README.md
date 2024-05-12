# 10FastFingersHack

Dakikada maksimum kelime sayısını elde etmek için bunu kopyalayıp tarayıcı konsolunuza yapıştırın

```javascript
var input = $('#inputfield')[0]
var ev = $.Event('keyup')
ev.which = 32
setInterval(function() {
    if ($('.highlight')[0]) {
        input.focus()
        input.value = $('.highlight').text()
        $(input).trigger(ev)
    }
}, 100)
```
