# Pràctiques

# Fitxa tècnica: Instal·lació i configuració d'un sensor de temperatura

## Objectiu

Configurar un sensor de temperatura digital en una placa Arduino Uno per llegir dades ambientals en temps real i enregistrar la informació.

## Materials

Placa Arduino Uno
Sensor de temperatura DHT11
Cables jumper mascle-mascle
Resistència de 4.7k Ω

## Procediment

Connectar el pin VCC del sensor al pin de 5V de l'Arduino.
Connectar el pin GND del sensor al pin GND de l'Arduino.
Connectar el pin de dades al pin digital 2 de l'Arduino.
Carregar el programa de lectura mitjançant la següent comanda de terminal:

arduino-cli compile --upload -p /dev/ttyACM0 --fqbn arduino:avr:uno

## Comprovacions

[ ] El LED d'alimentació de la placa està encès.
[ ] La placa és reconeguda al port corresponent.
[ ] Les lectures de temperatura s'actualitzen correctament.

## Incidències i solucions

| Incidència | Solució |
|---|---|
| Error de connexió al port COM | Reconnectar el cable USB i seleccionar el port a Eines > Port. |
| Valors incorrectes o absents | Comprovar la resistència i les connexions dels pinyons. |

## Flux de Treball amb Git

El flux de treball utilitzat per al control de versions d'aquesta fitxa tècnica segueix els següents passos:
1. Creació d'estructura: Definició dels apartats principals.
2. Desenvolupament de contingut: Inclusió del procediment, comprovacions i recursos gràfics.
3. Revisió de format: Validació de les taules, enllaços i blocs de codi.
4. Sincronització: Registre de canvis mitjançant commits locals i enviament al repositori remot (origin/main).

## Recursos

- [Documentació consultada](https://docs.arduino.cc/)
