## Arduino IDE

va installato e avviato. la prima volta la schermata si blocca. A quel punto è possibile stopparlo, aprire nella cartella `.arduinoIDE` della home dell'utente il file `arduino-cli,yaml`. Aggiungere in coda al file le impostazione del proxy di fiddler:

```
network:
  proxy: http://localhost:8888
```
