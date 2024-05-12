# Iniciar sessió

CAS D’ÚS:
INICIAR SESSIÓ
Versió
1.0
Descripció
L’usuari haurà d’inicialitzar sessió cada cop que vulgui entrar a l’aplicació. En cas que no s’hagi registrar s’haurà de registrar. Els clients es podran registrar mitjançant el correu electrònic, telèfon o un servei extern. Els transportistes només es podran registrar mitjançant les seves dades fiscals.
Actors
Usuari
Precondició
Si és transportista haurà de proporcionar les seves dades fiscals.
Flux Principal
1. Escollir registrar-se o loguear-se
2. Si s’ha registrar prèviament:
   2.1 L’usuari inicia sessió.
3. Sinó:
   3.1 L’usuari es registra.
Subfluxos
Si es registra un client:
   1. Si escull registrar-se per telèfon:
      1.1 L’usuari proporciona el seu telèfon i una contrasenya.
   2. Si escull registrar-se per correu electrònic:
      2.1 L’usuari proporciona el seu correu i una contrasenya.
   3. Si escull registrar-se per un servei extern:
      3.1 L’usuari inicia sessió a través d’aquest servei.

Si es registra un transportista:
   1. Proporcionar dades fiscals.
Fluxos alternatius


Postcondició
Cada cop que l’usuari vulgui entrar a la plataforma haurà d’iniciar sessió.
Requeriments no funcionals


Prioritat
Alta
Comentaris



