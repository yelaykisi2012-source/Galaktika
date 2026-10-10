SPACEEDU + LGPSM 404
=====================

1. LOYIHA HAQIDA
----------------

SpaceEdu — kosmos va sayyoralar mavzusidagi zamonaviy, cinematic uslubdagi landing page.
Sayt foydalanuvchini to‘liq ekranli kosmik video fon, markaziy planetalar kontenti va
interaktiv sayyora tanlash mexanizmi orqali kosmos olamiga olib kiradi.

Loyiha ichiga LGPSM uslubidagi maxsus 404 error ekrani ham integratsiya qilingan.
Shuning uchun asosiy sayt va 404 sahifa alohida sayt emas — ular bitta self-contained
HTML fayl ichida ishlaydi.

Asosiy fayl: spaceedu.html

2. SAYTNING ASOSIY MAQSADI
---------------------------

- Kosmik ta’lim platformasi uchun kuchli vizual birinchi taassurot yaratish.
- Sayyoralar haqida kurs va darslarga qiziqish uyg‘otish.
- Foydalanuvchini GET STARTED yoki Enroll orqali ro‘yxatdan o‘tishga yo‘naltirish.
- Har bir sayyorani interaktiv tarzda tanlash imkonini berish.
- Noma’lum sahifalar uchun brendga mos, oddiy browser 404 o‘rniga maxsus error tajribasini ko‘rsatish.

3. ASOSIY EKRAN: SPACEEDU GALAKTIKA HERO
-----------------------------------------

Bosh sahifa to‘liq viewportni egallaydi va quyidagi elementlardan tashkil topgan:

- Full-screen kosmik video fon.
- Yuqori qismda spaceedu logotipi.
- Navigatsiya menyusi:
  - Planets
  - Tution
  - Tutorials
  - Blog
  - 404
  - Enroll
- Markaziy hero kontenti:
  - PLANET eyebrow sarlavhasi.
  - Katta serif shriftidagi sayyora nomi.
  - Cyan rangli dekorativ chiziq.
  - Sayyora haqida qisqa tavsif.
  - GET STARTED pill tugmasi.
- Ekranning chap va o‘ng tomonlarida qisman ko‘rinadigan sayyora cut-out rasmlari.
- Pastki qismda scroll boshqaruvi.

4. SAYYORALAR INTERAKSIYASI
----------------------------

Saytda uchta sayyora mavjud:

- EARTH — boshlang‘ich featured sayyora.
- VENUS — issiq, bulutli sayyora.
- MARS — qizil, cho‘l ko‘rinishidagi sayyora.

Ishlash tartibi:

- Sahifa ochilganda Earth markaziy fon sifatida ko‘rsatiladi.
- Venus chap tomonda, Mars o‘ng tomonda chiqadi.
- Chap yoki o‘ng sayyoraga bosilganda u featured sayyoraga aylanadi.
- Fon videosi, headline, tavsif, label va yon sayyoralar bir vaqtda yangilanadi.
- Oldingi featured sayyora yon slotlardan biriga qaytadi.
- Earth → Venus → Mars → Earth aylanishi to‘liq reversiv ishlaydi.
- Har bir sayyora o‘zining video klipi, still rasmi va cut-out PNG assetiga ega.

5. NAVIGATSIYA VA TUGMALAR
--------------------------

Planets:
- Asosiy SpaceEdu hero ekraniga qaytaradi.
- 404 ekrani ochiq bo‘lsa, uni yopadi.

Tution:
- Tution haqida qisqa ma’lumot dialog oynasini ochadi.

Tutorials:
- Planetalar, orbitalar, atmosferalar va kosmik darslar haqida ma’lumot dialogini ochadi.

Blog:
- SpaceEdu jurnalida missiyalar, kashfiyotlar va astronomiya maqolalari bo‘lishi haqida ma’lumot beradi.

404:
- Maxsus LGPSM 404 ekranini ochadi.
- 404 raqami kirish animatsiyasi bilan paydo bo‘ladi.
- Logotip, chiziq va xabar ketma-ketlikda ko‘rinadi.

Enroll:
- Enrollment haqida qisqa ma’lumot dialog oynasini ochadi.

GET STARTED:
- Enroll bilan bir xil enrollment dialogini ochadi.

Scroll:
- Keyingi kontent bo‘lmagani uchun foydalanuvchini Tutorials dialogiga olib boradi.
- Shu bilan tugma ishlamaydigan dekorativ element bo‘lib qolmaydi.

Burger menyu:
- Tablet va mobil ekranlarda navigatsiyani ochadi/yopadi.
- Escape tugmasi bilan yopiladi.
- Menyu tashqarisiga bosilganda ham yopiladi.

6. MAXSUS 404 EKRANI
--------------------

404 ekrani SpaceEdu bilan bitta HTML faylga joylashtirilgan.

404 ekrani quyidagilardan iborat:

- Full-screen video background.
- Yuqorida LGPSM geometrik SVG logotipi.
- Markazda katta gradientli “404” raqami.
- “The path may be broken, but the journey isn’t. Let’s get you back.” xabari.
- BACK TO SPACEEDU tugmasi.

Animatsiya:

- Logo yumshoq fade-in bilan ko‘rinadi.
- 404 raqami scale va vertical rise animatsiyasi bilan paydo bo‘ladi.
- Divider markazdan ikki tomonga chiziladi.
- Xabar pastdan yumshoq rise animatsiyasi bilan chiqadi.
- prefers-reduced-motion yoqilgan foydalanuvchilar uchun animatsiyalar o‘chiriladi.

404 ochish usullari:

1) Navigatsiyadagi 404 tugmasini bosish.
2) Noma’lum URL’ga kirish, masalan:
   - /404
   - /missing-page
   - /test
   - /abc

404 dan qaytish:

- BACK TO SPACEEDU tugmasini bosish.
- Navigatsiyadagi Planets yoki logo tugmasini bosish.
- Browser history orqali qaytish.

7. DIZAYN VA VIZUAL TIZIM
-------------------------

Vizual yo‘nalish:

- Cinematic space education.
- Premium editorial composition.
- Qorong‘i kosmik fon va yorqin oq tipografiya.
- Cyan accent ranglar.
- Serif headline va body uchun geometrik sans/mono shriftlar.

Asosiy ranglar:

- Dark navy: #04101f
- Black fallback: #000000
- White: #ffffff
- Cyan accent: #79dce8
- Logo cyan: #5fd0e1
- Button ink: #071227

Tipografiya:

- SpaceEdu headline va planet labels: Prata.
- SpaceEdu body va navigation: Hanken Grotesk.
- SpaceEdu logo: Poppins.
- LGPSM 404 raqami va xabari: Geist Mono:SemiBold.

Kompozitsiya:

- Desktop layout 1353 × 1163 reference composition asosida qurilgan.
- Barcha asosiy o‘lchamlar responsive custom property --u orqali hisoblanadi.
- Markaziy kontent optik markazga joylashtirilgan.
- Yon planetalar ekran chetlaridan cropped ko‘rinishda ishlatiladi.

8. RESPONSIVE MOSLASHUV
-----------------------

Desktop:
- To‘liq desktop navigatsiya.
- Katta markaziy headline.
- Chap va o‘ng sayyoralar keng kompozitsiyada.

Tablet:
- Burger menyu yoqiladi.
- Hero composition markazda saqlanadi.
- Sayyoralar va CTA bir qatorda qoladi.

Mobil:
- Burger menyu ishlaydi.
- Kontent flex column tartibida joylashadi.
- Headline va paragraph ekran kengligiga moslashadi.
- Planet cut-outlar kichrayadi.
- Narrow phone ekranlarida label’lar tugma ostiga tushadi.
- Gorizontal scroll yo‘q.

404 mobile:
- Logo yuqoridan 32 design pixel masofada.
- Logo 75 foizga kichrayadi.
- 404 raqami clamp() yordamida responsive bo‘ladi.
- Divider mobil content width’ni to‘liq egallaydi.
- Xabar shrift o‘lchami mobil kenglikka moslashadi.

9. TEXNIK IMPLEMENTATSIYA
-------------------------

- Bitta self-contained spaceedu.html fayl.
- Framework talab qilmaydi.
- CSS bitta <style> block ichida.
- JavaScript <script> blocklar ichida.
- Tashqi JavaScript kutubxonalari ishlatilmagan.
- Video va image assetlar exact CDN URL’lar orqali yuklanadi.
- Sayyora videolari lazy warm/preload mexanizmi bilan yuklanadi.
- Venus va Mars video fayllari faqat kerak bo‘lganda birinchi marta source oladi.
- Planet switching vaqtida img.src qayta yozilmaydi, shu sababli oldingi rasm flash qilmaydi.
- Video autoplay uchun muted va playsinline ishlatiladi.
- Favicon Earth cut-out assetidan foydalanadi.

10. ACCESSIBILITY
-----------------

- Planetalar real button elementlari.
- Planet button’lar dynamic aria-label bilan ishlaydi.
- Videolar aria-hidden="true".
- Dekorativ cut-out rasmlar alt="" bilan belgilangan.
- SVG logotiplar aria-hidden="true".
- LGPSM brand wrapper aria-label="LGPSM".
- Keyboard navigation va focus-visible outline mavjud.
- Burger menyu aria-expanded holatini yangilaydi.
- Escape tugmasi menyuni va dialogni yopishga yordam beradi.
- prefers-reduced-motion qo‘llab-quvvatlanadi.

11. ASSETLAR
-----------

SpaceEdu background videolari:

EARTH:
https://d8j0ntlcm91z4.cloudfront.net/user_38xzZboKViGWJOttwIXH07lWA1P/hf_20260827_202422_3ffb4889-c520-432d-8458-038009eb40df.mp4

VENUS:
https://d8j0ntlcm91z4.cloudfront.net/user_38xzZboKViGWJOttwIXH07lWA1P/hf_20260827_202422_b211cd74-013b-4dd3-bfd0-64491d8696fa.mp4

MARS:
https://d8j0ntlcm91z4.cloudfront.net/user_38xzZboKViGWJOttwIXH07lWA1P/hf_20260827_202422_51eae59a-2459-4c84-907c-cc5edfe5fea7.mp4

LGPSM 404 background video:
https://d8j0ntlcm91z4.cloudfront.net/user_38xzZboKViGWJOttwIXH07lWA1P/hf_20260801_001207_ec20d138-aa45-4b2b-ab8c-bdc71607f240.mp4

Fonts:

- Google Fonts: Prata, Hanken Grotesk, Poppins.
- Figma Geist Mono font:
  https://static.figma.com/font/GeistMono_wght__1

12. ISHGA TUSHIRISH
--------------------

Variant A — oddiy lokal ko‘rish:

1. ZIP faylni oching.
2. spaceedu.html faylini browser’da oching.
3. Internet yoqilgan bo‘lishi kerak, chunki video, rasmlar va fontlar CDN’dan olinadi.

Variant B — local server:

Python:

  python3 -m http.server 8000

Keyin browser’da:

  http://localhost:8000/spaceedu.html

Variant C — hosting:

- spaceedu.html faylini hostingga joylashtiring.
- Hosting unknown routes uchun shu HTML faylni qaytarishi kerak.
- Masalan /404 yoki /missing-page URL’lari ham spaceedu.html ga fallback qilishi kerak.
- Shunda client-side JavaScript noma’lum route’ni aniqlab LGPSM 404 ekranini chiqaradi.

13. DEMO UCHUN TAVSIYA ETILADIGAN KETMA-KETLIK
-----------------------------------------------

1. Bosh sahifani ochib, kosmik video fonni ko‘rsating.
2. Earth featured holatida ekanini ko‘rsating.
3. Venus planetasini bosing va headline/fon/label qanday almashishini ko‘rsating.
4. Mars’ni bosing va aylanish reversiv ishlashini ko‘rsating.
5. Burger menyuni mobil preview’da oching.
6. Tutorials yoki Tution tugmasini bosib dialog oynasini ko‘rsating.
7. Enroll yoki GET STARTED orqali enrollment dialogini oching.
8. Nav menyusidagi 404 tugmasini bosing.
9. 404 animation: logo, 404 raqami, divider va xabar ketma-ketligini ko‘rsating.
10. BACK TO SPACEEDU tugmasi bilan asosiy hero’ga qayting.
11. Oxirida /missing-page kabi noma’lum URL orqali automatic 404 fallback’ni ko‘rsating.

14. LOYIHA XULOSASI
-------------------

SpaceEdu + LGPSM 404 — kosmik ta’lim brendi uchun yaratilgan, vizual jihatdan kuchli,
responsive va interaktiv single-page tajriba.

Saytning asosiy farqi:

- Cinematic video background.
- Real-time planet switching.
- Responsive desktop/tablet/mobile composition.
- Ishlaydigan navigatsiya va CTA elementlari.
- Brendga mos maxsus 404 error animation.
- Barcha asosiy funksiyalar bitta self-contained HTML faylda.
