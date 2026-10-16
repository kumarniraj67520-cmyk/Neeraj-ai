# Niraj AI Android (शुरुआती संस्करण)

यह Android ऐप बिना AI API key के लोकल कमांड चलाता है:
- हिंदी UI
- Android speech recognition (माइक अनुमति के बाद)
- Text-to-speech
- समय/तारीख, YouTube, Google, Maps खोलना
- ऐप खुला रहने तक साधारण रिमाइंडर

यह अभी ChatGPT-जैसा ऑनलाइन AI नहीं है। उसके लिए बाद में सुरक्षित backend और AI API जोड़नी होगी। API key को Android ऐप में कभी न रखें।

## फोन से APK बनाना
1. GitHub पर नया repository बनाएं।
2. इस ZIP की सारी फ़ाइलें repository में अपलोड करें (root में `settings.gradle.kts` दिखना चाहिए)।
3. GitHub repository में Actions खोलें और `Build Niraj AI APK` workflow चलाएं।
4. Workflow पूरा होने पर `NirajAI-debug-apk` artifact डाउनलोड करें।
5. ZIP artifact खोलें और `app-debug.apk` निकालें।
6. APK खोलें; Android यदि पूछे तो इस स्रोत से इंस्टॉल करने की अनुमति दें।

GitHub Actions इस्तेमाल करने के लिए GitHub अकाउंट और इंटरनेट चाहिए। यह debug APK निजी टेस्टिंग के लिए है, Play Store release नहीं।

## सीमाएँ
- Android speech recognition के लिए डिवाइस पर speech service/इंटरनेट की जरूरत पड़ सकती है।
- रिमाइंडर ऐप खुला रहने पर ही चलता है।
- केवल अनुमत/स्पष्ट कमांड किए जाते हैं; यह पूरे फोन को बिना अनुमति नियंत्रित नहीं करता।
