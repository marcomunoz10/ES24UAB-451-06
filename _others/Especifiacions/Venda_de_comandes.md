# Venda de comandes
**Versió**: 1.0

**Descripció**:<br>
Les botigues presenten els productes a la plataforma. Per a que la plataforma pugui obtenir beneficis, s’haurà de pagar una comissió sobre cada comanda feta amb cada botiga. En el moment de presentar les ofertes al client hi haurà banners de publicitat, d’això s’encarrega un servei extern.<br>

**Actors**: Botiguers, Servei de publicitat, Sistema d’assegurança.

**Precondició**: Les empreses que podran inscriure's al programa són les petites botigues i empreses de proximitat no associades a cap grup empresarial.

**Flux Principal**:
1. La botiga pacta una comissió de venta amb la plataforma.<br>
2. La botiga escull els mètodes de pagament que tindran els clients disponibles a l’hora de realitzar una comanda.<br>
3. Es mostren les ofertes en relació a les necessitats del client.<br>
4. Es mostra publicitat.<br>
5. Client finalitza realitza la compra de productes.<br>
6. Es paga a la plataforma segons la comissió.<br>
7. El botiguer escull tipus d’enviament de comanda.<br>

**Subfluxos**:
*Botiguer pot escollir entrega pròpia.* <br>
*Si botiguer vol fer enviament amb transportista*: <br>
1. Busca transportistes de proximitat.<br>
2. Comprova disponibilitat de transportista.<br>
3. Escull transportista.<br>

**Fluxos alternatius**:
1. Si pagament anul·lat:<br>
   1.1 Una companyia externa  fa un estudi per protegir als venedors.<br>
   
**Postcondició**:
Si botiguer escull fer enviament amb transportistes i no hi ha disponibilitat, botiguer fa entrega pel seu compte.

**Requeriments no funcionals**:
Hi ha d’haver un sistema de reclamacions per als venedors per si algun client anul·la un pagament havent rebut la compra.<br>
En cas que hagi de transportar el paquet el botiguer no hi haurà opció de seguiment del paquet, tot i això, quedarà constància dels quilòmetres del trajecte. 

**Prioritat**: Normal<br>
**Comentaris**: Cap



