# Diario de la unidad 1

Mi codigo inicial:
``` js
setcpm(78/4)

stack(
  
  s("bd ~ [~ bd] ~, ~ sd ~ sd, hh*8")
    .bank("tr909")
    .gain("0.85 0.45 0.55")
    .velocity("<0.85 0.65 0.75 0.6>")
    .sometimesBy(0.25, x => x.speed(0.98))
    .lpf(6500),

 
  note("<a1 d2 g1 c2>")
    .s("sine")
    .slow(4)
    .gain(0.65)
    .attack(0.02)
    .release(0.7)
    .lpf(600),

```
