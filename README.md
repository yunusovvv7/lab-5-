lab-5
1. inline
Inline funksiya chaqirilgan joyiga kodini o‘zi borib joylashib oladi. Shuning uchun har safar yangi obyekt ochib o‘tirmaydi, bu esa dastur ishlashini biroz tezlashtiradi.
2. return break continue
 ⁠return⁠ funksiyaning o‘zini to‘xtatib chiqarib yuboradi
 ⁠break⁠ — siklni (tsiklni) butunlay to‘xtatadi
 ⁠continue⁠ — siklning shu aylanmasini tashlab yuborib, keyingisiga o‘tib ketadi
3. noinline
Agar inline funksiyaga bir nechta lambda bersak-u bittasini o‘sha yerga yoyib yubormasdan, oddiy obyekt (o‘zgaruvchi) holatida saqlamoqchi bo‘lsak, ⁠noinline⁠ ishlatamiz
4. crossinline
Lambda ichidan turib tashqi funksiyani ⁠return⁠ qilib yuborishni (to‘xtatib qo‘yishni) taqiqlash uchun kerak dastur chalkashib ketmasligi uchun yordam beradi
5. reifiedbb
Kotlin'da generic tur vaqt o‘tib (kompilyatsiyadan keyin) yo‘qolib qoladi (⁠type erasure⁠) reified⁠ esa uni saqlab qolishga va funksiya ichida turi bo‘yicha tekshirishga imkon beradi Faqat ⁠inline⁠ bilan ishlaydi chunki kod aynan o‘sha joyga ko‘chib o‘tgandagina turning nima ekanligi bilinadi
6. inline property
Xuddi funksiyaga o‘xshab. property'ning getter yoki setter'ini chaqirilgan joyiga to‘g‘ridan-to‘g‘ri yozib yuboradi Ichida ⁠field⁠ (backing field) ishlatib bo‘lmaydi Masalan dp⁠ ni ⁠px⁠ ga o‘tkazadigan oddiy narsalar uchun zo‘r lekin katta kodlar uchun xotirani to‘ldirib yuboradi 
7. Public inline
Katta loyihalarda boshqa modullar buni o‘qiy oladi lekin o‘zining ⁠internal⁠ narsalariga tegolmaydi chunki kod boshqa modulga o‘tib ketadi ⁠@PublishedApi⁠ ana shu ⁠internal⁠ narsani inline funksiya ko‘rib ishlatishi uchun ruxsat berib qo‘yadi
8. typealias
Uzun yozilgan turlarga shunchaki qisqaroq  (name) qo‘yib qo‘yish Yangi tur yaratmaydi Masalan uzun generic nomlarni qisqartirish uchun qulay lekin oddiy so‘zlarga (⁠String⁠ ga o‘xshash) qo‘ysangiz adashib o‘rnini almashtirib yuborsangiz ham kompilyator sezmay qolishi mumkin
9. Any
Kotlin'dagi hamma narsaning otasi — eng asosiy tur Har bir klassga ⁠equals⁠ hashCode⁠ larni beradi Lekin ⁠Any qilib ishlatish xavfli chunki keyin uni to‘g‘ri turga cast qilish (⁠as⁠) kerak bo‘ladi aks holda xato berib yiqilib tushishi mumkin.
10. Nothing
Umuman qiymat qaytarmaydigan narsa (masalan doim xato otib to‘xtaydigan funksiyalar) U hamma turning quyi turi bo‘la oladi Masalan biron xato chiqib to‘xtagandan keyin kompilyator bu yerga boshqa kod kelmasligini tushunib o‘zi "smart-cast" qilib ketadi Yoki UI'dagi ⁠Loading⁠/⁠Error⁠ holatlarida ma'lumot ketkazish shart bo‘lmaganda ishlatiladi.) 
