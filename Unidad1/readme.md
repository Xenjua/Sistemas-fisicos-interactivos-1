# Diario de la unidad 1

Mi codigo inicial:
``` js
const { visualid } = createParams('visualid')

setcpm(25)

// DRUMS
let drum = stack(
  s("oh:1")
    .beat("3,7,11,15", 16)
    .visualid("drum_oh"),

  s("hh")
    .beat("0,2,4,6,8,10,12,14", 16)
    .visualid("drum_hh"),

  s("cp")
    .beat("4,12", 16)
    .visualid("drum_cp"),

  s("bd")
    .beat("0,3,7,10,14", 16)
    .visualid("drum_bd")
).bank("RolandTr909")

$drum: stack(drum, drum.osc())


// MELODY
let melody = note(
  "[c4 e4 g4 e4 d4 c4 ~ e4 g4 a4 g4 e4 d4]"
)
  .sound("piano")
  .legato(0.9)
  .gain(0.8)
  .visualid("melody")

$melody: stack(melody, melody.osc())


// HARMONY
let harmony = note(
  "<[c3,e3,g3] [a2,c3,e3] [f3,a3,c4] [g3,b3,d4]>"
)
  .sound("piano")
  .attack(0.25)
  .lpf(1500)
  .room(1.5)
  .gain(0.6)
  .visualid("harmony")

$harmony: stack(harmony, harmony.osc())
```
