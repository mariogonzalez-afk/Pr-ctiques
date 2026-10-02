# Pràctiques

# Fitxa tècnica: Instal·lació i configuració d'un sensor de temperatura

![Sensor de Temperatura](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTnOq4r9kkQfQS6JI4o9aHg52QDW5hn2E4YqDDGnhP18Q&s=10)

## Objectiu

Configurar un sensor de temperatura digital en una placa Arduino Uno per llegir dades ambientals en temps real i enregistrar la informació.

## Materials

- Placa Arduino Uno
- Sensor de temperatura DHT11
- Cables jumper mascle-mascle
- Resistència de 4.7k Ω

## Procediment

1. Connectar el pin VCC del sensor al pin de 5V de l'Arduino.
2. Connectar el pin GND del sensor al pin GND de l'Arduino.
3. Connectar el pin de dades al pin digital 2 de l'Arduino.
4. Carregar el programa de lectura mitjançant la següent comanda de terminal:

```bash
arduino-cli compile --upload -p /dev/ttyACM0 --fqbn arduino:avr:uno
```

## Comprovacions

- [ ] El LED d'alimentació de la placa està encès.
- [ ] La placa és reconeguda al port corresponent.
- [ ] Les lectures de temperatura s'actualitzen correctament.

## Incidències i solucions

| Incidència | Solució |
|---|---|
| Error de connexió al port COM | Reconnectar el cable USB i seleccionar el port a Eines > Port. |
| Valors incorrectes o absents | Comprovar la resistència i les connexions dels pinyons. |


## Recursos

- [Documentació consultada](https://docs.arduino.cc/)
