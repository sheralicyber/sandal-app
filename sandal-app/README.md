# Ишлаб чиқариш маркази — Android илова

https://sandal.aideveloper.uz/ сайтини телефонда илова сифатида очади (WebView).
Роллар сайтнинг ўзида логиндан кейин белгиланади, ҳар ким фақат ўз ролидаги бўлимларни кўради.

## APK қилиб олиш

1. Android Studio (Koala ёки янгироқ) ни очинг.
2. **File → Open** орқали `sandal-app` папкасини танланг, Gradle синхронлашини кутинг.
3. Синовдан ўтказиш: телефонни USB билан улаб **Run ▶** босинг.
4. Тарқатиш учун APK: **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
   Play Market учун: **Build → Generate Signed Bundle / APK** (ўз калитингиз билан).

## Созламалар

- Сайт манзили: `app/build.gradle` ичидаги `SITE_URL`.
- Иловa номи: `app/src/main/res/values/strings.xml` (`app_name`).
- Рангларни ўзгартириш: `res/values/colors.xml` (`brand`).
- Иконка: `res/drawable/ic_launcher_foreground.xml` ва `ic_launcher_background.xml`.
  Ўз логотипингизни Android Studio'да **New → Image Asset** орқали қўйсангиз бўлади.

## Нималар бор

- Логин сессияси сақланади (қайта-қайта киритиш шарт эмас)
- Тортиб янгилаш, юкланиш чизиғи
- Орқага тугмаси сайт ичида орқага қайтаради
- Интернет йўқ бўлса, "Қайта уриниш" экрани
- Файл/расм юклаш (input type=file) ишлайди
- Ташқи ҳаволалар (тел, Telegram ва ҳ.к.) тегишли иловада очилади
