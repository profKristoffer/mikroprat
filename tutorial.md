# Mikroprat
Vi skal nå lære å bruke radioen til en micro:bit til å sende tekstmeldinger til hverandre! 


## Steg 1
Først må vi dra inn en ``||radio: radio sett gruppe||``-blokk. Dette vil fungere som radiokanalen til vår micro:bit og vi kan bruke dette til å sørge for at det er bare du og en annen micro:bit som sender meldinger til hverandre.

```blocks
radio.setGroup(1)
```

## Steg 2
Bruk ``||input:når knapp trykkes||`` for å sende tekstmeldinger over radio med ``||radio:radio send tekst||``.

Dette vil sende en tekstmelding til enhver micro:bit i nærheten som er på samme radiogruppe!

```blocks
input.onButtonPressed(Button.A, function(){
radio.sendText(:-))
})
```







<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>