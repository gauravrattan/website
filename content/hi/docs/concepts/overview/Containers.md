---
linktitle: कुबेरनेट्स प्रलेखन
title: कंटेनरों
sitemap:
  priority: 1.0
---

कंटेनरों


आपके द्वारा चलाए जाने वाले प्रत्येक कंटेनर को दोहराया जा सकता है; निर्भरता शामिल होने से मानकीकरण का अर्थ है कि आप इसे जहाँ भी चलाते हैं, वही व्यवहार प्राप्त करते हैं।

कंटेनर अंतर्निहित मेजबान बुनियादी ढांचे से अनुप्रयोगों को अलग करते हैं। यह विभिन्न क्लाउड या OS वातावरणों में परिनियोजन को आसान बनाता है।

कुबेरनेट्स क्लस्टर में प्रत्येक नोड उन कंटेनरों को चलाता है जो उस नोड को सौंपे गए पॉड बनाते हैं। एक पॉड में कंटेनर सह-स्थित होते हैं और एक ही नोड पर चलने के लिए सह-अनुसूचित होते हैं।

कंटेनर छवियां

एक कंटेनर छवि एक रेडी-टू-रन सॉफ़्टवेयर पैकेज है, जिसमें एप्लिकेशन चलाने के लिए आवश्यक सब कुछ शामिल है: कोड और किसी भी रनटाइम की आवश्यकता होती है, एप्लिकेशन और सिस्टम लाइब्रेरी,
और किसी भी आवश्यक सेटिंग्स के लिए डिफ़ॉल्ट मान।

कंटेनर स्टेटलेस और अपरिवर्तनीय होने का इरादा रखते हैं: आपको पहले से चल रहे कंटेनर का कोड नहीं बदलना चाहिए। यदि आपके पास एक कंटेनरीकृत एप्लिकेशन है और परिवर्तन करना चाहते हैं, तो सही 
प्रक्रिया एक नई छवि बनाना है जिसमें परिवर्तन शामिल है, फिर अपडेट की गई छवि से शुरू करने के लिए कंटेनर को फिर से बनाएँ।

कंटेनर रनटाइम

कंटेनर रनटाइम वह सॉफ्टवेयर है जो कंटेनर चलाने के लिए जिम्मेदार होता है।

कुबेरनेट्स कंटेनर रनटाइम जैसे कंटेनरड, सीआरआई-ओ और कुबेरनेट्स सीआरआई (कंटेनर रनटाइम इंटरफेस) के किसी भी अन्य कार्यान्वयन का समर्थन करता है।

आमतौर पर, आप अपने क्लस्टर को पॉड के लिए डिफ़ॉल्ट कंटेनर रनटाइम चुनने की अनुमति दे सकते हैं। यदि आपको अपने क्लस्टर में एक से अधिक कंटेनर रनटाइम का उपयोग करने की आवश्यकता है, तो आप
यह सुनिश्चित करने के लिए पॉड के लिए रनटाइम क्लास निर्दिष्ट कर सकते हैं कि कुबेरनेट्स एक विशेष कंटेनर रनटाइम का उपयोग करके उन कंटेनरों को चलाते हैं।

आप एक ही कंटेनर रनटाइम के साथ अलग-अलग सेटिंग्स के साथ अलग-अलग पॉड चलाने के लिए RuntimeClass का भी उपयोग कर सकते हैं।
