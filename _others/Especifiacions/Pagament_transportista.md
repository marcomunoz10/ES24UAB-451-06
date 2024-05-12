# Pagament transportista

**Versió**: 1.0<br>
**Descripció:**
El cost del transport es calcula segons la distància recorreguda durant cada lliurament 
registrada pel GPS. La plataforma calcula el cost total dels lliuraments fets per cada transportista 
basant-se en les distàncies enregistrades pel GPS realitza una transferència bancària a cadascú. 
La plataforma manté un registre a la base de dades de tots els pagaments realitzats a cada transportista, assegurant-se 
que rebin la compensació adequada pel seu treball.<br>
**Actors**:
Transportista, GPS, Administrador de la plataforma, Client.<br>
**Precondició**:<br>
1. El transportista ha d’estar registrat amb les dades fiscals que l’identifiquin.<br>
2. L’usuari ha de finalitzar la comanda.<br>
3. El botiguer escull enviament per aquest transportista.<br>

**Flux Principal**:
1. L'usuari finalitza la comanda.<br>
2. El sistema cobra automàticament a la botiga la comissió.<br>
3. Si el botiguer no vol fer l'enviament:<br>
   3.1 El botiguer contracta un transportista.<br>
4. El sistema GPS rastreja el trajecte.<br>
5. La plataforma registra la distància recorreguda.<br>
6. La plataforma calcula la suma mensual.<br>
7. La plataforma paga al transportista.<br>

**Subfluxos**:<br>
3. Si botiguer vol fer l’enviament pel seu compte.<br>
  3.1 El botiguer s’encarrega de l’entrega.<br>
  3.2 No hi ha seguiment GPS.<br>
  
**Fluxos alternatius**:
*No hi ha transportistes disponibles*<br>
Emetre missatge d’error i botiguer fa l’entrega.<br>

**Postcondició**:<br>
**Requeriments no funcionals:** 
Seguretat del pagament: El sistema de pagament ha de ser segur, garantint la confidencialitat i la integritat de les transaccions financeres.<br>
**Prioritat**:
Alta<br>
**Comentaris**: cap



