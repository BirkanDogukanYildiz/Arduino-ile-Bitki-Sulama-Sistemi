Bağlantılar:

Arduino Uno:
5V → Röle VCC
5V → Nem Sensörü VCC
GND → Röle GND
GND → Nem Sensörü GND
A0 → Nem Sensörü A0
D2 → Röle IN
Opsiyonel ---> USB → Bilgisayar (güç + seri monitör). Bu sayede toprak nem sensörü kalibrasyonu yapabilirsiniz.

Röle:
VCC → Arduino 5V
GND → Arduino GND
IN → Arduino D2
COM → Pompa (+)
NO → Pil yatağı (+)

Pil Yatağı (3x AA = 4.5V):
(+) → Röle NO
(-) → Pompa (-)

Pompa:
(+) → Röle COM
(-) → Pil yatağı (-)

Nem Sensörü:
VCC → Arduino 5V
GND → Arduino GND
A0 → Arduino A0
