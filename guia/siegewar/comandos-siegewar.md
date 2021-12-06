---
description: Comandos necesarios para utilizar SiegeWar correctamente.
---

# 🧭 Comandos SiegeWar

### Ver Información

* Asedios - **/sw hud \[nombre de la ciudad]** - Activa / desactiva un HUD para monitorear el progreso de un asedio en particular.&#x20;
* Ciudad - **/t** o **/t here** o **/t \[nombre de la ciudad]** - Ver información detallada sobre el asedio a la ciudad (si lo hay).
* Nación - **/n \[nombre de la nación]**: muestra la lista de asedios en los que está involucrada la nación (si corresponde).

### Asignar rangos militares:&#x20;

* Pueblo - **/t rank add \[nombre del jugador] \[rango]** - Como alcalde, asigne rangos de **guardia** y **sheriff**. Como sheriff, asigne rangos de guardia. **Los guardias, alguaciles y alcaldes pueden ganar puntos de batalla si la ciudad está bajo asedio.** Los alcaldes también pueden ejecutar rendiciones por asedio.&#x20;
* Nación - **/n rank add \[nombre del jugador] \[rango]** - Como rey, asigne cualquier rango militar de la nación, p. Ej. **agente**, **sargento**, **teniente**, **capitan**, **mayor**, **coronel** y **general**. Como general, asigne cualquiera de estos excepto general. El rey, o cualquier soldado, puede ganar puntos de batalla en asedios de naciones / aliados. Los reyes y generales también pueden ejecutar ataques de asedio / abandonos / invasiones / saqueos.

#### Pagar a Soldados:&#x20;

* **/sw nation paysoldiers** - Como rey, paga un salario militar a tus soldados. Cada soldado recibe una parte del dinero, según su rango militar.

#### Cobro de ingresos militares:

* **/sw collect**: como soldado, obtenga los ingresos que le correspondan de: Saquear o Salario militar.

#### Cobrar el reembolso de la nación**:**

* /sw collect: como rey, si su nación es eliminada por cualquier motivo, incluida la captura de su última ciudad, se le reembolsará (80%) del costo de instalación inicial. Este comando cobra ese reembolso.&#x20;

#### Gestionar la ocupación de forma pacífica:

* **/sw nation removeoccupation** - Como rey, elimine pacíficamente la ocupación de una ciudad por parte de su nación.&#x20;
* /sw nation transferoccupation - Como rey, invita a otra nación a ocupar pacíficamente una ciudad que ocupas actualmente.&#x20;
* /sw town inviteoccupation - Como alcalde, invita a una nación a ocupar pacíficamente tu ciudad.

### Hacer la ciudad pacífica

* /t toggle peaceful: como alcalde, declara que tu ciudad es pacífica. La paz hará que su ciudad sea completamente inmune a los ataques de asedio y, a cambio, puede ser ocupado pacíficamente por naciones poderosas cercanas. ADVERTENCIA: No active esta función a menos que esté preparado para aceptar las desventajas, incluida la posibilidad de Ocupación pacífica.
* Tiempo de confirmación:&#x20;
  * El estado se confirmará en 5 días (o 2 si la ciudad es nueva).&#x20;
* Ventajas:&#x20;
  * La ciudad es inmune a los asedios.&#x20;
* Desventajas:&#x20;
  * La ciudad no puede mover el bloque de origen.&#x20;
  * Los residentes no pueden recibir rangos nacionales-militares.&#x20;
  * Los residentes se ven afectados por la enfermedad de guerra si entran en una zona de asedio.&#x20;
  * La ciudad puede ser ocupada pacíficamente, siguiendo las siguientes reglas:

> 1. Por cada pueblo pacífico, cada \*\* pueblo guardián \*\* dentro de 75 cuadras ejerce \*\* influencia \*\* en el pueblo pacífico.
>    * Una ciudad guardiana es cualquier ciudad no pacífica de una nación, de tamaño 30 bloques de ciudades (configurables) o más.
>    * Una ciudad guardiana ocupada ejerce influencia sobre su ocupante, no sobre su nación de origen.
>    * La fuerza de influencia de cualquier ciudad guardiana es igual a su número de cuadras.
> 2. Si la ciudad pacífica tiene una nación, las influencias de la nación de origen y las naciones enemigas extranjeras se amplifican enormemente, de tal manera que siempre serán más fuertes que las influencias de naciones extranjeras no enemigas.
> 3. Posibles resultados:
>    * Si hay influencia sobre la ciudad pacífica, la ciudad quedará desocupada.
>    * Si la influencia más fuerte pertenece a la nación de origen de la ciudad pacífica, la ciudad quedará desocupada.&#x20;
>    * Si la influencia más fuerte pertenece a una nación extranjera, la ciudad será ocupada pacíficamente por esa nación.

#### Hacer que la ciudad no sea pacífica:&#x20;

* /t toggle peaceful: como alcalde, declara que tu ciudad no es pacífica.&#x20;
* Tiempo de confirmación:&#x20;
  * El estado se confirmará en 5 días (o 2 si la ciudad es nueva).&#x20;
* Efectos:&#x20;
  * La paz y todos sus efectos serán eliminados.&#x20;
  * La ocupación NO se eliminará.&#x20;
  * Cualquier ocupante que tuviera la ciudad, antes de volverse pacífico, será restaurado.&#x20;

#### Gestionar la paz de la nación

* Si todas las ciudades de una nación son pacíficas, la nación se considera pacífica.

