# Pràctiques

# Fitxa tècnica: Instal·lació i configuració d'un sensor de temperatura amb Arduino

## Objectiu

Configurar un sensor de temperatura digital en una placa Arduino Uno per llegir dades ambientals en temps real i mostrar-les a través del monitor sèrie.

## Materials

- Placa Arduino Uno
- Cable USB Tipus A/B
- Protoboard (placa de proves)
- Sensor de temperatura DHT11
- 3 cables jumper mascle-mascle
- Resistència de 4.7k Ω

## Procediment

1. Connectar el pin VCC del sensor al pin de 5V de l'Arduino.
2. Connectar el pin GND del sensor al pin GND de l'Arduino.
3. Col·locar la resistència entre el pin VCC i el pin de dades del sensor.
4. Connectar el pin de dades del sensor al pin digital 2 de l'Arduino.
5. Connectar la placa a l'ordinador, obrir l'IDE d'Arduino i pujar el programa de lectura.

## Comprovacions

- [ ] El LED d'alimentació de la placa Arduino està encès.
- [ ] L'IDE d'Arduino reconeix el port COM assignat.
- [ ] El monitor sèrie mostra lectures de temperatura actualitzades.

## Incidències i solucions

|                   Incidència                 |                            Solució                             |
|----------------------------------------------|----------------------------------------------------------------|
| Error de comunicació amb el port COM         | Reconnectar el cable USB i seleccionar el port a Eines > Port. |
| Lectures de temperatura incorrectes o a 0 ºC | Comprovar les connexions i la resistència entre VCC i Dades.   |

## Recursos

- [Documentació consultada](https://docs.arduino.cc/)
