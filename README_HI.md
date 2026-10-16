# Neeraj AI — अगला शुरुआती वर्ज़न

यह Android Studio / GitHub Actions से APK बनाने वाला starter project है। इसमें हिंदी speech-to-text बटन, हिंदी text-to-speech, समय/तारीख, और YouTube/Google/Maps खोलने की कमांड हैं।

## जरूरी ईमानदार सीमा
- यह वर्ज़न **हमेशा बैकग्राउंड में “Hey Neeraj” सुनता नहीं है**। ऐप खोलकर माइक दबाना होगा।
- Android सुरक्षा के कारण यह PIN/pattern/password को bypass नहीं करता और आवाज़ के आधार पर सुरक्षित फोन अनलॉक नहीं करता।
- फोन लॉक होने पर voice assistant चलाना Android के default assistant role, device support और OS permissions पर निर्भर है; यह starter app अभी default assistant service नहीं है।
- AI मॉडल/API अभी कनेक्ट नहीं है; अनजान सवालों पर यह सीमित कमांड वाला जवाब देगा।
- यह debug APK बनाने का source project है, पहले से तैयार APK नहीं।

## फोन से APK बनाना
1. ZIP extract करें।
2. GitHub पर नया repository बनाएँ और सभी files upload करें।
3. Actions tab में `Build Neeraj AI APK` workflow चलाएँ।
4. Build सफल होने पर `NeerajAI-debug-apk` artifact डाउनलोड करें।
5. ZIP extract करके `app-debug.apk` इंस्टॉल करें। केवल अपने बनाए/विश्वसनीय APK को इंस्टॉल करें।

## स्थानीय बिल्ड
Android Studio में project खोलें और `assembleDebug` चलाएँ।
