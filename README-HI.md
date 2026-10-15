# Jan Samarth Vote — जन समर्थन वोट

यह GitHub Pages के लिए हिंदी + English में responsive static frontend है।

## इसमें क्या काम करता है?
- मोबाइल-फ्रेंडली होम पेज, पोल कार्ड और खोज
- पोल बनाना (केवल उसी ब्राउज़र में)
- वोटिंग और परिणाम का डेमो (केवल उसी ब्राउज़र में)
- शेयर लिंक/WhatsApp शेयर करने का प्रयास
- अनौपचारिक सर्वे का स्पष्ट डिस्क्लेमर

## महत्वपूर्ण सीमा
यह अभी **डेमो फ्रंटएंड** है। `localStorage` के कारण अलग-अलग लोगों के वोट आपस में साझा नहीं होते; उपयोगकर्ता ब्राउज़र डेटा मिटाकर फिर वोट भी दे सकता है। इसे वास्तविक सार्वजनिक चुनावी सर्वे की तरह प्रस्तुत न करें। सार्वजनिक उपयोग से पहले डेटाबेस/बैकएंड, rate limiting, duplicate-abuse protections, privacy notice, moderation और सुरक्षा परीक्षण जोड़ें।

## GitHub Pages पर प्रकाशित करें
1. GitHub में `jan-samarth-vote` repository खोलें।
2. `Add file` → `Upload files` चुनें।
3. `index.html`, `style.css`, `app.js`, `README-HI.md` अपलोड करें। (ZIP को सीधे upload करना पर्याप्त नहीं है; पहले extract करें।)
4. नीचे `Commit changes` दबाएँ।
5. Repository में `Settings` → `Pages` खोलें।
6. `Build and deployment` में `Deploy from a branch` चुनें।
7. Branch `main`, folder `/(root)` चुनें और `Save` दबाएँ।
8. कुछ मिनट बाद Pages स्क्रीन पर दिखने वाला URL खोलें।

## सार्वजनिक वोटिंग के लिए अगला चरण
Supabase या किसी अन्य backend पर server-side vote recording, row-level security, validation, rate limits और anti-abuse protections configure करें। **कभी भी service-role/secret key को HTML या JavaScript में न रखें।** केवल public/anon key को भी सही RLS policies के साथ ही इस्तेमाल करें।

## चुनाव संबंधी जिम्मेदार उपयोग
- पोल को अनौपचारिक जनमत के रूप में लेबल करें।
- आधिकारिक नतीजों के रूप में पोल परिणाम न दिखाएँ।
- चुनाव तारीख/उम्मीदवार/नतीजे प्रकाशित करने से पहले आधिकारिक स्रोतों से पुष्टि करें।
- उम्मीदवारों के बारे में आरोपों या भ्रामक दावों को बिना विश्वसनीय प्रमाण प्रकाशित न करें।
- यह साइट किसी सरकारी चुनाव प्राधिकरण से संबद्ध नहीं है।
