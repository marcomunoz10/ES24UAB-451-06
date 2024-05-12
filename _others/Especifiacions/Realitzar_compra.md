# Realitzar Compra

**Versió**: 1.0

**Descripció**:
Fer una compra per part de l'usuari és fer una comanda en l’aplicació dels productes que es volen adquirir. L’usuari ha d’indicar que és el que necessita i seguidament farà una comanda o més d’una amb els diferents productes que vagi escollint indicant per cada un la quantitat que vol. Es mostrarà les botigues més properes que tinguin els productes sol·licitats i el client haurà d’escollir la botiga. Per acabar, fer el pagament amb les opcions disponibles donades pel venedor.<br>

**Actors**: Client, Botiguer, Proveïdor.

**Precondició:**
L’usuari ha d’estar enregistrat com a client.

**Flux Principal**:<br>
1. L’usuari cerca el que vol o necessita.<br>
2. L’usuari afegeix el producte a la comanda.<br>
3. Si el producte no existeix o no està disponible:<br> 
   3.1. Posar un missatge indicant-ho.<br>
   3.2. Treure el producte de la comanda.<br>
   3.3. Tornar al pas 2.<br>
4. Indicar la quantitat del producte.<br>
5. Si vol més productes:<br>
   5.1. Tornar al pas 2.<br>
6. Veure botigues properes amb els productes sol·licitats.<br>
7. Escollir botiga i la forma de pagament.<br>
8. Realitzar pagament.<br>
9. Pagament ha fallat:<br>
   9.1.Tornar al pas 8.<br>
10. Indicar que la compra s’ha realitzat.<br>


**Subfluxos**:<br>

**Fluxos alternatius**:
El client no ha seleccionat cap producte. 
Emetre missatge d’error.<br>

**Postcondició**:
El client ha d’haver afegit un o més productes a la seva comanda.
Indicar si no hi ha cap botiga que tingui disponible un producte de la comanda.<br>

**Requeriments no funcionals:**
Seguretat de la compra: S’ha de poder fer la compra sense el cap estafa possible i sempre respectant la seguretat de la informació que s’hagi utilitzat.

**Prioritat:** Alta.<br>
**Comentaris:** Cap.