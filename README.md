# Butor-Webshop
# SZTE TTIK Mobilalkfejl beadando

## Válaszott téma: 17 - Bútor webshop
Ha esetlegesen az apk nem lenne elérhető, akkor a download link itt megtalálható: 
https://mega.nz/file/vjBmAQJJ#YeOo2V8yGKHP9swrSDumWaIQrXOAIr2AqMABJAVbCjE

kis segítség a javításhoz

| Pontozási szempont | hintek |
| --- | --- |
| Fordítási hiba nincs | nincs |
| Futtatási hiba nincs | nincs |
| Firebase autentikáció meg van valósítva: | `RegisterActivity` és `MainActivity`, be lehet jelentkezni felhasználóval, névtelenül, illetve google fiókkal  |
| Adatmodell definiálása (class vagy interfész formájában) | `ShoppingItem` |
| Legalább 3 különböző activity használata  | 3 activity van, `RegisterActivity`, `MainActivity`, `ShopListActivity` |
| Beviteli mezők beviteli típusa megfelelő (jelszó kicsillagozva, email-nél megfelelő billentyűzet jelenik meg stb. | `res/layout` mappában vannak megvalósítva a szükséges beviteli mezők, pl.: `activity_main.xml`, `activity_shop_list.xml` |
| ConstraintLayout és még egy másik layout típus használata | ConstraintLayoutra például az `activity_main.xml`, RelativeLayoutra és LinearLayoutra példa a `activity_register.xml`,  |
| Reszponzív | Minden layout-hoz külön álló és fekvő, illetve tablet mód is található|
| Legalább 2 különböző animáció használata | A kosár ikonján megjelenő piros kör alakú számláló forog, ha növekszik a kosár tartalma`ShopListActivity updateAlertIcon()`, `res/anim rotate.xml`. Másik animáció, amiben becsúsznak oldalról a bútorbolt tartalmai az a `ShoppingItemAdapter onCreateViewHolder()`-ben található meg, `res/layout slide_in_row.xml`|
| Intentek használata: navigáció meg van valósítva az activityk között (minden activity elérhető) | `MainActivity`, `RegisterActivity`, illetve a `ShopListActivity`-ben egyárant megtalálhatóak |
| Lifecycle Hookok | például `MainActivity`-ben `onPause()`, `onLoadFinished()`|
| Notification, alarm manager használata | `NotificationHandler` `AlarmReceiver` `ShopListActivity` például: időközönként feldobált értesítések |
| CRUD műveletek | `RandomAsyncTask`, `RandomAsyncTaskLoader`, `ShopListActivity`-ben pl.: `deleteItem()`, `queryData()`, `updateAlertIcon()`, `initializeData()`  |
| 2 komplex firestore lekérdezés | ShopListActivity `queryData()` rendezés, limitálás |

Ha bármilyen kérdésed van discordon megtalálsz: DnL#0381
