# Micro:Bit & Phyphox ☀️⚡
```package
bluetooth
-radio
```
## Einführung @unplugged

Lerne wie man den @boardname@ mit Phyphox via Bluetooth verknüpft und die Daten einer Photovoltaikzelle analysiert.

## Bluetooth aktivieren @fullscreen

Klicke auf (+)  ``||advanced:extension:bluetooth||`` und füge Bluetooth dazu. Dabei musst du die Auswahl bestätigen, da der @boardname@ entweder per 
Bluetooth statt Radio kommunizieren wird. 

## Verbindungskontrolle  ✔️

Um zu Kontrollieren, ob der @boardname@ verbunden ist, fügen wir einen ``||bluetooth:onBluetoothConnected||``
melden mit einem Bild ``||basic:showIcon||`` das erfolgreiche Verbinden zurück.

```blocks
bluetooth.onBluetoothConnected(function () {
    basic.showIcon(IconNames.Yes)
})
```

## Verbindungskontrolle  ❌

Look at the virtual @boardname@, you should see the heart and your drawing blink on the screen.
```blocks
bluetooth.onBluetoothDisconnected(function () {
    basic.showIcon(IconNames.No)
})
```
## Bluetoothservice starten

```blocks
bluetooth.startUartService()
```
## Daten senden 

```blocks
basic.forever(function () {
    bluetooth.uartWriteLine("")
})
```

## Installieren auf dem @boardname@

Klicke auf ``||download||``, um dein Programm auf deinen @boardname@ zu übertragen!


> Diese Seite bei [https://gitalm.github.io/tutorial-microbit--phyphox-/](https://gitalm.github.io/tutorial-microbit--phyphox-/) öffnen

## Als Erweiterung verwenden

Dieses Repository kann als **Erweiterung** in MakeCode hinzugefügt werden.

* öffne [https://makecode.microbit.org/](https://makecode.microbit.org/)
* klicke auf **Neues Projekt**
* klicke auf **Erweiterungen** unter dem Zahnrad-Menü
* nach **https://github.com/gitalm/tutorial-microbit--phyphox-** suchen und importieren

## Dieses Projekt bearbeiten ![Build Status Abzeichen](https://github.com/gitalm/tutorial-microbit--phyphox-/workflows/MakeCode/badge.svg)

Um dieses Repository in MakeCode zu bearbeiten.

* öffne [https://makecode.microbit.org/](https://makecode.microbit.org/)
* klicke auf **Importieren** und dann auf **Importiere URL**
* füge **https://github.com/gitalm/tutorial-microbit--phyphox-** ein und klicke auf Importieren

## Blockvorschau

Dieses Bild zeigt den Blockcode vom letzten Commit im Master an.
Die Aktualisierung dieses Bildes kann einige Minuten dauern.

![Eine gerenderte Ansicht der Blöcke](https://github.com/gitalm/tutorial-microbit--phyphox-/raw/master/.github/makecode/blocks.png)

#### Metadaten (verwendet für Suche, Rendering)

* for PXT/microbit
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
