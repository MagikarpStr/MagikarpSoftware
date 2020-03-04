# MagikarpSoftware
software e script di Magikarp

SASSO CARTA FORBICE in python

from random import randint 
print("carta forbici sasso contro piton") 
premio = "un bel niente"
print("se vinci ricevi come premio " + premio)
print("\ncome ti chiami?")
nome = input()
print("\nbuona fortuna " + nome + ". che vinca il migliore!")
comando = ""
while(comando != "ora basta"):
  print("che arma scegli?")
  armi = ["carta", "forbici", "sasso"]
  for arma in armi:
      print(arma)
  print("premi 0 per carta , premi 1 per forbici , premi 2 per sasso")
  numero_scelto = int(input())
  arma_scelta = armi[numero_scelto]
  print("hai scelto " + arma_scelta)

  arma_piton = ""
  numero_piton = randint(0,2)
  arma_piton =  armi[numero_piton]
  print("...anche piton ha fatto la sua scelta :D")

  verdetto = ""

  if(arma_scelta == "carta" and arma_piton == "sasso"):
     verdetto = nome + " bravo hai vinto!1!1!1!1"
  if(arma_scelta == "forbici" and arma_piton == "carta"):
     verdetto = nome + " bravo hai vinto!1!1!1!1"
  if(arma_scelta == "sasso" and arma_piton == "forbici"):
     verdetto = nome + " bravo hai vinto!1!1!1!1"
  if(arma_scelta == arma_piton):
     verdetto = "pareggio , sempre meglio di niente no?"
  if(verdetto == ""):
     verdetto = " piton ti ha sconfitto"
  print("premi invio per scoprire chi ha vinto :)")
  input()
  print("piton ha scelto " + arma_piton)
  print(verdetto)
  print("\n Scrivi il comando 'ora basta' se ti sei stancato a giocare ")
  comando = input()
print("GIOCO TERMINATO!")
