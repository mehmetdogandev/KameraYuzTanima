# 📚 Documentation Index / Dokümantasyon İndeksi

Welcome to the documentation section! All detailed guides and references are organized here.

Dokümantasyon bölümüne hoş geldiniz! Tüm detaylı rehberler ve referanslar burada düzenlenmiştir.

---

## 📖 Available Documents / Mevcut Dökümanlar

### 🇹🇷 Turkish Documentation (Türkçe Dökümanlar)

All documentation is currently available in Turkish. English translations coming soon!

#### 1. [📘 README_SCREEN.md](README_SCREEN.md) - Complete Feature Guide
**Tam Özellik Rehberi**

Bu dokümanda bulacaklarınız:
- ✨ OLED ekran sistemi özellikleri
- 📋 Gereksinimler (Arduino kütüphaneleri ve Python paketleri)
- 🔌 Donanım bağlantı şeması
- ⚙️ Kurulum adımları
- 🌐 API kullanım kılavuzu
- 🐍 Python entegrasyon örnekleri
- 🎨 Ekran düzeni ve tasarımı
- 🔧 Sorun giderme
- 🎯 Performans bilgileri

**Best for:** Understanding all features and API details
**En iyisi:** Tüm özellikleri ve API detaylarını öğrenmek için

---

#### 2. [🔧 KURULUM.md](KURULUM.md) - Step-by-Step Installation
**Adım Adım Kurulum Rehberi**

Bu dokümanda bulacaklarınız:
- 1️⃣ Arduino IDE kütüphane kurulumu
- 2️⃣ Donanım bağlantı talimatları
- 3️⃣ Arduino IDE ayarları (Board, Partition Scheme, vb.)
- 4️⃣ WiFi yapılandırması
- 5️⃣ Kod yükleme prosedürü
- 6️⃣ IP adresi bulma
- 7️⃣ Test prosedürleri
- 8️⃣ Sorun giderme (detaylı)
- 9️⃣ Başarı kriterleri

**Best for:** First-time setup and installation
**En iyisi:** İlk kurulum ve yükleme için

---

#### 3. [🔌 BAGLANTI_SEMASI.md](BAGLANTI_SEMASI.md) - Wiring Diagrams
**Detaylı Bağlantı Şemaları**

Bu dokümanda bulacaklarınız:
- 🔌 OLED SSD1306 bağlantı şeması
- 📊 Detaylı bağlantı tablosu
- ⚠️ Voltaj seçimi (3.3V vs 5V)
- 🔍 I2C adres kontrolü ve tarama
- 🎯 Alternatif pin seçenekleri
- 📸 Sistem mimarisi diyagramı
- 🔧 Fiziksel bağlantı kontrol listesi
- 🛠️ Donanım sorun giderme
- ✅ Final checklist

**Best for:** Hardware connection and troubleshooting
**En iyisi:** Donanım bağlantısı ve sorun giderme için

---

#### 4. [📝 DEGISIKLIKLER.md](DEGISIKLIKLER.md) - Change Log
**Kod Değişiklikleri ve Modifikasyonlar**

Bu dokümanda bulacaklarınız:
- 📁 Değiştirilen dosyalar listesi
- ➕ Eklenen kod parçaları
- 🔄 Modifiye edilen fonksiyonlar
- 📄 Yeni oluşturulan dosyalar
- 🔌 API özellikleri detayları
- 🎨 Ekran düzeni açıklaması
- ⚙️ Donanım gereksinimleri
- 🚀 Hızlı başlangıç özeti
- ✅ Garanti edilen özellikler
- 🎯 Kullanım senaryoları

**Best for:** Understanding code changes and architecture
**En iyisi:** Kod değişikliklerini ve mimariyi anlamak için

---

## 🗺️ Documentation Roadmap / Dokümantasyon Yol Haritası

### For New Users / Yeni Kullanıcılar İçin

1. **Start Here:** [KURULUM.md](KURULUM.md) - Install everything
2. **Then:** [BAGLANTI_SEMASI.md](BAGLANTI_SEMASI.md) - Connect hardware
3. **Next:** [README_SCREEN.md](README_SCREEN.md) - Learn API usage
4. **Finally:** Test with Python scripts in root directory

### For Developers / Geliştiriciler İçin

1. **Architecture:** [DEGISIKLIKLER.md](DEGISIKLIKLER.md) - Code structure
2. **API Details:** [README_SCREEN.md](README_SCREEN.md) - HTTP endpoints
3. **Hardware:** [BAGLANTI_SEMASI.md](BAGLANTI_SEMASI.md) - Pin assignments
4. **Integration:** Check `advanced_screen_control.py` examples

### For Troubleshooting / Sorun Giderme İçin

1. **Hardware Issues:** [BAGLANTI_SEMASI.md](BAGLANTI_SEMASI.md)
2. **Installation Problems:** [KURULUM.md](KURULUM.md)
3. **API Errors:** [README_SCREEN.md](README_SCREEN.md)
4. **General Help:** All documents have troubleshooting sections

---

## 📖 Quick Reference / Hızlı Referans

### Hardware Connection / Donanım Bağlantısı
```
OLED Pin    →    ESP32 Pin
────────────────────────────
VCC         →    3.3V
GND         →    GND
SDA         →    D10
SCL         →    D11
```

### API Endpoint / API Uç Noktası
```
POST http://[ESP32_IP]/screen

Parameters:
  data: 0 (LEFT) | 1 (RIGHT) | 2 (BOTH)
  status: 0 (INCREMENT) | 1 (DECREMENT)
```

### Python Quick Test / Python Hızlı Test
```python
import requests
url = "http://192.168.1.100/screen"
requests.post(url, data={'data': 0, 'status': 0})
```

---

## 🔍 Search Guide / Arama Rehberi

Looking for something specific? Here's where to find it:

### Installation & Setup
- **Arduino libraries** → [KURULUM.md](KURULUM.md) §1
- **WiFi configuration** → [KURULUM.md](KURULUM.md) §4
- **Upload settings** → [KURULUM.md](KURULUM.md) §3

### Hardware
- **Wiring diagram** → [BAGLANTI_SEMASI.md](BAGLANTI_SEMASI.md) §1
- **I2C address** → [BAGLANTI_SEMASI.md](BAGLANTI_SEMASI.md) §2
- **Pin alternatives** → [BAGLANTI_SEMASI.md](BAGLANTI_SEMASI.md) §4

### API & Software
- **HTTP POST examples** → [README_SCREEN.md](README_SCREEN.md) §5
- **Python integration** → [README_SCREEN.md](README_SCREEN.md) §7
- **Response format** → [README_SCREEN.md](README_SCREEN.md) §6

### Troubleshooting
- **OLED not working** → [BAGLANTI_SEMASI.md](BAGLANTI_SEMASI.md) §7
- **WiFi issues** → [KURULUM.md](KURULUM.md) §8
- **Compilation errors** → [KURULUM.md](KURULUM.md) §8

### Code Details
- **Modified files** → [DEGISIKLIKLER.md](DEGISIKLIKLER.md) §1
- **New functions** → [DEGISIKLIKLER.md](DEGISIKLIKLER.md) §2
- **API implementation** → [DEGISIKLIKLER.md](DEGISIKLIKLER.md) §3

---

## 💡 Tips & Tricks / İpuçları ve Püf Noktaları

### 🎯 Most Common Mistakes / En Yaygın Hatalar

1. **Forgetting Partition Scheme**
   - Must set "Huge APP" in Arduino IDE
   - → See [KURULUM.md](KURULUM.md) §3

2. **Wrong I2C Address**
   - Default is 0x3C, some use 0x3D
   - → See [BAGLANTI_SEMASI.md](BAGLANTI_SEMASI.md) §2

3. **WiFi Credentials**
   - SSID is case-sensitive
   - → See [KURULUM.md](KURULUM.md) §4

4. **Wrong IP Address**
   - Check Serial Monitor at 115200 baud
   - → See [KURULUM.md](KURULUM.md) §6

### ⚡ Pro Tips / Uzman İpuçları

- **Use USB 2.0 ports** for more stable uploads
- **Keep wires short** (<20cm) for I2C stability
- **Test camera first** before adding OLED
- **Monitor Serial output** during development
- **Use Python controller** for easy integration

---

## 📞 Getting Help / Yardım Alma

### Before Asking / Soru Sormadan Önce

1. ✅ Read the relevant documentation above
2. ✅ Check Serial Monitor (115200 baud)
3. ✅ Verify hardware connections
4. ✅ Try the troubleshooting sections

### When Reporting Issues / Sorun Bildirirken

Please include:
- 📋 Which document you followed
- 🖥️ Serial Monitor output
- 🔌 Hardware configuration
- 💻 Code modifications (if any)
- ⚠️ Error messages

---

## 🌟 Contributing to Documentation / Dokümantasyona Katkı

Want to improve these docs? We welcome:

- 🌍 Translations (English, etc.)
- 📸 Photos and diagrams
- 🐛 Corrections and clarifications
- 💡 Additional examples
- 🎨 Better formatting

See main [README.md](../README.md) for contribution guidelines.

---

## 📅 Documentation Version / Dokümantasyon Versiyonu

- **Last Updated:** November 2025
- **Version:** 1.0
- **Language:** Turkish (Türkçe)
- **Status:** Complete and tested

---

**🏠 [Back to Main README](../README.md)**

*Happy making! / İyi projeler!* 🚀
