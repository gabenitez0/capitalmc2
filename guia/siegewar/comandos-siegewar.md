---
description: Comandos necesarios para utilizar SiegeWar correctamente.
---

# 馃Л Comandos SiegeWar

### Ver Informaci贸n

* Asedios - **/sw hud \[nombre de la ciudad]** - Activa / desactiva un HUD para monitorear el progreso de un asedio en particular.&#x20;
* Ciudad - **/t** o **/t here** o **/t \[nombre de la ciudad]** - Ver informaci贸n detallada sobre el asedio a la ciudad (si lo hay).
* Naci贸n - **/n \[nombre de la naci贸n]**: muestra la lista de asedios en los que est谩 involucrada la naci贸n (si corresponde).

### Asignar rangos militares:&#x20;

* Pueblo - **/t rank add \[nombre del jugador] \[rango]** - Como alcalde, asigne rangos de **guardia** y **sheriff**. Como sheriff, asigne rangos de guardia. **Los guardias, alguaciles y alcaldes pueden ganar puntos de batalla si la ciudad est谩 bajo asedio.** Los alcaldes tambi茅n pueden ejecutar rendiciones por asedio.&#x20;
* Naci贸n - **/n rank add \[nombre del jugador] \[rango]** - Como rey, asigne cualquier rango militar de la naci贸n, p. Ej. **agente**, **sargento**, **teniente**, **capitan**, **mayor**, **coronel** y **general**. Como general, asigne cualquiera de estos excepto general. El rey, o cualquier soldado, puede ganar puntos de batalla en asedios de naciones / aliados. Los reyes y generales tambi茅n pueden ejecutar ataques de asedio / abandonos / invasiones / saqueos.

#### Pagar a Soldados:&#x20;

* **/sw nation paysoldiers** - Como rey, paga un salario militar a tus soldados. Cada soldado recibe una parte del dinero, seg煤n su rango militar.

#### Cobro de ingresos militares:

* **/sw collect**: como soldado, obtenga los ingresos que le correspondan de: Saquear o Salario militar.

#### Cobrar el reembolso de la naci贸n**:**

* **/sw collect**: como rey, si su naci贸n es eliminada por cualquier motivo, incluida la captura de su 煤ltima ciudad, se le reembolsar谩 (80%) del costo de instalaci贸n inicial. Este comando cobra ese reembolso.&#x20;

#### Gestionar la ocupaci贸n de forma pac铆fica:

* **/sw nation removeoccupation** - Como rey, elimine pac铆ficamente la ocupaci贸n de una ciudad por parte de su naci贸n.&#x20;
* **/sw nation transferoccupation** - Como rey, invita a otra naci贸n a ocupar pac铆ficamente una ciudad que ocupas actualmente.&#x20;
* **/sw town inviteoccupation** - Como alcalde, invita a una naci贸n a ocupar pac铆ficamente tu ciudad.

### Hacer la ciudad pac铆fica

* **/t toggle neutral**: como alcalde, declara que tu ciudad es pac铆fica. La paz har谩 que su ciudad sea completamente inmune a los ataques de asedio y, a cambio, puede ser ocupado pac铆ficamente por naciones poderosas cercanas. ADVERTENCIA: No active esta funci贸n a menos que est茅 preparado para aceptar las desventajas, incluida la posibilidad de Ocupaci贸n pac铆fica.
* Tiempo de confirmaci贸n:&#x20;
  * El estado se confirmar谩 en 5 d铆as (o 2 si la ciudad es nueva).&#x20;
* Ventajas:&#x20;
  * La ciudad es inmune a los asedios.&#x20;
* Desventajas:&#x20;
  * La ciudad no puede mover el bloque de origen.&#x20;
  * Los residentes no pueden recibir rangos nacionales-militares.&#x20;
  * Los residentes se ven afectados por la enfermedad de guerra si entran en una zona de asedio.&#x20;
  * La ciudad puede ser ocupada pac铆ficamente, siguiendo las siguientes reglas:

> 1. Por cada pueblo pac铆fico, cada \*\* pueblo guardi谩n \*\* dentro de 75 cuadras ejerce \*\* influencia \*\* en el pueblo pac铆fico.
>    * Una ciudad guardiana es cualquier ciudad no pac铆fica de una naci贸n, de tama帽o 30 bloques de ciudades (configurables) o m谩s.
>    * Una ciudad guardiana ocupada ejerce influencia sobre su ocupante, no sobre su naci贸n de origen.
>    * La fuerza de influencia de cualquier ciudad guardiana es igual a su n煤mero de cuadras.
> 2. Si la ciudad pac铆fica tiene una naci贸n, las influencias de la naci贸n de origen y las naciones enemigas extranjeras se amplifican enormemente, de tal manera que siempre ser谩n m谩s fuertes que las influencias de naciones extranjeras no enemigas.
> 3. Posibles resultados:
>    * Si hay influencia sobre la ciudad pac铆fica, la ciudad quedar谩 desocupada.
>    * Si la influencia m谩s fuerte pertenece a la naci贸n de origen de la ciudad pac铆fica, la ciudad quedar谩 desocupada.&#x20;
>    * Si la influencia m谩s fuerte pertenece a una naci贸n extranjera, la ciudad ser谩 ocupada pac铆ficamente por esa naci贸n.

#### Hacer que la ciudad no sea pac铆fica:&#x20;

* **/t toggle neutral**: como alcalde, declara que tu ciudad no es pac铆fica.&#x20;
* Tiempo de confirmaci贸n:&#x20;
  * El estado se confirmar谩 en 5 d铆as (o 2 si la ciudad es nueva).&#x20;
* Efectos:&#x20;
  * La paz y todos sus efectos ser谩n eliminados.&#x20;
  * La ocupaci贸n NO se eliminar谩.&#x20;
  * Cualquier ocupante que tuviera la ciudad, antes de volverse pac铆fico, ser谩 restaurado.&#x20;

#### Gestionar la paz de la naci贸n

* Si todas las ciudades de una naci贸n son pac铆ficas, la naci贸n se considera pac铆fica.

