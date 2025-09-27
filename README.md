# Emotional Helper App (EmoCare)
Mobile application combining Artificial Intelligence, IoT, and Computer Vision to detect emotions and provide real-time support for students under academic pressure.

---

## Main Features
- Mobile app built with **React Native + Firebase**, integrating **OpenAI API** and **Google TTS**.  
- CNN trained with **30,000+ images in Keras** for facial emotion recognition.
    - [Facial Emotion Recognition CNN Repository](https://github.com/DanielaRochaMunoz/Facial-emotion-recognitionCNN) 
- IoT device (**ECG + NodeMCU**) sending heart rate data every 7 seconds to Firebase.  
- Emotionally personalized responses via **chat and voice**.  
- Strengthened Firebase security with **user authentication** and **granular access rules**.  

---

## Results
- Model accuracy: **~75% in emotion detection**.  
- Dataset: **30,000 labeled images** for training and validation.  
- Validated use cases: **anxiety, academic stress, and social comparison**.  

---

## Tech Stack
- **Languages:** JavaScript, Python  
- **Frameworks/Libraries:** React Native, NestJS, Keras, NumPy, Pandas  
- **Infrastructure:** Firebase, NodeMCU (IoT), Vercel  
- **AI/ML:** Convolutional Neural Networks (CNN) + OpenAI API  
- **Security:** Firebase Auth, access rules, data encryption  

---

## Complementary repositories
This project is composed of **3 main repositories**:  
- **Frontend (React Native App)** → mobile interface, voice recognition, and chat.  
- **Backend (NestJS)** → server logic, OpenAI and Google TTS integration.  
- **Facial Recognition CNN** → Keras CNN for emotion classification.  

---

## Installation & Execution

### 1. Clone repository
```bash
git clone <repo-emocare>
cd emocare
```

### 2. Configure dependencies  

 **Frontend (React Native)**  
```bash
yarn add @react-native-voice/voice
yarn add expo-av
yarn add expo-file-system
```

 **Backend (NestJS)**  
```bash
npm i -g @nestjs/cli
yarn add @google-cloud/text-to-speech
yarn add openai
yarn add dotenv
yarn add cors
```

 **CNN (Keras)**  
```bash
pip install -r requirements.txt
```

---

### 3. Environment variables (.env)  
```env
OPENAI_API_KEY=your_api_key
GOOGLE_TTS_KEY=your_api_key
FIREBASE_API_KEY=your_api_key
```

---

### 4. Database (Firebase)
- Configure **Firebase Authentication**.  
- Define **security rules** to restrict sensitive data access.  
- Connect the app with **google-services.json**.  

---

### 5. Run app  

 **Frontend (React Native)**  
```bash
npx expo start
```

 **Backend (NestJS)**  
```bash
npm run start:dev
```

 **CNN**  
```bash
python train.py
python predict.py --image test.jpg
```

---

##  Data Security
- **Firebase Auth** → user authentication.  
- **Access rules** → granular sensitive data control.  
- **Secure IoT** → NodeMCU sends encrypted data to Firebase.  

---

##  Use Cases
- Students with **social anxiety** during presentations.  
- Youth under **high academic pressure**.  
- Situations of **comparison and isolation**.  
