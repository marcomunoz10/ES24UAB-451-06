# Tipus LLiurament


**Versió**: 1.0<br>


**Descripció:**
Un cop enregistrada i pagada la comanda correctament, el botiguer podrà triar 
entre dues opcions: fer una entrega pròpia en la qual la botiga serà l’encarregada 
de fer la distribució de comandes, o bé mitjançant transportistes de proximitat. 
A la fase de distribució es mostrarà un mapa on el client podrà veure on es troba el 
transportista, el dia i la hora aproximada de lliurament.<br>


**Actors**:
Botiguer, GPS, Administrador de Plataforma.<br>


**Precondició**:<br>
1. El transportista ha d’estar registrat amb les dades fiscals que l’identifiquin.<br>
2. L’usuari ha de finalitzar la comanda i pagar-la correctament.<br>


**Flux Principal**:
1. L'usuari finalitza la comanda.<br>
2. El sistema cobra automàticament a la botiga la comissió.<br>
3. Si el botiguer no vol fer l'enviament:
   3.1 El botiguer contracta un transportista.<br>
4. El sistema mostra mitjançant una interfície gràfica com Google Maps on es troba el transportista.
   També mostrarà el dia i hora aproximada de lliurament a la plataforma.<br>

**Subfluxos**:<br>
3. Si botiguer vol fer l’enviament pel seu compte.<br>
  3.1 El botiguer s’encarrega de l’entrega.<br>


**Fluxos alternatius**:<br>
*No hi ha transportistes disponibles*<br>
Emetre missatge d’error i botiguer fa l’entrega.<br>


**Postcondició**:<br>


**Requeriments no funcionals:** 
Un transportista podrà obtenir un encàrrec si aquest es troba enregistrat a l'aplicació i la seva ubicació és propera al comerç o botiga que el vol contractar.<br>


**Prioritat**:
Normal<br>


**Comentaris**: cap



