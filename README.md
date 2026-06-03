## Açıklama
Projenin kodlar kısmında "#define ESIK" kısmında ESIK yanındaki sayıyı kendi verilerinize göre kalibre ederek su pompasının çalışmasını sağlayabilirsiniz. Toprak nem sensöründen veriler gelir ve ESIK'i geçerek su pompasının çalışmasını sağlamaktadır.

Röle olarak röle modülü kullanılmıştır. Projenin şematik gösteriminde röle modül olarak olmadığı için kendi tasarladığım bir röle modülü bulunmakta. Ancak bunla uğraşmak yerine direkt modül almanızı tavsiye ederim.  

## 🔌 Bağlantı Şeması

### Arduino Uno
| Pin | Bağlantı |
|-----|----------|
| 5V  | Röle VCC |
| 5V  | Nem Sensörü VCC |
| GND | Röle GND |
| GND | Nem Sensörü GND |
| A0  | Nem Sensörü A0 |
| D2  | Röle IN |
| Opsiyonel: USB | Bilgisayar (güç + seri monitör). Bu sayede toprak nem sensörü kalibrasyonu yapabilirsiniz. |

### Adaptör
| Pin | Bağlantı |
|-----|----------|
| 12V  | Arduino Adaptör Girişi |

### Röle
| Pin | Bağlantı |
|-----|----------|
| VCC | Arduino 5V |
| GND | Arduino GND |
| IN  | Arduino D2 |
| COM | Pompa (+) |
| NO  | Pil Yatağı (+) |

### Toprak Nem Sensörü
| Pin | Bağlantı |
|-----|----------|
| VCC | Arduino 5V |
| GND | Arduino GND |
| A0  | Arduino A0 |

### Pil Yatağı (3x AA = 4.5V)
| Pin | Bağlantı |
|-----|----------|
| (+) | Röle NO  |
| (-) | Pompa (-) |

### Dalgıç Su Pompası
| Pin | Bağlantı |
|-----|----------|
| (+) | Röle COM |
| (-) | Pil Yatağı (-) |

