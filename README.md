# Qara Bazar — GitHub Pages Qurulum Təlimatı

## Fayllar
- `index.html` — Camahat üçün bazar səhifəsi
- `admin.html` — Şifrəli admin panel

---

## GitHub Pages-ə Necə Yükləmək

### 1. GitHub hesabı aç
→ https://github.com/signup (pulsuz)

### 2. Yeni repo yarat
- GitHub-da "New repository" düyməsinə bas
- Ad: `qara-bazar` (və ya istədiyin ad)
- Public seç
- "Create repository" düyməsinə bas

### 3. Faylları yüklə
- Repo səhifəsində "Add file" → "Upload files"
- `index.html` və `admin.html` fayllarını sürükle-burax
- "Commit changes" düyməsinə bas

### 4. GitHub Pages aktiv et
- Repo → Settings → Pages (sol menyu)
- Source: "Deploy from a branch"
- Branch: `main` / `root`
- Save düyməsinə bas
- 2-3 dəqiqə gözlə

### 5. Linkin hazırdır!
`https://SƏNIN_ADИН.github.io/qara-bazar/`

---

## Admin Panel İstifadəsi

**URL:** `https://SƏNIN_ADИН.github.io/qara-bazar/admin.html`

**Giriş məlumatları (ilk dəfə):**
- İstifadəçi adı: `admin`
- Şifrə: `qara2026`

> ⚠️ Şifrəni dəyişmək üçün `admin.html` faylını aç,
> `ADMIN_USER` və `ADMIN_PASS` dəyişənlərini tap və yenilə.

---

## 2 Gündən Bir Yeniləmə

1. `admin.html`-ə gir, şifrənlə daxil ol
2. Malların qiymətlərini cədvəldə dəyişdir (birbaşa yazmaq olar)
3. Yeni mal əlavə et və ya köhnəni sil
4. **"Yadda saxla & Yayımla"** düyməsinə bas
5. Tarix avtomatik yenilənir, camahat görür ✓

---

## Şifrəni Dəyişmək

`admin.html` faylını aç, bu sətirlərini tap:
```js
const ADMIN_USER='admin';
const ADMIN_PASS='qara2026';
```
İstədiyin ad və şifrəylə əvəz et, sonra GitHub-a yenidən yüklə.

---

## Məlumatlar Harada Saxlanır?

Məlumatlar brauzerin `localStorage`-ında saxlanır.
Yəni: sən admin-dən dəyişirsən → camahat öz brauzerindən yeniləmə görür.

> GitHub Pages-də backend yoxdur, buna görə bu ən sadə həlldir.
> Əgər gələcəkdə bütün istifadəçilər EYNI məlumatı görsün istəyirsənsə,
> Firebase (pulsuz) inteqrasiyası əlavə etmək olar.
