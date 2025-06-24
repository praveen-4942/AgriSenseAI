

# AgriSenseAI 🌾📡

AgriSenseAI is a smart farming system that uses sensor data and AI models to detect crop diseases and pests while monitoring environmental conditions. The system automates notifications using Twilio to help farmers make better, faster decisions about irrigation and plant health.

## 📌 Features

- 🌡️ Real-time monitoring using DHT11 and Soil Moisture sensors  
- 🌿 AI-driven tomato disease detection (9 classes)  
- 🐛 AI-based pest classification (9 classes)  
- 🖼️ HSV-based image preprocessing for better inference accuracy  
- 📲 Twilio-based SMS alerts to farmers  
- 🔄 Continuous monitoring loop via Raspberry Pi  

## ⚙️ Hardware

- Raspberry Pi 4B  
- DHT11 Temperature and Humidity Sensor (GPIO 27)  
- Soil Moisture Sensor (GPIO 4)  
- USB or Pi Camera  
- Internet connectivity (for Twilio SMS)  

## 🧠 Software Stack

- Python 3  
- TensorFlow / Keras  
- OpenCV  
- NumPy  
- Twilio SDK  
- RPi.GPIO  
- dht11 Python module  

## 📦 Installation

```bash
pip install tensorflow keras opencv-python numpy twilio RPi.GPIO
```

## 🚀 How to Run

1. Place your trained models (`tomato.h5` and `pest.h5`) inside the `/my_project/` directory  
2. Replace Twilio credentials in the script  
3. Connect sensors and the camera to Raspberry Pi  
4. Run the script:

```bash
python3 agrisenseai.py
```

## 🔍 Sample Output

```
Soil moisture: 1 (Dry)
Temperature: 30.6°C
Humidity: 72.1%
Predicted Disease: Tomato_Leaf_Mold (Confidence: 92.3%)
Predicted Pest: Aphid (Confidence: 89.1%)
```

## 📲 Sample SMS

```
SMART AGRICULTURAL MONITORING SYSTEM
Soil moisture : 1
Temperature : 30.6°C
Humidity : 72.1%
predicted_disease1 : Tomato_Leaf_Mold
```

## 🛠️ Future Enhancements

- Automated irrigation control  
- Dashboard for live visualization (Flask/React)  
- Weather API integration  
- Multi-crop detection support  
- Localized language support for SMS  

## 🙌 Developer

Developed with ❤️ by Praveen  
[GitHub](https://github.com/) • [LinkedIn](https://www.linkedin.com/) • [Email](mailto:your.email@example.com)

---

> “Harvesting data to nourish the future.”
```

If you need a flowchart, logo, or even a contributor badge pack to add some flair to the repo, I’ve got you covered!
