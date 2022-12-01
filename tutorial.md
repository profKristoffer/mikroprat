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
radio.sendString(":-)")
})
```

## Steg 3
Legg til en ``||radio:når radio mottar recivedString||``-blokk. Her skal vi legge til kode som kjøres hver gang vi mottar en tekstmelding.

```blocks
radio.onReceivedString(function (receivedString) {
	
})
```

## Steg 4
Legg til en ``||basic:vis tekst||``-blokk for å vise frem meldinga på skjermen. Dra ``||radio:recivedString||`` ned fra ``||radio:når radio mottar recivedString||`` og dra den inn i ``||basic:vis tekst||``.





<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>