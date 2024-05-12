# Iniciar sessió

**Versió**: 1.0

**Descripció**:
L’usuari haurà d’inicialitzar sessió cada cop que vulgui entrar a l’aplicació. En cas que no s’hagi registrat s’haurà de registrar. Els clients es podran registrar mitjançant el correu electrònic, telèfon o un servei extern. Els transportistes només es podran registrar mitjançant les seves dades fiscals.<br>

**Actors**: Usuari.

**Precondició:**
Si és transportista haurà de proporcionar les seves dades fiscals.

**Flux Principal**:<br>
1. Escollir registrar-se o loguear-se<br>
2. Si s’ha registrat prèviament:<br>
   2.1 L’usuari inicia sessió.<br>
3. Si n:<br>
   3.1 L’usuari es registra.<br>

**Subfluxos**:<br>

*Si es registra un client:*<br>
   1. Si escull registrar-se per telèfon:<br>
      1.1 L’usuari proporciona el seu telèfon i una contrasenya.<br>
   2. Si escull registrar-se per correu electrònic:<br>
      2.1 L’usuari proporciona el seu correu i una contrasenya.<br>
   3. Si escull registrar-se per un servei extern:<br>
      3.1 L’usuari inicia sessió a través d’aquest servei.<br>
      
*Si es registra un transportista:*<br>
   1. Proporcionar dades fiscals.<br>
   
**Fluxos alternatius**:<br>
**Postcondició**:
Cada cop que l’usuari vulgui entrar a la plataforma haurà d’iniciar sessió.
Requeriments no funcionals.<br>

**Prioritat**: Alta.<br>
**Comentaris**: Cap.



