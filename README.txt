ITI JOB PREP — FULL STARTER PROJECT
===================================

यह प्रोजेक्ट चरण 1 की वेबसाइट और चरण 2–5 के लिए जरूरी शुरुआती फाइलें देता है।
यह अपने-आप इंटरनेट पर प्रकाशित नहीं होता और इसमें अभी लाइव Supabase project credentials नहीं हैं।

फाइलें:
- index.html: मोबाइल-फ्रेंडली वेबसाइट, हिंदी/English, 16 ट्रेड, नमूना CBT टेस्ट, लोकल प्रगति
- manifest.webmanifest: PWA जानकारी
- sw.js: बेसिक offline cache
- supabase/schema.sql: डेटाबेस की शुरुआती टेबल और Row Level Security policies
- android-wrapper/: Android wrapper बनाने के अगले चरण के निर्देश

चरण 1 — वेबसाइट चलाएँ:
1. ZIP Extract करें।
2. index.html ब्राउज़र में खोलकर टेस्ट करें।
3. कुछ मोबाइल ब्राउज़र local file पर service worker/PWA नहीं चलाते; ऑनलाइन होस्टिंग के बाद PWA टेस्ट करें।

चरण 2 — ऑनलाइन प्रकाशित करें:
1. GitHub पर अपना अकाउंट बनाकर एक नया repository बनाएँ।
2. इस फोल्डर की फाइलें repository में upload करें।
3. Repository Settings → Pages में publishing source चुनें।
4. प्रकाशित URL को मोबाइल पर खोलकर टेस्ट करें।
वैकल्पिक: Netlify Drop/अन्य static hosting का इस्तेमाल करें। होस्टिंग सेवा की वर्तमान शर्तें/फ्री सीमा खुद जाँचें।

चरण 3 — ऑनलाइन डेटाबेस:
1. https://supabase.com/ पर अपना project बनाएँ।
2. SQL Editor में supabase/schema.sql की सामग्री चलाएँ।
3. अपनी Project URL और anon/public key प्राप्त करें।
4. frontend में Supabase JS client जोड़ने और data access implement करने का अलग चरण अभी बाकी है।
5. कभी भी service_role/secret key वेबसाइट में न डालें। RLS को बंद न करें।
इस ZIP का front-end अभी Supabase से जुड़ा नहीं है; schema तैयार करना, database connection होना नहीं है।

चरण 4 — प्रश्न और भर्ती:
- ट्रेड के अनुसार प्रश्नों को अलग-अलग सत्यापित करें।
- पुराने प्रश्नपत्रों का उपयोग तभी करें जब वे सार्वजनिक/अनुमत हों; दूसरे ऐप से प्रश्न कॉपी न करें।
- भर्ती की deadline और पात्रता आधिकारिक नोटिफिकेशन से सत्यापित करें।
- लाइव भर्ती अपडेट अभी अपने-आप नहीं आते; उन्हें admin workflow/API से जोड़ना होगा।

चरण 5 — Android:
- इस source में अभी installable APK शामिल नहीं है।
- Android wrapper बनाने के लिए Node.js, Android Studio और Capacitor build setup की जरूरत होगी।
- android-wrapper/README.txt में आगे की प्रक्रिया दी गई है।

अभी पूरा हुआ:
✓ वेबसाइट का front-end demo
✓ हिंदी/English switch
✓ 16 ट्रेड सेक्शन
✓ sample quiz, score और browser-local progress
✓ official job portal links
✓ PWA manifest/service worker starter
✓ Supabase database schema starter

अभी बाकी:
- वास्तव में ऑनलाइन deploy करना (आपके अपने account से)
- Supabase से frontend जोड़ना
- secure admin login/roles
- live recruitment verification/update workflow
- full trade-wise question bank
- APK build/signing

सुरक्षा:
- कोई पासवर्ड, OTP, service-role key या निजी account credential चैट में न भेजें।
- लाइव करने से पहले access rules और प्रश्नों की शुद्धता की जाँच करें।
