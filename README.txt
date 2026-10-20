LIVE TV CHANNELS APP — files aur tareeqa
================================

YEH FILES HAIN:
- index.html    → poori app (design + channels wala system)
- manifest.json → mobile install ki maloomat (naam, icon)
- sw.js         → app ko tez aur offline-ready rakhne wali file
- icon-192.png / icon-512.png → app ka icon

APP KAISE BANTI HAI (asaan lafzon mein):
1. App asal mein ek website hoti hai — index.html mein sab kuch hota hai.
2. Channels kisi server par rakhe nahi hote. App internet se free channels
   ki list (iptv-org ka public data) leti hai aur channel tap karne par
   usi broadcaster ki free stream chala deti hai jo wo khud internet par
   sab ke liye deta hai.
3. In files ko internet par lagana "hosting" kehlata hai. Yeh app
   Cloudflare par lagi hai — files upload karne se ek link ban jata hai.
4. Mobile par woh link Chrome mein kholo → menu (3 dots) → "Install app"
   ya "Add to Home screen" — app mobile mein install ho jati hai,
   home screen par icon aa jata hai.

SETTINGS WALI BAAT:
- 18+ category default BAND hai. Settings mein "Allow 18+ Channels"
  ON karne se hi nazar aati hai.
- Sach: bare free sources (iptv-org waghera) ne 18+ channels ki free
  streams taqreeban khatam kar di hain, is liye 18+ list abhi aksar
  khaali mile gi. Jab koi working free stream dobara ayegi, channel
  khud list mein aa jaye ga.

WORKING STREAMS WALA SYSTEM:
- App ki lists ab raw nahi hain. Har stream ko pehle test kiya jata hai —
  sirf wohi channel list mein aata hai jo asal mein chalta hai aur mobile
  browser mein play ho sakta hai.
- Har channel ke sath 2-4 backup streams bhi hoti hain: pehli band mile
  to player khud dusri, phir teesri try karta hai.
- Player mein quality button hai: "Kam MB" (default) data kam khata hai,
  "High" best quality deta hai.

SPORTS MATCHES:
- Sports kholne par upar "Aaj ke Matches" aate hain (football, cricket,
  basketball, tennis waghera — jo free data mein available hon).
- Match par tap karne se us sport ke channels khul jate hain.

SHARE:
- Upar 📤 button se app ka link kisi ko bhi bhej sakte ho — link kholne
  wala app install kar sakta hai.

ADS / MONEY (MONETIZATION):
- App mein ads ki jagah tayyar hai, lekin ads chalane ke liye ad network
  par account TUMHE banana hoga (paisay tumhare naam/account mein aate
  hain, is liye sign-up tumhara hona chahiye).
- Asaan tareeqa: Monetag (monetag.com) ya Adsterra (adsterra.com) par
  free account banao → website add karo: 
  arslanmuhammad6670-alt.github.io/live-tv-channels
  → wahan se ek chhota sa ad code mile ga → wo code mujhe bhej dena,
  mein app mein laga dunga, ads chal parein ge.

NAYE FEATURES:
- Home par "Install App" button (ek tap se install).
- Player mein "Pichla / Agla" button — back kiye baghair channel badlo.
- Home par "Recently Watched" — jo channel dekha, wo dobara wahin milta hai.

FAVORITES:
- Kisi channel ke sath ☆ dabane se wo ⭐ Favorites mein save ho jata hai
  (mobile ke andar hi save hota hai).
