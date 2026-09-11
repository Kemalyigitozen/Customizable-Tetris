ENGLISH
## 🛠️ Installation and Setup Guide
First open the Tetris file 

Follow the steps below to build and run this project on your own hardware.

### 1. Installing Required Libraries
To ensure the graphics and game dynamics run smoothly, you need to install the **Adafruit** libraries via the Arduino IDE.

1. Open the Arduino IDE.
2. Go to **Sketch** > **Include Library** > **Manage Libraries...** from the top menu.
3. Use the search bar to find and install the following libraries:
   * **Adafruit GFX Library:** For basic graphics and shape drawing.
   * **Adafruit ILI9341:** The hardware driver for the TFT display.

### 2. Circuit Setup and Wiring
Proper wiring between the Raspberry Pi Pico, the ILI9341 display, and the control buttons is crucial for the components to communicate.
<img width="852" height="514" alt="Pin" src="https://github.com/user-attachments/assets/f58f4595-604c-482c-ab53-4f9fd835ddb9" />
Please wire the circuit on your breadboard exactly as shown in the **pinout diagram** provided in this repository. The basic logic is as follows:
* **ILI9341 Display:** Connect the SPI pins (SCK, MOSI, CS, etc.) to the corresponding SPI pins on the Pico, and VCC to the 3.3V output, as indicated in the diagram.
* **Control Buttons:** Connect one leg of the movement (Right, Left, Down) and rotate buttons to the specified Pico GPIO pins, and the other leg directly to the common GND (Ground) line. (Internal Pull-Up resistors are enabled in the code).

### 3. Uploading the Code
1. Once the wiring is complete according to the schematic, connect your Raspberry Pi Pico to your computer using a USB cable.
2. In the Arduino IDE, make sure you have selected the correct board (Raspberry Pi Pico) and the corresponding Port.
3. Open the main project code and click the **Upload** button.
4. Once the upload is complete, the screen will boot up and the game will be ready to play!

<img width="1884" height="2272" alt="Gemini_Generated_Image_nr6orvnr6orvnr6o" src="https://github.com/user-attachments/assets/ca7fb15c-190c-4a61-a403-da76195b70e4" />

Contact me if there is a problem.
/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
TÜRKÇE
## 🛠️ Kurulum ve Kullanım Adımları

Bu projeyi kendi donanımınızda çalıştırmak için aşağıdaki adımları sırasıyla izleyebilirsiniz.

### 1. Gerekli Kütüphanelerin Kurulumu
Ekrandaki grafiklerin ve oyun dinamiklerinin sorunsuz çalışması için Arduino IDE üzerinde **Adafruit** kütüphanelerine ihtiyacımız var. 

1. Arduino IDE'yi açın.
2. Üst menüden **Taslak (Sketch)** > **library ekle (Include Library)** > **Kütüphaneleri Yönet (Manage Libraries)** seçeneğine tıklayın.
3. Arama çubuğunu kullanarak aşağıdaki kütüphaneleri bulup yükleyin:
   * **Adafruit GFX Library:** Temel grafik ve şekil çizimleri için.
   * **Adafruit ILI9341:** Kullandığımız TFT ekranın donanım sürücüsü.

### 2. Devre Kurulumu ve Kablolama
Raspberry Pi Pico, ILI9341 ekran ve yön/döndürme butonlarının birbiriyle haberleşebilmesi için bağlantıların doğru yapılması çok önemlidir. 

Repoda (proje dosyaları arasında) yer alan **pin şeması görseline** bakarak devre tahtası (breadboard) üzerindeki bağlantıları birebir kurun. Temel mantık şu şekildedir:
* **ILI9341 Ekran:** Şemada belirtilen SPI pinleri (SCK, MOSI, CS vb.) Pico'nun ilgili SPI bacaklarına, VCC ise 3.3V çıkışına bağlanmalıdır.
* **Kontrol Butonları:** Hareket (Sağ, Sol, Aşağı) ve Döndürme butonlarının birer bacağı şemada belirtilen Pico GPIO pinlerine, diğer bacakları ise doğrudan ortak GND (Toprak) hattına bağlanır. (Kod içerisinde dahili Pull-Up dirençleri aktifleştirilmiştir.)

### 3. Kodu Yükleme ve Başlatma
1. Devre bağlantılarını şemaya uygun şekilde tamamladıktan sonra Raspberry Pi Pico'yu USB kablosu ile bilgisayarınıza bağlayın.
2. Arduino IDE üzerinden doğru kartı (Raspberry Pi Pico) ve bağlı olduğu Port'u seçtiğinizden emin olun.
3. Projedeki ana oyun kodunu açıp **Yükle (Upload)** butonuna basın.
4. Yükleme tamamlandığında ekran açılacak ve oyun oynamaya hazır hale gelecektir!

Bir sorun olduğunda bana ulaşın.
