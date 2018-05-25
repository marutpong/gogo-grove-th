# 3.1 Sensors Provided in the GoGo Board Kit

## Lever Switches and Buttons {#lever-switches-and-buttons}

![](https://lh6.googleusercontent.com/XXhoiviM0cP9LWZSgzPx0pWmHF0x-tR4V8OhTWUseZfxY3xGaHsyGhh-O5gTvfPI-BFfGeMEibbzyN9AMxTOgTI_vG4uYLYIu8t6anoM7GqdF8GhQbq1BX0YVVc38N52Md8o0loC)

Lever switches and buttons are similar. They both produce a high value readout when pressed and become near zero when released. Lever switches \(also called limit switches\) are suitable for detecting objects such as walls, balls, and other mechanical parts. Buttons, on the other hand, are usually for humans to press.

## Button Set {#button-set}

![](https://lh5.googleusercontent.com/VUuiVQfDIceaurA8ryCCKjCOdan_ojwqc-Ogk9oiTRG6wBkPoh3-9_3EjxNkxEgRUqDUo_AL_sG_9mdyHAXpLfrVwb0iCmKGt-oUY4JY7gBwwPLyMTdp5RJ7jfbck4nPfMl6uJOx)

Useful as a game or motion controller, the button set produces different readouts for each button.

## Light Sensor \(LDR\) {#light-sensor}

![](https://lh5.googleusercontent.com/Rmta4SQ9rb1CuqJC9vY8uw2z4zgpFS7AN6q9hSuqbtxWINkbDGAognrPA6hnccv69Y8ekl-TX3fxjedsuwo3xmHmx09xpjsnYAJB_OJgzHxJvoyNSvG8lybrCexIjteQXqjVuOnZ)

The readout value varies according to the amount of light the sensor receives.

## Temperature Sensor {#temperature-sensor}

![sensor temperature.png](https://lh4.googleusercontent.com/GgtVOBlhdmGlF5LMSz3Avz-HLId9joXpfCZim2qFtt0QcdBQ25VHQd26BjgpoJD-vrjQtmdlnh5DhBlurrMIGVKLwScvIS4_8jwphbhye3EXrXdJP_gFW9FFYLhtqAdA9J5Dwn5j)

The readout value corresponds to the ambient temperature. Note that the readout is not in Celsius or Fahrenheit. The value is reflects the resistance of the sensor. Mappings between the resistance and the standard units must be done manually.

## Magnetic Sensor {#magnetic-sensor}

![](https://lh6.googleusercontent.com/CQGNhkdfH75drhz385lKoW1OglalqJBSMLQhiySijjqP--X6O6tu1wlXJOunjBo812kH5iarjZ3BdrSkZTjiJ4qFYrz-Be1pFbg5Ih_bgaO-koYnUkgcByjTe5c2BLh3POmkZuE5)

Magnetic sensors are sensitive to magnetic fields such as those produced by magnets.

Magnetic sensors are often used as a non-contact switch. For example, to measure the speed of a bicycle, a magnetic sensor can be placed on the wheel’s frame. A magnet is stuck on to the wheel. With this setup, the magnetic sensor will detect the magnet every time it passes by. Measuring the time between counts can be later used to calculate the bicycle’s speed.

## Infrared Reflective Sensor {#infrared-reflective-sensor}

![](https://lh6.googleusercontent.com/9bqUi-qv_uhq71zSn1qe5G5Q2os-9ULuRJx4bYSiWGFkwLS6zst3X9RLamf2FFtss5Z84vbJSwBFot1EuPXAiKHHl78HWCK0QvImOj_90SzTNkjAKNDW9R7ATZbA-Ty3MOQCzG-f)

This sensor is commonly used to measure proximity. It emits infrared light and measures how much of that light is reflected back. Therefore, if there is no object to bounce back the light, the sensor will give a small measurement. The closer an object is to the sensor, the higher the measurement. The effective range of this sensor is less than 5 centimeters. Note that color of the object also determines how much light is reflected. For example, black objects absorbs more light than lighter colors and, at the same distance, produces a lower measurement. Therefore, this sensor can also be adapted as a color sensor.

> **Caution** - This sensor is sensitive to infrared light from other sources as well. Therefore, the interference of sunlight, fluorescent light or other infrared light sources may lead to irregular readings.

## Rain Sensor {#rain-sensor}

![sensor rain.png](https://lh6.googleusercontent.com/CfP5LQKjRSXzFGOnuqzSghzV4rAUu6DPD7DwLa5ZfnhmXN8CpqvpPtg5rDMCYnX90mYWqtnHv-SApJSrw7jd4kprxunTzj0wi4qAgi-3HP3QB5qRG6e1Uy38ju5tB-EuAfmII9am)

The metal below this sensor is very sensitive to raindrops. In the event of a rainfall, it is best to turn this side up for direct rainfall detection. Make sure to keep the connector dry.

## Soil Humidity Sensor {#soil-humidity-sensor}

![](https://lh5.googleusercontent.com/ShjcJG_JzPDLen6CHoZZ4e0Sj32jGRE9LkxeuEOF3dj6xbNRnLBs99zIflF2-HfLuEQvP3Mxs25vxdhhigT3l7XoaJ09EYUyPRfVp_y9uOvdiCScQY8JnIfMLVQ_Ea48FmfoWtS4)

Under this sensor lies 2 metal plates to measure soil humidity or moisture in the soil. After inserting the probe into the soil, make sure the connector stays dry for an accurate readout.

## Terminal Connector {#terminal-connector}

![](https://lh6.googleusercontent.com/BsDQ0Lmmj7k9reFACTEsyOA4DZzNWpNU4UPFLcLUXE90ZmSS-JHGJHknNh9i-nWG90HLG6i3DOGQdDADIxE3sIH4rUigGNeczo-xpQE5f32wpqlR7wWbCZlke0e652HwQEYGV5Og)

This terminal connector is used for additional sensors that are not included in this kit. Three screws in the adapter are used for power, ground, and signal \(VCC, GND, Sig\).

