---
title: Islo privacy policy
---

# Islo privacy policy

*Last updated: 2 November 2026*

Islo is a Dynamic Island for Windows. It runs on your PC, has no account, and
has no servers of its own. It collects nothing about you and sends nothing to
its developer: no analytics, no tracking, no ads.

## What stays on your PC

Everything Islo shows comes from your own PC and stays there:

- **Notifications** from your apps are read from Windows' notification list
  to show them on the island. They are never saved or sent anywhere. In the
  Microsoft Store version, Windows asks you first, and Islo reads them only
  while you allow it; you can turn it off in Windows' Settings (Privacy,
  Notifications).
- **What you copy** (the clipboard) is shown on the island and kept in memory
  for the Clipboard page. It's never saved to disk (except a copied
  screenshot you drag, see below) or sent anywhere, and it's gone when Islo
  closes. What password managers copy (they mark it so) is skipped: it never
  shows and isn't kept.
- **Notes, the shelf and your settings** are saved in `%LOCALAPPDATA%\Islo`
  on your PC, with your approximate place for the weather (so it isn't looked
  up again each time).
- **Music**: what's playing comes from Windows' media controls. Lyrics found
  for a song are saved in `%LOCALAPPDATA%\Islo\lyrics` (with the song's title
  and artist), so a song heard before shows them at once; at most 10 MB, the
  songs not heard for longest go first.
- **Camera, microphone, battery, devices and downloads**: Islo only notices
  that they changed (for example, "the microphone is in use", or a download's
  file name and progress). It never records sound or video.
- **Screenshots**: when you take one, Islo opens that new picture to show it
  small on the island, ready to drag. A screenshot that is only on the
  clipboard (no file) gets a file in `%LOCALAPPDATA%\Islo\Screenshots` when
  you drag it or put it on the shelf; the newest 20 are kept. Islo doesn't
  open your other files, and never uploads or sends any file.
- **The keyboard**: Islo is never told which keys you press. For its Caps
  Lock and keyboard-language cards it asks Windows a few times a second
  whether Caps Lock or Num Lock is on and which language the window in front
  types in. It can't see or record what you type.
- **The window in front, during a focus session only**: to warn you about
  distracting apps and sites you chose, Islo looks at the name of the app in
  front and its window title (a browser's shows the page's title). It's
  compared with your list there and then, never saved or sent.
- **A log** (`islo.log`) in the same folder helps fix problems. It never
  contains notification text, what you copied, or your notes.
- **If Islo crashes**, it saves `islo-crash.dmp` in the same folder, to find
  out why. It can hold bits of what Islo had in memory at that moment. It
  stays on your PC and is never sent anywhere; it reaches the developer only
  if you send it yourself.

## What goes over the internet

Islo talks to these services, and only for the features below. Each is
sent only what it needs:

| Service | What for | What it receives |
|---|---|---|
| [ipwho.is](https://ipwho.is), or [ipapi.co](https://ipapi.co) if it doesn't answer | Your approximate city, for weather and prayer times | Your internet address (every website sees it). Not used when you type a city in Settings. |
| [Open-Meteo](https://open-meteo.com) | Weather, and finding a city you type | Approximate coordinates of your city, or the city name you typed |
| [LRCLIB](https://lrclib.net) | Synced lyrics for the song playing | The song's title, artist and length. You can turn lyrics off in Settings → Music. |
| Microsoft (`msftconnecttest.com`) | Opened only if you click "Sign in" on a card that says the network needs a sign-in page (e.g. hotel Wi-Fi) | What any browser sends when opening a page |
| Google or Microsoft, only if you add your calendar | Your calendar's events, for the island | Only the request for your calendar's own address |

**Your calendar** (only if you add it in Settings → Calendar): Islo reads it from the
calendar's secret iCal address, which you copy from Google Calendar or Outlook. The
address is saved only in `settings.ini` on your PC and never written to the log. Every
15 minutes Islo downloads it directly from Google or Microsoft over https, from that
address and nowhere else. Today's and tomorrow's events are kept in
`calendar-events.tsv` in the same folder for the island to show; nothing about your
calendar is sent anywhere.

Prayer times are worked out on your PC. Islo doesn't send your notifications,
your clipboard, your notes, or anything else.

## Children

Islo collects no personal information from anyone, including children.

## Changes

If this policy changes, the new version will be published here with a new date.

## Contact

Questions: wessamelden7@gmail.com

---

<div dir="rtl" markdown="1">

# سياسة الخصوصية لـ Islo

*آخر تحديث: 2 نوفمبر 2026*

Islo جزيرة ديناميكية لويندوز. بيشتغل على جهازك، ومن غير حساب، ومالوش سيرفرات.
مش بيجمع أي بيانات عنك ومش بيبعت حاجة لمطوّره: لا إحصائيات ولا تتبع ولا إعلانات.

## اللي بيفضل على جهازك

- **الإشعارات** بتتقري من قايمة إشعارات ويندوز عشان تظهر على الجزيرة. مش بتتحفظ ومش بتتبعت لأي مكان. في نسخة Microsoft Store، الويندوز بيستأذنك الأول، وIslo مبيقراهاش غير وانت سامح بده، وتقدر تقفله من إعدادات الويندوز (الخصوصية، الإشعارات).
- **اللي بتنسخه** بيظهر على الجزيرة ويفضل في الذاكرة لصفحة الحافظة. مش بيتحفظ على الجهاز (إلا لقطة شاشة منسوخة بتسحبها، تحت) ومش بيتبعت، وبيروح لما Islo يتقفل. واللي برامج الباسوردات بتنسخه (بتعلّم عليه) Islo بيتجاهله: مش بيظهر ومش بيتحفظ.
- **الملاحظات والرف والإعدادات** متخزنين في `%LOCALAPPDATA%\Islo` على جهازك، ومعاهم مكانك التقريبي للطقس (عشان ميتدورش عليه كل مرة).
- **الموسيقى**: اللي شغال بيتعرف من أزرار الميديا في ويندوز. كلمات الأغاني اللي بتتلاقي بتتحفظ في `%LOCALAPPDATA%\Islo\lyrics` (مع اسم الأغنية والفنان)، عشان الأغنية اللي سمعتها قبل كده تظهر كلماتها على طول. أقصى حاجة 10 ميجا، والأغاني اللي بقالك أكتر وقت مسمعتهاش بتتمسح الأول.
- **الكاميرا والميكروفون والبطارية والأجهزة والتحميلات**: Islo بيلاحظ إنها اتغيرت بس (زي «الميكروفون شغال»، أو اسم الملف اللي بيتحمّل ووصل لفين). مش بيسجّل صوت أو صورة.
- **لقطات الشاشة**: لما تاخد لقطة، Islo بيفتح الصورة الجديدة دي بس عشان يعرضها صغيرة على الجزيرة وتقدر تسحبها. ولو اللقطة متنسخة بس من غير ملف، Islo بيعملها ملف في `%LOCALAPPDATA%\Islo\Screenshots` لما تسحبها أو تحطها على الرف، وبيحتفظ بآخر 20 بس. مش بيفتح ملفاتك التانية، ومش بيرفع أو يبعت أي ملف.
- **الكيبورد**: Islo مبيتبلّغش أبداً بالزراير اللي بتدوسها. عشان كروت Caps Lock ولغة الكيبورد، بيسأل الويندوز كام مرة في الثانية: Caps Lock أو Num Lock شغالين؟ والنافذة اللي قدامك بتكتب بأنهي لغة؟ مش بيقدر يشوف أو يسجّل اللي بتكتبه.
- **النافذة اللي قدامك، وقت جلسة التركيز بس**: عشان يحذّرك من البرامج والمواقع المشتتة اللي اخترتها، Islo بيشوف اسم البرنامج اللي قدامك وعنوان نافذته (المتصفح بيكتب فيه عنوان الصفحة). بيتقارن بقايمتك في نفس اللحظة، ومش بيتحفظ ولا بيتبعت.
- **سجل** (`islo.log`) في نفس الفولدر بيساعد في حل المشاكل. مفيهوش أبداً نص الإشعارات ولا اللي نسخته ولا ملاحظاتك.
- **لو Islo وقع**، بيحفظ `islo-crash.dmp` في نفس الفولدر عشان نعرف السبب. ممكن يكون فيه حتت من اللي كان في ذاكرة Islo ساعتها. بيفضل على جهازك ومش بيتبعت لأي مكان، ومبيوصلش للمطوّر غير لو انت بعته بنفسك.

## اللي بيروح على الإنترنت

| الخدمة | ليه | بتستقبل إيه |
|---|---|---|
| ipwho.is، أو ipapi.co لو مردّتش | مدينتك التقريبية للطقس ومواقيت الصلاة | عنوان الإنترنت بتاعك (أي موقع بيشوفه). مش بتُستخدم لو كتبت مدينتك في الإعدادات. |
| Open-Meteo | الطقس، ولقي المدينة اللي كتبتها | إحداثيات تقريبية لمدينتك، أو اسم المدينة اللي كتبته |
| LRCLIB | كلمات الأغنية اللي شغالة | اسم الأغنية والفنان والمدة. تقدر تقفل الكلمات من الإعدادات ← الموسيقى. |
| مايكروسوفت (`msftconnecttest.com`) | بيتفتح بس لو دست «تسجيل الدخول» على كارت بيقول إن الشبكة محتاجة صفحة دخول (زي واي فاي الفنادق) | اللي أي متصفح بيبعته وهو بيفتح صفحة |
| Google أو مايكروسوفت، لو ضفت التقويم بتاعك بس | مواعيد التقويم بتاعك عشان تظهر على الجزيرة | طلب عنوان التقويم بتاعك وبس |

**التقويم بتاعك** (لو ضفته من الإعدادات ← التقويم بس): Islo بيقراه من العنوان السري للتقويم بصيغة iCal اللي بتنسخه من Google Calendar أو Outlook. العنوان بيتحفظ في `settings.ini` على جهازك بس، ومش بيتكتب في السجل أبداً. كل 15 دقيقة Islo بيجيب التقويم من Google أو مايكروسوفت على طول بـ https، من العنوان ده ومن مكان غيره لأ. مواعيد النهارده وبكره بتتحفظ في `calendar-events.tsv` في نفس الفولدر عشان الجزيرة تعرضها، ولا حاجة من التقويم بتتبعت لأي مكان.

مواقيت الصلاة بتتحسب على جهازك. Islo مش بيبعت إشعاراتك ولا الحافظة ولا ملاحظاتك ولا أي حاجة تانية.

## الأطفال

Islo مش بيجمع أي بيانات شخصية من أي حد، ومن ضمنهم الأطفال.

## التغييرات

لو السياسة دي اتغيرت، النسخة الجديدة هتتنشر هنا بتاريخ جديد.

## التواصل

wessamelden7@gmail.com

</div>
