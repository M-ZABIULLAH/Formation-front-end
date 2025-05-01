# Objectifs journaliers

## Mercredi 30/04/2025

### Javascript :

### Première introduction au langage Javascript :

- [x] Comprendre la structure du code et la syntaxe en JavaScript :
  - [x] EcmaScript vs JavaScript
    - [x] l'importance de la ponctuation
    - [x] standard & environnement d'exécution
  - [x] ce qu'est une instruction
  - [x] ce qu'est l'insertion automatique (ou implicite) de point-virgule
  - [x] les commentaires
- [ x] Découvrir l'écosystème JavaScript :
  - [x] à quoi sert use-strict et comment l'utiliser (ES5, ES6+, etc ...)
  - [x] qu'est-ce que le TC39
  - [x] qu'est-ce que le ECMA-262
  - [x] quelle est la version actuelle du standard ECMAScript ?
- [x] Comprendre le fonctionnement des variables en JavaScript (https://fr.javascript.info/variables)
- [x] Découvrir les types de données en JavaScript (https://fr.javascript.info/types)
- [x] Comprendre `Les conversions de types` en JavaScript (https://fr.javascript.info/type-conversions)
- [x] Comprendre les mécanismes des opérateurs mathématiques en JavaScript (https://fr.javascript.info/operators) :
  - [x] concaténation
  - [x] précédence des opérateurs
  - [x] préfix & postfix


---


```markdown
# 🌐 Première introduction au langage JavaScript

---

## 🔹 1. Comprendre la structure du code et la syntaxe en JavaScript

### 🔸 EcmaScript vs JavaScript

- **JavaScript** est un langage de programmation interprété utilisé dans les navigateurs.
- **ECMAScript (ES)** est le **standard** qui définit la syntaxe et les fonctionnalités.
- JavaScript est une **implémentation** d’ECMAScript.

#### 📌 L'importance de la ponctuation
- Utilisation correcte de : `{}`, `()`, `[]`, `;`, `,`, `.`.
- Une mauvaise ponctuation = erreurs de syntaxe.

#### 📌 Standard & environnement d’exécution
- **Standard :** ECMA-262 (définit ECMAScript).
- **Environnements d’exécution :**
  - Navigateurs (Chrome, Firefox…)
  - Node.js (serveur)

### 🔸 Ce qu’est une instruction
- Une **instruction** = une action exécutée par le moteur JS.
```js
let nom = "Ali";
console.log(nom);
```

### 🔸 Insertion automatique de point-virgule
- JavaScript ajoute parfois `;` automatiquement → peut provoquer des erreurs :
```js
return 
  5; // retourne undefined
```

### 🔸 Les commentaires
```js
// Ceci est un commentaire

/*
   Ceci est un commentaire
   multi-ligne
*/
```

---

## 🔹 2. Découvrir l’écosystème JavaScript

### 🔸 À quoi sert `"use strict"` ?
- Active un **mode strict** (à partir de ES5)
- Empêche certaines erreurs :
```js
"use strict";
let x = 5;
```

### 🔸 Qu’est-ce que le TC39 ?
- Groupe de travail qui propose et valide les fonctionnalités ECMAScript.

### 🔸 Qu’est-ce que ECMA-262 ?
- Le document officiel qui **définit ECMAScript** (spécification du langage).

### 🔸 Quelle est la version actuelle d’ECMAScript ?
- En mai 2025 : **ECMAScript 2024** (publiée en juin 2024).

---

## 🔹 3. Comprendre le fonctionnement des variables

🔗 [Lire sur JavaScript.info](https://fr.javascript.info/variables)

- `let` → portée bloc, réaffectable.
- `const` → portée bloc, non modifiable.
- `var` → portée fonction (ancien, à éviter).

```js
let age = 30;
const pays = "France";
var nom = "Ali";
```

---

## 🔹 4. Découvrir les types de données

🔗 [Lire sur JavaScript.info](https://fr.javascript.info/types)

### Types primitifs :
- `number`, `string`, `boolean`, `null`, `undefined`, `symbol`, `bigint`

### Type objet :
```js
let utilisateur = {
  nom: "Zabi",
  age: 25
};
```

---

## 🔹 5. Conversions de types

🔗 [Lire sur JavaScript.info](https://fr.javascript.info/type-conversions)

### Conversion explicite :
```js
String(123)      // "123"
Number("42")     // 42
Boolean("")      // false
```

### Conversion implicite :
```js
"5" + 1          // "51" (concaténation)
"5" * "2"        // 10  (conversion en number)
```

---

## 🔹 6. Opérateurs mathématiques

🔗 [Lire sur JavaScript.info](https://fr.javascript.info/operators)

### 🔸 Concaténation :
```js
"Bonjour " + "Zabi"  // "Bonjour Zabi"
```

### 🔸 Précédence des opérateurs :
```js
let x = 1 + 2 * 3;  // Résultat : 7
```

### 🔸 Préfixe & Postfixe :
```js
let a = 1;
let b = ++a;  // b = 2
let c = a++;  // c = 2, a = 3
```

---
# 🌐 مقدمه‌ای بر زبان JavaScript

---

## 🔹 1. درک ساختار کد و نحو (Syntax) در JavaScript

### 🔸 EcmaScript در برابر JavaScript

- **JavaScript** یک زبان برنامه‌نویسی است که در مرورگرها استفاده می‌شود.
- **ECMAScript (ES)** استانداردی است که ساختار و ویژگی‌های JavaScript را تعریف می‌کند.
- JavaScript در واقع یک **پیاده‌سازی از ECMAScript** است.

#### 📌 اهمیت علائم نگارشی
- استفاده صحیح از `{}`, `()`, `[]`, `;`, `,`, `.` مهم است.
- اشتباه در استفاده از این علامت‌ها باعث خطا در کد می‌شود.

#### 📌 استاندارد و محیط اجرا
- **استاندارد:** ECMA-262 (که ECMAScript را تعریف می‌کند)
- **محیط‌های اجرا:**
  - مرورگرها (مثل Chrome، Firefox)
  - Node.js برای سمت سرور

### 🔸 دستور چیست؟
- هر **دستور** عملی است که موتور JS آن را اجرا می‌کند.
```js

let nom = "علی";
console.log(nom);
```

### 🔸 درج خودکار نقطه‌ویرگول (`;`)
- JavaScript در برخی موارد خودش `;` را اضافه می‌کند، اما ممکن است باعث خطا شود:
```js
return 
  5; // خروجی undefined می‌شود!
```

### 🔸 کامنت‌ها در JavaScript
```js
// این یک کامنت تک‌خطی است

/*
   این یک کامنت
   چندخطی است
*/
```

---

## 🔹 2. آشنایی با اکوسیستم JavaScript

### 🔸 use strict برای چیست؟
- حالت strict (سخت‌گیرانه) را فعال می‌کند (از نسخه ES5).
- از بروز برخی خطاها جلوگیری می‌کند.
```js
"use strict";
let x = 5;
```

### 🔸 TC39 چیست؟
- گروهی از برنامه‌نویسان که ویژگی‌های جدید JavaScript را طراحی و تأیید می‌کنند.

### 🔸 ECMA-262 چیست؟
- سند رسمی که تمام ویژگی‌ها و نحوه عملکرد زبان ECMAScript را تعریف می‌کند.

### 🔸 نسخه فعلی ECMAScript چیست؟
- تا مه ۲۰۲۵، نسخه **ECMAScript 2024** جدیدترین نسخه منتشرشده است (ژوئن ۲۰۲۴).

---

## 🔹 3. متغیرها در JavaScript

🔗 [لینک مرجع](https://fr.javascript.info/variables)

- `let` → قابل تغییر است، فقط در همان بلوک قابل استفاده است.
- `const` → مقدار ثابت دارد و فقط یک‌بار تعریف می‌شود.
- `var` → قدیمی و با محدوده تابع (function-scoped) است.

```js
let age = 30;
const pays = "France";
var nom = "Ali";
```

---

## 🔹 4. انواع داده در JavaScript

🔗 [لینک مرجع](https://fr.javascript.info/types)

### نوع‌های اولیه (Primitive):
- `number`, `string`, `boolean`, `null`, `undefined`, `symbol`, `bigint`

### نوع شیء (Object):
```js
let utilisateur = {
  nom: "Zabi",
  age: 25
};
```

---

## 🔹 5. تبدیل نوع (Type Conversions)

🔗 [لینک مرجع](https://fr.javascript.info/type-conversions)

### تبدیل صریح (Explicit):
```js
String(123)      // "123"
Number("42")     // 42
Boolean("")      // false
```

### تبدیل ضمنی (Implicit):
```js
"5" + 1          // "51" → رشته
"5" * "2"        // 10   → عدد
```

---

## 🔹 6. عملگرهای ریاضی در JavaScript

🔗 [لینک مرجع](https://fr.javascript.info/operators)

### 🔸 الحاق (Concaténation):
```js
"سلام " + "زبی"  // "سلام زبی"
```

### 🔸 تقدم عملگرها:
```js
let x = 1 + 2 * 3;  // نتیجه: 7
```

### 🔸 پیشوندی و پسوندی:
```js
let a = 1;
let b = ++a;  // b = 2
let c = a++;  // c = 2، a = 3
```

---

```
