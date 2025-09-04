# HTML va CSS to'liq darslik

## 1-BO'LIM: HTML ASOSLARI
### 1.2 HTML hujjat strukturasi
### 1.3 Asosiy HTML taglar

### 1.1 HTML nima?
HTML (HyperText Markup Language) - veb sahifalarini yaratish uchun ishlatiladigan markup tili. HTML elementlar yordamida matnni strukturalashtiradi.

### 1.2 HTML hujjat strukturasi
```html
<!DOCTYPE html>
<html lang="uz-UZ" dir="ltr">
<head>
    <!-- Character Encoding (har doim birinchi bo'lishi kerak) -->
    <meta charset="UTF-8">
    
    <!-- Viewport (responsive dizayn uchun) -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no">
    
    <!-- HTTP-Equiv Meta -->
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="refresh" content="30">
    
    <!-- SEO Meta Tags -->
    <title>Sahifa sarlavhasi - Brand nomi</title>
    <meta name="description" content="Sahifa tavsifi 150-160 belgi ichida">
    <meta name="keywords" content="kalit, so'zlar, vergul, bilan">
    <meta name="author" content="Muallif ismi">
    <meta name="robots" content="index, follow">
    <meta name="googlebot" content="index, follow">
    
    <!-- Open Graph (Facebook) -->
    <meta property="og:type" content="website">
    <meta property="og:title" content="Sahifa sarlavhasi">
    <meta property="og:description" content="Sahifa tavsifi">
    <meta property="og:image" content="https://example.com/image.jpg">
    <meta property="og:url" content="https://example.com/page">
    <meta property="og:site_name" content="Sayt nomi">
    
    <!-- Twitter Card -->
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:title" content="Sahifa sarlavhasi">
    <meta name="twitter:description" content="Sahifa tavsifi">
    <meta name="twitter:image" content="https://example.com/image.jpg">
    
    <!-- Icons -->
    <link rel="icon" type="image/x-icon" href="/favicon.ico">
    <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
    <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
    <link rel="manifest" href="/site.webmanifest">
    
    <!-- External Resources -->
    <link rel="stylesheet" href="styles.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
    
    <!-- Performance hints -->
    <link rel="preload" href="hero-image.jpg" as="image">
    <link rel="prefetch" href="next-page.html">
    <link rel="dns-prefetch" href="//example.com">
</head>
<body>
    <!-- Sahifa tarkibi -->
    
    <!-- Scripts (sahifa oxirida) -->
    <script src="script.js" defer></script>
</body>
</html>
```

**Tushuntirish:**
- `<!DOCTYPE html>` - HTML5 hujjat ekanligini bildiradi
- `<html>` - barcha HTML kodlarni o'rab oladi
- `<head>` - sahifa haqida ma'lumotlar (ko'rinmaydigan)
- `<body>` - sahifaning asosiy tarkibi (ko'rinadigan)

### 1.3 Asosiy HTML taglar
#### Sarlavhalar (Headings)
```html
<h1>Eng katta sarlavha</h1>
<h2>Ikkinchi darajali sarlavha</h2>
<h3>Uchinchi darajali sarlavha</h3>
<h4>To'rtinchi darajali sarlavha</h4>
<h5>Beshinchi darajali sarlavha</h5>
<h6>Olti darajali sarlavha</h6>
```

#### Matnlar
```html
<p>Bu paragraf. Matnning asosiy qismi shu yerda yoziladi.</p>
<span>Bu inline element - qatorning ichida ishlatiladi.</span>
<div>Bu block element - alohida qator egallaydi.</div>

<!-- Matn formatlashtirish -->
<strong>Qalin matn</strong>
<b>Qalin matn (style uchun)</b>
<em>Kursiv matn (ta'kidlash uchun)</em>
<i>Kursiv matn (style uchun)</i>
<u>Chizilgan matn</u>
<s>O'chirilgan matn</s>
<mark>Belgilangan matn</mark>
<small>Kichik matn</small>
```

#### Ro'yxatlar
```html
<!-- Tartibsiz ro'yxat -->
<ul>
    <li>Birinchi element</li>
    <li>Ikkinchi element</li>
    <li>Uchinchi element</li>
</ul>

<!-- Tartiblangan ro'yxat -->
<ol>
    <li>Birinchi qadam</li>
    <li>Ikkinchi qadam</li>
    <li>Uchinchi qadam</li>
</ol>

<!-- Ta'rif ro'yxati -->
<dl>
    <dt>HTML</dt>
    <dd>HyperText Markup Language</dd>
    <dt>CSS</dt>
    <dd>Cascading Style Sheets</dd>
</dl>
```

#### Havolalar va rasmlar
```html
<!-- Havolalar -->
<a href="https://example.com">Tashqi havola</a>
<a href="#section1">Ichki havola</a>
<a href="mailto:email@example.com">Email havola</a>
<a href="tel:+998901234567">Telefon raqami</a>

<!-- Rasmlar -->
<img src="rasm.jpg" alt="Rasm tavsifi" width="300" height="200">
<img src="https://example.com/rasm.png" alt="Onlayn rasm">

<!-- Rasm bilan havola -->
<a href="https://example.com">
    <img src="logo.png" alt="Kompaniya logotipi">
</a>
```

### 1.4 Jadvallar
```html
<table>
    <thead>
        <tr>
            <th>Ism</th>
            <th>Yosh</th>
            <th>Shahar</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Ali</td>
            <td>25</td>
            <td>Toshkent</td>
        </tr>
        <tr>
            <td>Vali</td>
            <td>30</td>
            <td>Samarqand</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td colspan="3">Jami: 2 kishi</td>
        </tr>
    </tfoot>
</table>
```

### 1.5 Formalar
```html
<form action="/submit" method="POST">
    <!-- Matn kiritish -->
    <label for="name">Ism:</label>
    <input type="text" id="name" name="name" required>
    
    <!-- Email kiritish -->
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
    
    <!-- Parol -->
    <label for="password">Parol:</label>
    <input type="password" id="password" name="password" required>
    
    <!-- Radio tugmalar -->
    <fieldset>
        <legend>Jins:</legend>
        <input type="radio" id="male" name="gender" value="male">
        <label for="male">Erkak</label>
        
        <input type="radio" id="female" name="gender" value="female">
        <label for="female">Ayol</label>
    </fieldset>
    
    <!-- Checkbox -->
    <input type="checkbox" id="agree" name="agree" required>
    <label for="agree">Shartlarga roziman</label>
    
    <!-- Select -->
    <label for="city">Shahar:</label>
    <select id="city" name="city">
        <option value="">Tanlang</option>
        <option value="tashkent">Toshkent</option>
        <option value="samarqand">Samarqand</option>
        <option value="bukhara">Buxoro</option>
    </select>
    
    <!-- Textarea -->
    <label for="message">Xabar:</label>
    <textarea id="message" name="message" rows="4" cols="50"></textarea>
    
    <!-- Submit tugma -->
    <button type="submit">Yuborish</button>
    <button type="reset">Tozalash</button>
</form>
```

### 1.6 Semantic HTML5 elementlar
```html
<header>
    <nav>
        <ul>
            <li><a href="#home">Bosh sahifa</a></li>
            <li><a href="#about">Biz haqimizda</a></li>
            <li><a href="#contact">Aloqa</a></li>
        </ul>
    </nav>
</header>

<main>
    <section id="hero">
        <h1>Xush kelibsiz</h1>
        <p>Bu bizning asosiy sahifamiz</p>
    </section>
    
    <section id="content">
        <article>
            <header>
                <h2>Maqola sarlavhasi</h2>
                <p>Muallif: <strong>Ali Valiyev</strong> | Sana: <time datetime="2024-01-15">15 yanvar, 2024</time></p>
            </header>
            <p>Maqola matni...</p>
            <footer>
                <p>Kategoriya: <mark>Texnologiya</mark></p>
            </footer>
        </article>
        
        <aside>
            <h3>Qo'shimcha ma'lumot</h3>
            <p>Bu yon panel tarkibi</p>
        </aside>
    </section>
</main>

<footer>
    <p>&copy; 2024 Mening saytim. Barcha huquqlar himoyalangan.</p>
</footer>
```

## 2-BO'LIM: CSS ASOSLARI

### 2.1 CSS nima?
CSS (Cascading Style Sheets) - HTML elementlarning ko'rinishini belgilaydigan til. Ranglar, o'lchamlar, joylashuv va boshqa vizual xususiyatlarni boshqaradi.

### 2.2 CSSni ulash usullari

#### 1. Inline CSS
```html
<p style="color: red; font-size: 18px;">Qizil matn</p>
```

#### 2. Internal CSS
```html
<head>
    <style>
        p {
            color: blue;
            font-size: 16px;
        }
    </style>
</head>
```

#### 3. External CSS
```html
<head>
    <link rel="stylesheet" href="styles.css">
</head>
```

### 2.3 CSS selektorlar

#### Asosiy selektorlar
```css
/* Element selektori */
h1 {
    color: red;
}

/* ID selektori */
#header {
    background-color: blue;
}

/* Class selektori */
.highlight {
    background-color: yellow;
}

/* Universal selektor */
* {
    margin: 0;
    padding: 0;
}
```

#### Murakkab selektorlar
```css
/* Descendant selector */
div p {
    color: green;
}

/* Child selector */
div > p {
    font-weight: bold;
}

/* Adjacent sibling */
h1 + p {
    margin-top: 0;
}

/* General sibling */
h1 ~ p {
    color: gray;
}

/* Attribute selector */
input[type="text"] {
    border: 1px solid #ccc;
}

/* Pseudo-class */
a:hover {
    color: red;
}

/* Pseudo-element */
p::first-line {
    font-weight: bold;
}
```

### 2.4 CSS xususiyatlari

#### Matn stillashtirish
```css
.text-style {
    /* Font */
    font-family: Arial, sans-serif;
    font-size: 16px;
    font-weight: bold;
    font-style: italic;
    
    /* Matn rangi va hizalanishi */
    color: #333;
    text-align: center;
    text-decoration: underline;
    text-transform: uppercase;
    
    /* Qator balandligi va harf oraligi */
    line-height: 1.5;
    letter-spacing: 1px;
    word-spacing: 2px;
}
```

#### Box Model
```css
.box {
    /* O'lchami */
    width: 300px;
    height: 200px;
    
    /* Padding (ichki bo'shliq) */
    padding: 20px;
    padding-top: 10px;
    padding-right: 15px;
    padding-bottom: 10px;
    padding-left: 15px;
    
    /* Border */
    border: 2px solid #000;
    border-radius: 10px;
    
    /* Margin (tashqi bo'shliq) */
    margin: 20px;
    margin: 10px 20px; /* vertikal horizontal */
    margin: 10px 15px 10px 15px; /* top right bottom left */
    
    /* Fon */
    background-color: #f0f0f0;
    background-image: url('pattern.png');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
}
```

#### Pozitsiya va display
```css
/* Display turlari */
.block {
    display: block;
}

.inline {
    display: inline;
}

.inline-block {
    display: inline-block;
}

.none {
    display: none;
}

/* Position turlari */
.static {
    position: static; /* standart */
}

.relative {
    position: relative;
    top: 10px;
    left: 20px;
}

.absolute {
    position: absolute;
    top: 50px;
    right: 30px;
}

.fixed {
    position: fixed;
    bottom: 0;
    right: 0;
}

.sticky {
    position: sticky;
    top: 0;
}
```

### 2.5 Flexbox
```css
.flex-container {
    display: flex;
    
    /* Yo'nalish */
    flex-direction: row; /* row, column, row-reverse, column-reverse */
    
    /* Asosiy o'q bo'yicha hizalash */
    justify-content: center; /* flex-start, flex-end, center, space-between, space-around */
    
    /* Kesish o'qi bo'yicha hizalash */
    align-items: center; /* flex-start, flex-end, center, baseline, stretch */
    
    /* O'rash */
    flex-wrap: wrap; /* nowrap, wrap, wrap-reverse */
    
    /* Bo'shliq */
    gap: 20px;
}

.flex-item {
    /* Flex xususiyatlari */
    flex-grow: 1;
    flex-shrink: 0;
    flex-basis: 200px;
    
    /* Yoki qisqacha */
    flex: 1 0 200px; /* grow shrink basis */
    
    /* Alohida hizalash */
    align-self: flex-end;
}
```

### 2.6 CSS Grid
```css
.grid-container {
    display: grid;
    
    /* Grid shablonlari */
    grid-template-columns: 1fr 2fr 1fr;
    grid-template-rows: auto 1fr auto;
    
    /* Yoki repeat bilan */
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(2, 200px);
    
    /* Bo'shliqlar */
    gap: 20px;
    grid-column-gap: 15px;
    grid-row-gap: 10px;
    
    /* Hizalash */
    justify-content: center;
    align-content: center;
    justify-items: stretch;
    align-items: center;
}

.grid-item {
    /* Grid joylashuvi */
    grid-column: 1 / 3;
    grid-row: 2 / 4;
    
    /* Yoki qisqacha */
    grid-area: 2 / 1 / 4 / 3; /* row-start / col-start / row-end / col-end */
    
    /* Alohida hizalash */
    justify-self: end;
    align-self: start;
}

/* Grid template areas */
.grid-layout {
    display: grid;
    grid-template-areas:
        "header header header"
        "sidebar main main"
        "footer footer footer";
    grid-template-columns: 200px 1fr 1fr;
    grid-template-rows: auto 1fr auto;
}

.header { grid-area: header; }
.sidebar { grid-area: sidebar; }
.main { grid-area: main; }
.footer { grid-area: footer; }
```

### 2.7 Responsive dizayn
```css
/* Mobile First yondashuv */
.container {
    width: 100%;
    padding: 10px;
}

/* Tablet */
@media screen and (min-width: 768px) {
    .container {
        max-width: 750px;
        margin: 0 auto;
        padding: 20px;
    }
}

/* Desktop */
@media screen and (min-width: 1024px) {
    .container {
        max-width: 1200px;
        padding: 30px;
    }
}

/* Flexible images */
img {
    max-width: 100%;
    height: auto;
}

/* Responsive typography */
html {
    font-size: 16px;
}

@media screen and (max-width: 768px) {
    html {
        font-size: 14px;
    }
}

/* Responsive Grid */
.responsive-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}
```

### 2.8 CSS animatsiyalar

#### Transitions
```css
.button {
    background-color: blue;
    color: white;
    padding: 10px 20px;
    transition: all 0.3s ease;
}

.button:hover {
    background-color: red;
    transform: scale(1.1);
}

/* Alohida xususiyatlar uchun */
.element {
    transition-property: background-color, transform;
    transition-duration: 0.3s, 0.5s;
    transition-timing-function: ease, ease-in-out;
    transition-delay: 0s, 0.1s;
}
```

#### Keyframe animatsiyalar
```css
@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes bounce {
    0%, 100% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(-20px);
    }
}

.animate-fade-in {
    animation: fadeIn 1s ease-out;
}

.animate-bounce {
    animation: bounce 2s infinite;
}

/* Animation xususiyatlari */
.animation-example {
    animation-name: fadeIn;
    animation-duration: 1s;
    animation-timing-function: ease-out;
    animation-delay: 0.5s;
    animation-iteration-count: 1;
    animation-direction: normal;
    animation-fill-mode: both;
}
```

### 2.9 CSS o'zgaruvchilar (Custom Properties)
```css
:root {
    --primary-color: #007bff;
    --secondary-color: #6c757d;
    --font-size-base: 16px;
    --border-radius: 4px;
    --spacing: 20px;
}

.card {
    background-color: var(--primary-color);
    font-size: var(--font-size-base);
    border-radius: var(--border-radius);
    padding: var(--spacing);
    margin-bottom: calc(var(--spacing) * 2);
}

/* Media query ichida o'zgaruvchilarni o'zgartirish */
@media (max-width: 768px) {
    :root {
        --font-size-base: 14px;
        --spacing: 15px;
    }
}
```

## 3-BO'LIM: AMALIY MISOLLAR

### 3.1 Oddiy veb-sahifa shablon
```html
<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mening saytim</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            color: #333;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            background-color: #2c3e50;
            color: white;
            padding: 1rem 0;
        }
        
        nav ul {
            list-style: none;
            display: flex;
            gap: 2rem;
        }
        
        nav a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        nav a:hover {
            color: #3498db;
        }
        
        main {
            padding: 2rem 0;
        }
        
        .hero {
            text-align: center;
            padding: 4rem 0;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border-radius: 8px;
            margin-bottom: 2rem;
        }
        
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin: 2rem 0;
        }
        
        .feature {
            background: #f8f9fa;
            padding: 1.5rem;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.3s;
        }
        
        .feature:hover {
            transform: translateY(-5px);
        }
        
        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 1rem 0;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <nav>
                <ul>
                    <li><a href="#home">Bosh sahifa</a></li>
                    <li><a href="#about">Biz haqimizda</a></li>
                    <li><a href="#services">Xizmatlar</a></li>
                    <li><a href="#contact">Aloqa</a></li>
                </ul>
            </nav>
        </div>
    </header>
    
    <main>
        <div class="container">
            <section class="hero">
                <h1>Xush kelibsiz!</h1>
                <p>Bu bizning ajoyib veb-saytimiz</p>
            </section>
            
            <section class="features">
                <div class="feature">
                    <h3>Tezlik</h3>
                    <p>Saytimiz juda tez yuklanadi</p>
                </div>
                <div class="feature">
                    <h3>Responsive</h3>
                    <p>Barcha qurilmalarda yaxshi ko'rinadi</p>
                </div>
                <div class="feature">
                    <h3>Zamonaviy</h3>
                    <p>Eng so'nggi texnologiyalar ishlatilgan</p>
                </div>
            </section>
        </div>
    </main>
    
    <footer>
        <div class="container">
            <p>&copy; 2024 Mening saytim. Barcha huquqlar himoyalangan.</p>
        </div>
    </footer>
</body>
</html>
```

### 3.2 Responsive navigatsiya menyusi
```html
<style>
.nav-toggle {
    display: none;
    background: none;
    border: none;
    font-size: 1.5rem;
    cursor: pointer;
    color: white;
}

@media (max-width: 768px) {
    .nav-toggle {
        display: block;
    }
    
    nav ul {
        display: none;
        flex-direction: column;
        position: absolute;
        top: 100%;
        left: 0;
        right: 0;
        background-color: #2c3e50;
        padding: 1rem;
    }
    
    nav ul.active {
        display: flex;
    }
}
</style>

<script>
document.querySelector('.nav-toggle').addEventListener('click', function() {
    document.querySelector('nav ul').classList.toggle('active');
});
</script>
```

## 4-BO'LIM: ENG YAXSHI AMALIYOTLAR

### 4.1 HTML eng yaxshi amaliyotlar
- Semantic taglardan foydalaning
- Alt atributini rasmlarga qo'shing
- Form elementlariga label qo'ying
- W3C validatordan foydalaning
- Accessibility ni hisobga oling

### 4.2 CSS eng yaxshi amaliyotlar
- Mobile-first yondashuvini qo'llang
- CSS o'zgaruvchilardan foydalaning
- Flexbox va Grid dan foydalaning
- Optimized rasmlardan foydalaning
- CSS fayllari hajmini kamaytiring

### 4.3 Performance optimizatsiya
- Rasmlarni siqing
- CSS va JS fayllarini minify qiling
- CDN dan foydalaning
- Lazy loading qo'llang
- Browser cache dan foydalaning

Bu darslik HTML va CSS ning asosiy va ilg'or mavzularini qamrab oladi. Har bir mavzu amaliy misollar bilan tushuntirilgan va real loyihalarda qo'llash mumkin.



## 1.2 Text Content va Typography

### Heading Hierarchy va Best Practices
```html
<!-- Hierarchical structure -->
<article>
    <header>
        <h1>Asosiy sarlavha (faqat bitta sahifada)</h1>
        <p class="subtitle">Qo'shimcha sarlavha</p>
        <time datetime="2024-01-15">15 yanvar, 2024</time>
    </header>
    
    <section>
        <h2>Bo'lim sarlavhasi</h2>
        <p>Bo'lim tarkibi...</p>
        
        <h3>Kichik bo'lim</h3>
        <p>Kichik bo'lim tarkibi...</p>
        
        <h4>Yana kichikroq bo'lim</h4>
        <p>Tafsilotlar...</p>
    </section>
</article>

<!-- Multiple Articles -->
<main>
    <article>
        <h2>Birinchi maqola (h1 dan keyin h2)</h2>
        <!-- content -->
    </article>
    
    <article>
        <h2>Ikkinchi maqola</h2>
        <!-- content -->
    </article>
</main>
```

### Advanced Text Formatting
```html
<!-- Semantic text elements -->
<p>
    <strong>Muhim matn</strong> va <em>ta'kidlangan matn</em>.
    <b>Vizual jihatdan qalin</b> va <i>vizual jihatdan qiyshiq</i>.
    <mark>Belgilangan matn</mark> va <del>o'chirilgan matn</del>.
    <ins>Qo'shilgan matn</ins> va <s>noto'g'ri matn</s>.
</p>

<!-- Subscript va Superscript -->
<p>Kimyoviy formula: H<sub>2</sub>SO<sub>4</sub></p>
<p>Matematik ifoda: E = mc<sup>2</sup></p>

<!-- Code elements -->
<p>JavaScript da <code>console.log()</code> ishlatiladi.</p>

<pre><code>
function hello() {
    console.log("Salom dunyo!");
}
</code></pre>

<p><kbd>Ctrl</kbd> + <kbd>C</kbd> ni bosing.</p>

<!-- Quotes -->
<blockquote cite="https://example.com">
    <p>"Katta iqtibos matni bu yerda joylashadi. Bu juda uzun bo'lishi mumkin va alohida paragrafda ko'rsatiladi."</p>
    <footer>
        — <cite>Muallif ismi</cite>
    </footer>
</blockquote>

<p>Qisqa <q>iqtibos matni</q> paragraf ichida.</p>

<!-- Abbreviations -->
<p><abbr title="HyperText Markup Language">HTML</abbr> veb sahifalar uchun.</p>

<!-- Address -->
<address>
    <p>Aloqa ma'lumotlari:</p>
    <p>
        <a href="mailto:info@example.com">info@example.com</a><br>
        <a href="tel:+998901234567">+998 90 123 45 67</a>
    </p>
</address>

<!-- Ruby annotations (East Asian typography) -->
<ruby>
    漢 <rt>kan</rt>
    字 <rt>ji</rt>
</ruby>
```

## 1.3 Advanced Lists va Navigation

### Complex List Structures
```html
<!-- Nested lists -->
<ul class="main-menu">
    <li>
        <a href="#home">Bosh sahifa</a>
    </li>
    <li>
        <a href="#products">Mahsulotlar</a>
        <ul class="submenu">
            <li><a href="#laptops">Noutbuklar</a></li>
            <li><a href="#phones">Telefonlar</a></li>
            <li>
                <a href="#accessories">Aksessuarlar</a>
                <ul>
                    <li><a href="#cases">Qopqoqlar</a></li>
                    <li><a href="#chargers">Zaryadlovchilar</a></li>
                </ul>
            </li>
        </ul>
    </li>
    <li><a href="#contact">Aloqa</a></li>
</ul>

<!-- Custom ordered lists -->
<ol type="I" start="5">
    <li>Beshinchi element (V)</li>
    <li>Oltinchi element (VI)</li>
    <li>Yettinchi element (VII)</li>
</ol>

<ol type="a" reversed>
    <li>Oxirgi element</li>
    <li>Oxirgidan bitta oldingi</li>
    <li>Oxirgidan ikki oldingi</li>
</ol>

<!-- Definition lists with complex content -->
<dl class="glossary">
    <dt>Frontend Development</dt>
    <dd>
        <p>Foydalanuvchi ko'radigan va o'zaro ta'sir qiladigan veb-sayt qismini yaratish.</p>
        <p>Texnologiyalar: HTML, CSS, JavaScript, React, Vue.js</p>
    </dd>
    
    <dt>Backend Development</dt>
    <dd>Server tomonidagi logika va ma'lumotlar bazasi bilan ishlash.</dd>
    
    <dt>Full Stack</dt>
    <dd>Frontend va Backend ikkalasini ham bilish.</dd>
</dl>

<!-- Task lists (GitHub flavored) -->
<ul class="task-list">
    <li><input type="checkbox" checked disabled> Tugallangan vazifa</li>
    <li><input type="checkbox" disabled> Tugallanmagan vazifa</li>
    <li><input type="checkbox" disabled> Boshqa vazifa</li>
</ul>
```

## 1.4 Advanced Tables

### Complex Table Structure
```html
<figure>
    <figcaption>2024 yil sotuvlar statistikasi</figcaption>
    <table class="data-table">
        <caption>Oylik sotuvlar hisoboti (ming so'mda)</caption>
        <colgroup>
            <col span="1" class="month-col">
            <col span="2" class="product-group-1">
            <col span="2" class="product-group-2">
            <col span="1" class="total-col">
        </colgroup>
        <thead>
            <tr>
                <th rowspan="2" scope="col">Oy</th>
                <th colspan="2" scope="colgroup">Texnika</th>
                <th colspan="2" scope="colgroup">Kiyim</th>
                <th rowspan="2" scope="col">Jami</th>
            </tr>
            <tr>
                <th scope="col">Noutbuk</th>
                <th scope="col">Telefon</th>
                <th scope="col">Ko'ylak</th>
                <th scope="col">Shim</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <th scope="row">Yanvar</th>
                <td>5,200</td>
                <td>8,100</td>
                <td>3,400</td>
                <td>2,800</td>
                <td><strong>19,500</strong></td>
            </tr>
            <tr>
                <th scope="row">Fevral</th>
                <td>6,100</td>
                <td>9,300</td>
                <td>4,200</td>
                <td>3,100</td>
                <td><strong>22,700</strong></td>
            </tr>
            <tr>
                <th scope="row">Mart</th>
                <td>5,800</td>
                <td>7,900</td>
                <td>3,800</td>
                <td>2,900</td>
                <td><strong>20,400</strong></td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <th scope="row">Jami</th>
                <td><strong>17,100</strong></td>
                <td><strong>25,300</strong></td>
                <td><strong>11,400</strong></td>
                <td><strong>8,800</strong></td>
                <td><strong>62,600</strong></td>
            </tr>
        </tfoot>
    </table>
</figure>

<!-- Responsive table wrapper -->
<div class="table-responsive">
    <table>
        <!-- table content -->
    </table>
</div>

<!-- Sortable table headers -->
<table>
    <thead>
        <tr>
            <th>
                <button type="button" aria-label="Ism bo'yicha saralash">
                    Ism <span aria-hidden="true">↕</span>
                </button>
            </th>
            <th>
                <button type="button" aria-label="Yosh bo'yicha saralash">
                    Yosh <span aria-hidden="true">↕</span>
                </button>
            </th>
        </tr>
    </thead>
    <!-- tbody content -->
</table>
```

## 1.5 Professional Forms

### Complete Form Structure
```html
<form action="/submit" method="POST" enctype="multipart/form-data" novalidate>
    <fieldset>
        <legend>Shaxsiy ma'lumotlar</legend>
        
        <!-- Text inputs with validation -->
        <div class="form-group">
            <label for="firstName">Ism <span class="required">*</span></label>
            <input 
                type="text" 
                id="firstName" 
                name="firstName" 
                required 
                minlength="2"
                maxlength="50"
                pattern="[A-Za-z\s]+"
                aria-describedby="firstName-help firstName-error"
                autocomplete="given-name"
            >
            <small id="firstName-help">Faqat harflar va bo'shliqlar</small>
            <div id="firstName-error" class="error-message" aria-live="polite"></div>
        </div>

        <div class="form-group">
            <label for="email">Email manzil <span class="required">*</span></label>
            <input 
                type="email" 
                id="email" 
                name="email" 
                required
                aria-describedby="email-help"
                autocomplete="email"
                placeholder="example@domain.com"
            >
            <small id="email-help">To'g'ri email formatida kiriting</small>
        </div>

        <!-- Phone input -->
        <div class="form-group">
            <label for="phone">Telefon raqami</label>
            <input 
                type="tel" 
                id="phone" 
                name="phone"
                pattern="[+][0-9]{3}[0-9]{2}[0-9]{3}[0-9]{2}[0-9]{2}"
                placeholder="+998901234567"
                autocomplete="tel"
            >
        </div>

        <!-- Date input -->
        <div class="form-group">
            <label for="birthDate">Tug'ilgan sana</label>
            <input 
                type="date" 
                id="birthDate" 
                name="birthDate"
                min="1900-01-01" 
                max="2024-12-31"
                autocomplete="bday"
            >
        </div>
    </fieldset>

    <fieldset>
        <legend>Parol</legend>
        
        <div class="form-group">
            <label for="password">Parol <span class="required">*</span></label>
            <div class="password-container">
                <input 
                    type="password" 
                    id="password" 
                    name="password" 
                    required
                    minlength="8"
                    pattern="(?=.*[a-z])(?=.*[A-Z])(?=.*\d).{8,}"
                    aria-describedby="password-help"
                    autocomplete="new-password"
                >
                <button type="button" class="password-toggle" aria-label="Parolni ko'rsatish/yashirish">
                    👁
                </button>
            </div>
            <small id="password-help">
                Kamida 8 belgidan iborat, katta va kichik harflar, raqamlar bo'lishi kerak
            </small>
        </div>

        <div class="form-group">
            <label for="confirmPassword">Parolni takrorlang <span class="required">*</span></label>
            <input 
                type="password" 
                id="confirmPassword" 
                name="confirmPassword" 
                required
                autocomplete="new-password"
            >
        </div>
    </fieldset>

    <fieldset>
        <legend>Qo'shimcha ma'lumotlar</legend>

        <!-- Radio buttons -->
        <div class="form-group">
            <fieldset class="radio-group">
                <legend>Jins</legend>
                <div class="radio-option">
                    <input type="radio" id="male" name="gender" value="male">
                    <label for="male">Erkak</label>
                </div>
                <div class="radio-option">
                    <input type="radio" id="female" name="gender" value="female">
                    <label for="female">Ayol</label>
                </div>
                <div class="radio-option">
                    <input type="radio" id="other" name="gender" value="other">
                    <label for="other">Boshqa</label>
                </div>
            </fieldset>
        </div>

        <!-- Checkboxes -->
        <div class="form-group">
            <fieldset class="checkbox-group">
                <legend>Qiziqishlar (bir nechtasini tanlash mumkin)</legend>
                <div class="checkbox-option">
                    <input type="checkbox" id="tech" name="interests" value="technology">
                    <label for="tech">Texnologiya</label>
                </div>
                <div class="checkbox-option">
                    <input type="checkbox" id="sport" name="interests" value="sport">
                    <label for="sport">Sport</label>
                </div>
                <div class="checkbox-option">
                    <input type="checkbox" id="music" name="interests" value="music">
                    <label for="music">Musiqa</label>
                </div>
                <div class="checkbox-option">
                    <input type="checkbox" id="travel" name="interests" value="travel">
                    <label for="travel">Sayohat</label>
                </div>
            </fieldset>
        </div>

        <!-- Select dropdown -->
        <div class="form-group">
            <label for="country">Mamlakat</label>
            <select id="country" name="country" autocomplete="country">
                <option value="">Mamlakatni tanlang</option>
                <optgroup label="Markaziy Osiyo">
                    <option value="uz">O'zbekiston</option>
                    <option value="kz">Qozog'iston</option>
                    <option value="kg">Qirg'iziston</option>
                    <option value="tj">Tojikiston</option>
                    <option value="tm">Turkmaniston</option>
                </optgroup>
                <optgroup label="Boshqa mamlakatlar">
                    <option value="ru">Rossiya</option>
                    <option value="us">AQSH</option>
                    <option value="de">Germaniya</option>
                </optgroup>
            </select>
        </div>

        <!-- Multiple select -->
        <div class="form-group">
            <label for="languages">Bilgan tillar (Ctrl tugmasini bosib bir nechtasini tanlang)</label>
            <select id="languages" name="languages" multiple size="4">
                <option value="uz">O'zbek</option>
                <option value="en">Ingliz</option>
                <option value="ru">Rus</option>
                <option value="de">Nemis</option>
                <option value="fr">Fransuz</option>
            </select>
        </div>

        <!-- Textarea -->
        <div class="form-group">
            <label for="bio">O'zingiz haqingizda</label>
            <textarea 
                id="bio" 
                name="bio" 
                rows="4" 
                cols="50"
                maxlength="500"
                placeholder="O'zingiz haqingizda qisqacha yozing..."
            ></textarea>
            <small>Maksimal 500 belgi</small>
        </div>

        <!-- File upload -->
        <div class="form-group">
            <label for="avatar">Profil rasmi</label>
            <input 
                type="file" 
                id="avatar" 
                name="avatar"
                accept="image/*"
                capture="user"
            >
            <small>Faqat rasm fayllari (JPEG, PNG)</small>
        </div>

        <!-- Range input -->
        <div class="form-group">
            <label for="experience">Tajriba (yil)</label>
            <input 
                type="range" 
                id="experience" 
                name="experience"
                min="0" 
                max="20" 
                value="5"
                oninput="document.getElementById('exp-value').textContent = this.value"
            >
            <output id="exp-value">5</output> yil
        </div>

        <!-- Color input -->
        <div class="form-group">
            <label for="favoriteColor">Sevimli rang</label>
            <input type="color" id="favoriteColor" name="favoriteColor" value="#ff0000">
        </div>
    </fieldset>

    <fieldset>
        <legend>Qo'shimcha xizmatlar</legend>
        
        <!-- Agreement checkbox -->
        <div class="form-group">
            <div class="checkbox-option">
                <input type="checkbox" id="newsletter" name="newsletter" value="yes">
                <label for="newsletter">
                    Yangiliklar xatlarini olishni xohlayman
                </label>
            </div>
        </div>

        <div class="form-group">
            <div class="checkbox-option">
                <input type="checkbox" id="terms" name="terms" required>
                <label for="terms">
                    <a href="/terms" target="_blank">Foydalanish shartlari</a>ga roziman <span class="required">*</span>
                </label>
            </div>
        </div>
    </fieldset>

    <!-- Form actions -->
    <div class="form-actions">
        <button type="submit" class="btn btn-primary">
            <span aria-hidden="true">✓</span> Ro'yxatdan o'tish
        </button>
        <button type="reset" class="btn btn-secondary">
            <span aria-hidden="true">↻</span> Tozalash
        </button>
        <button type="button" class="btn btn-outline" onclick="history.back()">
            <span aria-hidden="true">←</span> Orqaga
        </button>
    </div>
</form>
```

## 1.6 Modern HTML5 Elements

### Semantic Structure
```html
<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modern veb sayt</title>
</head>
<body>
    <!-- Skip to main content (accessibility) -->
    <a href="#main" class="skip-link">Asosiy tarkibga o'tish</a>

    <!-- Header -->
    <header role="banner">
        <div class="container">
            <div class="logo">
                <img src="logo.png" alt="Kompaniya logotipi">
            </div>
            
            <nav role="navigation" aria-label="Asosiy navigatsiya">
                <ul>
                    <li><a href="#home" aria-current="page">Bosh sahifa</a></li>
                    <li><a href="#about">Biz haqimizda</a></li>
                    <li><a href="#services">Xizmatlar</a></li>
                    <li><a href="#blog">Blog</a></li>
                    <li><a href="#contact">Aloqa</a></li>
                </ul>
            </nav>

            <!-- Mobile menu button -->
            <button class="menu-toggle" aria-expanded="false" aria-controls="main-nav">
                <span class="sr-only">Menyu ochish</span>
                <span class="hamburger"></span>
            </button>
        </div>
    </header>

    <!-- Main content -->
    <main id="main" role="main">
        <!-- Hero section -->
        <section class="hero" aria-labelledby="hero-title">
            <div class="hero-content">
                <h1 id="hero-title">Xush kelibsiz bizning saytimizga</h1>
                <p class="hero-description">
                    Biz professional veb yechimlari taklif etamiz
                </p>
                <div class="hero-actions">
                    <a href="#services" class="btn btn-primary">Xizmatlarni ko'rish</a>
                    <a href="#contact" class="btn btn-outline">Bog'lanish</a>
                </div>
            </div>
            <figure class="hero-image">
                <img src="hero.jpg" alt="Jamoaviy ish jarayoni">
            </figure>
        </section>

        <!-- Features section -->
        <section class="features" aria-labelledby="features-title">
            <div class="container">
                <header class="section-header">
                    <h2 id="features-title">Bizning afzalliklarimiz</h2>
                    <p>Nima uchun bizni tanlashingiz kerak</p>
                </header>

                <div class="features-grid">
                    <article class="feature-card">
                        <header>
                            <div class="feature-icon" aria-hidden="true">🚀</div>
                            <h3>Tezlik</h3>
                        </header>
                        <p>Saytlarimiz juda tez yuklanadi va optimallashtirilgan</p>
                        <footer>
                            <a href="#speed-details">Batafsil</a>
                        </footer>
                    </article>

                    <article class="feature-card">
                        <header>
                            <div class="feature-icon" aria-hidden="true">📱</div>
                            <h3>Responsive</h3>
                        </header>
                        <p>Barcha qurilmalarda mukammal ko'rinish</p>
                        <footer>
                            <a href="#responsive-details">Batafsil</a>
                        </footer>
                    </article>

                    <article class="feature-card">
                        <header>
                            <div class="feature-icon" aria-hidden="true">🔒</div>
                            <h3>Xavfsizlik</h3>
                        </header>
                        <p>Zamonaviy xavfsizlik standartlari</p>
                        <footer>
                            <a href="#security-details">Batafsil</a>
                        </footer>
                    </article>
                </div>
            </div>
        </section>

        <!-- Blog section -->
        <section class="blog" aria-labelledby="blog-title">
            <div class="container">
                <header class="section-header">
                    <h2 id="blog-title">So'nggi maqolalar</h2>
                </header>

                <div class="blog-grid">
                    <article class="blog-card">
                        <figure class="blog-image">
                            <img src="blog1.jpg" alt="Web dizayn tendensiyalari">
                        </figure>
                        <div class="blog-content">
                            <header>
                                <h3><a href="/blog/web-design-trends">2024 yil veb dizayn tendensiyalari</a></h3>
                                <div class="blog-meta">
                                    <time datetime="2024-01-15">15 yanvar, 2024</time>
                                    <span class="author">Muallif: <a href="/authors/john">John Doe</a></span>
                                    <span class="category">Kategoriya: <a href="/category/design">Dizayn</a></span>
                                </div>
                            </header>
                            <p>Bu yil eng mashhur veb dizayn tendensiyalari haqida...</p>
                            <footer class="blog-footer">
                                <div class="blog-tags">
                                    <a href="/tag/design" class="tag">dizayn</a>
                                    <a href="/tag/trends" class="tag">tendensiyalar</a>
                                    <a href="/tag/2024" class="tag">2024</a>
                                </div>
                                <a href="/blog/web-design-trends" class="read-more">To'liqini o'qish</a>
                            </footer>
                        </div>
                    </article>

                    <!-- More blog articles... -->
                </div>
            </div>
        </section>

        <!-- Contact section -->
        <section class="contact" aria-labelledby="contact-title">
            <div class="container">
                <header class="section-header">
                    <h2 id="contact-title">Biz bilan bog'laning</h2>
                </header>

                <div class="contact-content">
                    <div class="contact-info">
                        <address>
                            <h3>Bizning manzilimiz</h3>
                            <p>
                                <strong>Kompaniya nomi</strong><br>
                                Toshkent shahri, Yunusobod tumani<br>
                                Amir Temur ko'chasi, 123-uy<br>
                                100000, O'zbekiston
                            </p>
                            <p>
                                Tel: <a href="tel:+998712345678">+998 71 234 56 78</a><br>
                                Email: <a href="mailto:info@company.uz">info@company.uz</a>
                            </p>
                        </address>

                        <!-- Social links -->
                        <div class="social-links">
                            <h3>Ijtimoiy tarmoqlar</h3>
                            <ul>
                                <li>
                                    <a href="https://facebook.com/company" aria-label="Facebook sahifamiz">
                                        <span aria-hidden="true">📘</span> Facebook
                                    </a>
                                </li>
                                <li>
                                    <a href="https://twitter.com/company" aria-label="Twitter sahifamiz">
                                        <span aria-hidden="true">🐦</span> Twitter
                                    </a>
                                </li>
                                <li>
                                    <a href="https://instagram.com/company" aria-label="Instagram sahifamiz">
                                        <span aria-hidden="true">📷</span> Instagram
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>

                    <!-- Contact form -->
                    <div class="contact-form">
                        <form action="/contact" method="POST">
                            <div class="form-group">
                                <label for="contact-name">Ismingiz</label>
                                <input type="text" id="contact-name" name="name" required>
                            </div>
                            <div class="form-group">
                                <label for="contact-email">Email</label>
                                <input type="email" id="contact-email" name="email" required>
                            </div>
                            <div class="form-group">
                                <label for="contact-subject">Mavzu</label>
                                <input type="text" id="contact-subject" name="subject" required>
                            </div>
                            <div class="form-group">
                                <label for="contact-message">Xabar</label>
                                <textarea id="contact-message" name="message" rows="5" required></textarea>
                            </div>
                            <button type="submit" class="btn btn-primary">Xabar yuborish</button>
                        </form>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Sidebar (optional) -->
    <aside role="complementary" aria-labelledby="sidebar-title">
        <h2 id="sidebar-title" class="sr-only">Qo'shimcha ma'lumotlar</h2>
        
        <section class="widget" aria-labelledby="recent-posts">
            <h3 id="recent-posts">So'nggi maqolalar</h3>
            <ul>
                <li><a href="/post1">Birinchi maqola</a></li>
                <li><a href="/post2">Ikkinchi maqola</a></li>
                <li><a href="/post3">Uchinchi maqola</a></li>
            </ul>
        </section>

        <section class="widget" aria-labelledby="newsletter">
            <h3 id="newsletter">Yangiliklar</h3>
            <p>Bizning yangiliklar xatlarimizga obuna bo'ling</p>
            <form action="/subscribe" method="POST">
                <div class="form-group">
                    <label for="newsletter-email" class="sr-only">Email manzili</label>
                    <input 
                        type="email" 
                        id="newsletter-email" 
                        name="email" 
                        placeholder="Email manzilingiz"
                        required
                    >
                </div>
                <button type="submit" class="btn btn-small">Obuna bo'lish</button>
            </form>
        </section>
    </aside>

    <!-- Footer -->
    <footer role="contentinfo">
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>Kompaniya</h3>
                    <nav aria-label="Footer navigatsiya">
                        <ul>
                            <li><a href="/about">Biz haqimizda</a></li>
                            <li><a href="/team">Jamoa</a></li>
                            <li><a href="/careers">Karyera</a></li>
                            <li><a href="/press">Matbuot</a></li>
                        </ul>
                    </nav>
                </div>

                <div class="footer-section">
                    <h3>Xizmatlar</h3>
                    <ul>
                        <li><a href="/web-design">Veb dizayn</a></li>
                        <li><a href="/development">Dasturlash</a></li>
                        <li><a href="/seo">SEO</a></li>
                        <li><a href="/marketing">Marketing</a></li>
                    </ul>
                </div>

                <div class="footer-section">
                    <h3>Qo'llab-quvvatlash</h3>
                    <ul>
                        <li><a href="/help">Yordam</a></li>
                        <li><a href="/contact">Aloqa</a></li>
                        <li><a href="/faq">FAQ</a></li>
                        <li><a href="/documentation">Hujjatlar</a></li>
                    </ul>
                </div>

                <div class="footer-section">
                    <h3>Huquqiy</h3>
                    <ul>
                        <li><a href="/privacy">Maxfiylik</a></li>
                        <li><a href="/terms">Shartlar</a></li>
                        <li><a href="/cookies">Cookie</a></li>
                        <li><a href="/disclaimer">Rad etish</a></li>
                    </ul>
                </div>
            </div>

            <div class="footer-bottom">
                <p>&copy; 2024 Kompaniya nomi. Barcha huquqlar himoyalangan.</p>
                <div class="footer-meta">
                    <span>Sayt versiyasi: 2.1.0</span>
                    <span>Oxirgi yangilanish: <time datetime="2024-01-15">15.01.2024</time></span>
                </div>
            </div>
        </div>
    </footer>

    <!-- Back to top button -->
    <button class="back-to-top" aria-label="Sahifa boshiga qaytish" style="display: none;">
        <span aria-hidden="true">↑</span>
    </button>

    <!-- Scripts -->
    <script src="scripts/main.js" defer></script>
</body>
</html>
```

## 1.7 Advanced HTML5 API Elements

### Media Elements
```html
<!-- Advanced Video -->
<figure class="video-container">
    <video 
        controls 
        preload="metadata"
        poster="video-poster.jpg"
        width="800" 
        height="450"
        crossorigin="anonymous"
    >
        <source src="video.mp4" type="video/mp4">
        <source src="video.webm" type="video/webm">
        <source src="video.ogv" type="video/ogg">
        
        <!-- Subtitles -->
        <track 
            kind="subtitles" 
            src="subtitles-uz.vtt" 
            srclang="uz" 
            label="O'zbek"
            default
        >
        <track 
            kind="subtitles" 
            src="subtitles-en.vtt" 
            srclang="en" 
            label="English"
        >
        <track 
            kind="captions" 
            src="captions-uz.vtt" 
            srclang="uz" 
            label="O'zbek (Tinglash qiyinchilik)"
        >
        
        <!-- Fallback content -->
        <p>Sizning brauzeringiz video playerni qo'llab-quvvatlamaydi.</p>
        <a href="video.mp4">Videoni yuklab oling</a>
    </video>
    <figcaption>
        Video tavsifi: Kompaniya taqdimoti
    </figcaption>
</figure>

<!-- Advanced Audio -->
<figure class="audio-container">
    <audio controls preload="metadata" crossorigin="anonymous">
        <source src="audio.mp3" type="audio/mpeg">
        <source src="audio.ogg" type="audio/ogg">
        <source src="audio.wav" type="audio/wav">
        
        <!-- Fallback -->
        <p>Sizning brauzeringiz audio playerni qo'llab-quvvatlamaydi.</p>
        <a href="audio.mp3">Audio faylni yuklab oling</a>
    </audio>
    <figcaption>Podcast epizodi #15: Web Development</figcaption>
</figure>

<!-- Picture element for responsive images -->
<picture>
    <source 
        media="(min-width: 1200px)" 
        srcset="hero-large.webp 1200w, hero-large@2x.webp 2400w"
        type="image/webp"
    >
    <source 
        media="(min-width: 768px)" 
        srcset="hero-medium.webp 768w, hero-medium@2x.webp 1536w"
        type="image/webp"
    >
    <source 
        srcset="hero-small.webp 320w, hero-small@2x.webp 640w"
        type="image/webp"
    >
    <!-- Fallback -->
    <img 
        src="hero-medium.jpg" 
        srcset="hero-small.jpg 320w, hero-medium.jpg 768w, hero-large.jpg 1200w"
        sizes="(min-width: 1200px) 1200px, (min-width: 768px) 768px, 320px"
        alt="Hero rasm tavsifi"
        loading="lazy"
        decoding="async"
    >
</picture>
```

### Interactive Elements
```html
<!-- Details/Summary -->
<details class="faq-item">
    <summary>Savollar va javoblar bo'limi</summary>
    <div class="faq-content">
        <h4>Birinchi savol</h4>
        <p>Bu birinchi savolga javob.</p>
        
        <h4>Ikkinchi savol</h4>
        <p>Bu ikkinchi savolga javob.</p>
    </div>
</details>

<details open>
    <summary>Bu bo'lim ochiq holda ko'rsatiladi</summary>
    <p>Bu bo'lim sahifa yuklanganida ochiq bo'ladi.</p>
</details>

<!-- Dialog element -->
<dialog id="modal-dialog" aria-labelledby="modal-title" aria-describedby="modal-description">
    <header class="modal-header">
        <h2 id="modal-title">Modal oyna sarlavhasi</h2>
        <button type="button" class="modal-close" aria-label="Modalni yopish">×</button>
    </header>
    <div id="modal-description" class="modal-body">
        <p>Modal oyna tarkibi bu yerda.</p>
    </div>
    <footer class="modal-footer">
        <button type="button" class="btn btn-primary">Tasdiqlash</button>
        <button type="button" class="btn btn-secondary">Bekor qilish</button>
    </footer>
</dialog>

<!-- Meter element -->
<div class="progress-container">
    <label for="file-progress">Fayl yuklash jarayoni:</label>
    <meter id="file-progress" min="0" max="100" value="75">75%</meter>
    <span>75%</span>
</div>

<div class="disk-usage">
    <label for="disk-usage">Disk ishlatilishi:</label>
    <meter 
        id="disk-usage" 
        min="0" 
        max="100" 
        low="20" 
        high="80" 
        optimum="30" 
        value="65"
    >
        65%
    </meter>
</div>

<!-- Progress element -->
<div class="download-progress">
    <label for="download">Yuklab olish:</label>
    <progress id="download" max="100" value="45">45%</progress>
</div>

<!-- Indeterminate progress -->
<progress>Yuklanmoqda...</progress>
```

### Canvas va SVG
```html
<!-- Canvas -->
<figure class="canvas-container">
    <canvas 
        id="myCanvas" 
        width="800" 
        height="400"
        aria-label="Interaktiv grafik"
    >
        Sizning brauzeringiz canvas elementini qo'llab-quvvatlamaydi.
        <img src="canvas-fallback.png" alt="Grafik tasviri">
    </canvas>
    <figcaption>Interaktiv grafik (Canvas)</figcaption>
</figure>

<!-- Inline SVG -->
<svg 
    width="200" 
    height="200" 
    viewBox="0 0 200 200"
    role="img"
    aria-labelledby="svg-title svg-desc"
>
    <title id="svg-title">Doira grafik</title>
    <desc id="svg-desc">Qizil rangli doira va ko'k rangli kvadrat</desc>
    
    <circle cx="50" cy="50" r="40" fill="red" />
    <rect x="100" y="10" width="80" height="80" fill="blue" />
</svg>

<!-- External SVG -->
<object 
    data="diagram.svg" 
    type="image/svg+xml"
    width="300" 
    height="200"
    aria-label="Kompaniya diagrammasi"
>
    <img src="diagram.png" alt="Kompaniya diagrammasi">
</object>
```

---

# 🎨 2-BO'LIM: CSS - PROFESSIONAL MUKAMMAL DARAJA

## 2.1 CSS Architecture va Metodologiya

### CSS Reset va Normalize
```css
/* Modern CSS Reset */
*,
*::before,
*::after {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    line-height: 1.15;
    -webkit-text-size-adjust: 100%;
    -moz-text-size-adjust: 100%;
    text-size-adjust: 100%;
}

body {
    margin: 0;
    font-family: system-ui, -apple-system, 'Segoe UI', 'Roboto', sans-serif;
    line-height: 1.6;
    color: #333;
    background-color: #fff;
}

/* Remove list styles */
ol[role="list"],
ul[role="list"] {
    list-style: none;
}

/* Make images easier to work with */
img,
picture,
video,
canvas,
svg {
    display: block;
    max-width: 100%;
    height: auto;
}

/* Inherit fonts for inputs and buttons */
input,
button,
textarea,
select {
    font: inherit;
}

/* Remove default button styles */
button {
    background: none;
    border: none;
    cursor: pointer;
}

/* Improve text rendering */
h1, h2, h3, h4, h5, h6 {
    text-wrap: balance;
}

p {
    text-wrap: pretty;
    max-width: 75ch;
}

/* Reduce motion for users who prefer it */
@media (prefers-reduced-motion: reduce) {
    *,
    *::before,
    *::after {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
        scroll-behavior: auto !important;
    }
}
```

### CSS Custom Properties (Variables) - Advanced
```css
:root {
    /* Color System */
    --primary-hue: 220;
    --primary-saturation: 80%;
    
    --primary-50: hsl(var(--primary-hue), var(--primary-saturation), 95%);
    --primary-100: hsl(var(--primary-hue), var(--primary-saturation), 85%);
    --primary-200: hsl(var(--primary-hue), var(--primary-saturation), 75%);
    --primary-500: hsl(var(--primary-hue), var(--primary-saturation), 50%);
    --primary-600: hsl(var(--primary-hue), var(--primary-saturation), 40%);
    --primary-900: hsl(var(--primary-hue), var(--primary-saturation), 10%);
    
    /* Semantic Colors */
    --color-success: #22c55e;
    --color-warning: #f59e0b;
    --color-error: #ef4444;
    --color-info: #3b82f6;
    
    /* Neutral Colors */
    --gray-50: #f9fafb;
    --gray-100: #f3f4f6;
    --gray-200: #e5e7eb;
    --gray-300: #d1d5db;
    --gray-400: #9ca3af;
    --gray-500: #6b7280;
    --gray-600: #4b5563;
    --gray-700: #374151;
    --gray-800: #1f2937;
    --gray-900: #111827;
    
    /* Typography Scale */
    --font-family-sans: system-ui, -apple-system, 'Segoe UI', Roboto, sans-serif;
    --font-family-serif: Georgia, 'Times New Roman', serif;
    --font-family-mono: 'Fira Code', Consolas, 'Courier New', monospace;
    
    --font-size-xs: 0.75rem;    /* 12px */
    --font-size-sm: 0.875rem;   /* 14px */
    --font-size-base: 1rem;     /* 16px */
    --font-size-lg: 1.125rem;   /* 18px */
    --font-size-xl: 1.25rem;    /* 20px */
    --font-size-2xl: 1.5rem;    /* 24px */
    --font-size-3xl: 1.875rem;  /* 30px */
    --font-size-4xl: 2.25rem;   /* 36px */
    --font-size-5xl: 3rem;      /* 48px */
    --font-size-6xl: 3.75rem;   /* 60px */
    
    --font-weight-light: 300;
    --font-weight-normal: 400;
    --font-weight-medium: 500;
    --font-weight-semibold: 600;
    --font-weight-bold: 700;
    --font-weight-extrabold: 800;
    
    --line-height-tight: 1.25;
    --line-height-normal: 1.6;
    --line-height-relaxed: 1.75;
    
    /* Spacing Scale */
    --space-0: 0;
    --space-1: 0.25rem;   /* 4px */
    --space-2: 0.5rem;    /* 8px */
    --space-3: 0.75rem;   /* 12px */
    --space-4: 1rem;      /* 16px */
    --space-5: 1.25rem;   /* 20px */
    --space-6: 1.5rem;    /* 24px */
    --space-8: 2rem;      /* 32px */
    --space-10: 2.5rem;   /* 40px */
    --space-12: 3rem;     /* 48px */
    --space-16: 4rem;     /* 64px */
    --space-20: 5rem;     /* 80px */
    --space-24: 6rem;     /* 96px */
    --space-32: 8rem;     /* 128px */
    
    /* Border Radius */
    --radius-sm: 0.125rem;
    --radius-base: 0.25rem;
    --radius-md: 0.375rem;
    --radius-lg: 0.5rem;
    --radius-xl: 0.75rem;
    --radius-2xl: 1rem;
    --radius-full: 9999px;
    
    /* Shadows */
    --shadow-sm: 0 1px 2px 0 rgb(0 0 0 / 0.05);
    --shadow-base: 0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);
    --shadow-md: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
    --shadow-lg: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);
    --shadow-xl: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);
    --shadow-2xl: 0 25px 50px -12px rgb(0 0 0 / 0.25);
    
    /* Z-Index Scale */
    --z-dropdown: 1000;
    --z-sticky: 1020;
    --z-fixed: 1030;
    --z-modal-backdrop: 1040;
    --z-modal: 1050;
    --z-popover: 1060;
    --z-tooltip: 1070;
    --z-toast: 1080;
    
    /* Animation */
    --duration-fast: 150ms;
    --duration-normal: 300ms;
    --duration-slow: 500ms;
    
    --easing-linear: linear;
    --easing-ease: ease;
    --easing-ease-in: ease-in;
    --easing-ease-out: ease-out;
    --easing-ease-in-out: ease-in-out;
    --easing-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);
    
    /* Container widths */
    --container-sm: 640px;
    --container-md: 768px;
    --container-lg: 1024px;
    --container-xl: 1280px;
    --container-2xl: 1536px;
}

/* Dark theme */
[data-theme="dark"] {
    --primary-50: hsl(var(--primary-hue), var(--primary-saturation), 10%);
    --primary-100: hsl(var(--primary-hue), var(--primary-saturation), 20%);
    --primary-200: hsl(var(--primary-hue), var(--primary-saturation), 30%);
    --primary-500: hsl(var(--primary-hue), var(--primary-saturation), 60%);
    --primary-600: hsl(var(--primary-hue), var(--primary-saturation), 70%);
    --primary-900: hsl(var(--primary-hue), var(--primary-saturation), 90%);
}

/* System theme preference */
@media (prefers-color-scheme: dark) {
    :root {
        color-scheme: dark;
        /* Dark theme variables */
    }
}
```

## 2.2 Advanced Selectors va Pseudo-classes

### Complex Selectors
```css
/* Attribute selectors */
/* Exact match */
input[type="email"] { border-color: blue; }

/* Contains */
[class*="btn"] { padding: 0.5rem 1rem; }

/* Starts with */
[class^="icon-"] { font-family: 'Icons'; }

/* Ends with */
[class$="-large"] { font-size: 1.25rem; }

/* Word match */
[title~="important"] { color: red; }

/* Language match */
[lang|="en"] { font-style: italic; }

/* Case insensitive */
[title*="important" i] { color: red; }

/* Multiple attributes */
input[type="text"][required] { 
    border: 2px solid var(--color-error);
}

/* Advanced pseudo-classes */
/* Structural pseudo-classes */
li:first-child { margin-top: 0; }
li:last-child { margin-bottom: 0; }
li:only-child { text-align: center; }

tr:nth-child(even) { background-color: var(--gray-50); }
tr:nth-child(odd) { background-color: white; }
tr:nth-child(3n) { font-weight: bold; }
tr:nth-child(3n+1) { color: red; }

p:nth-last-child(2) { margin-bottom: var(--space-8); }

/* Type-based pseudo-classes */
h2:first-of-type { margin-top: 0; }
h2:last-of-type { margin-bottom: var(--space-12); }
img:only-of-type { display: block; margin: 0 auto; }

/* UI state pseudo-classes */
input:valid { border-color: var(--color-success); }
input:invalid { border-color: var(--color-error); }
input:required { position: relative; }
input:required::after {
    content: "*";
    color: var(--color-error);
    position: absolute;
    right: -15px;
}

input:optional { opacity: 0.8; }
input:disabled { 
    opacity: 0.5;
    cursor: not-allowed;
}

input:checked + label { font-weight: bold; }
input:indeterminate { opacity: 0.7; }

/* Link pseudo-classes */
a:link { color: var(--primary-500); }
a:visited { color: var(--primary-600); }
a:hover { color: var(--primary-400); }
a:active { color: var(--primary-700); }
a:focus { outline: 2px solid var(--primary-300); }

/* Advanced interaction pseudo-classes */
.button:hover:not(:disabled) {
    transform: translateY(-2px);
}

.card:focus-within {
    box-shadow: var(--shadow-lg);
}

/* Root and empty pseudo-classes */
:root { /* Already defined above */ }
p:empty { display: none; }

/* Target pseudo-class */
:target {
    background-color: var(--primary-50);
    animation: highlight 2s ease-out;
}

@keyframes highlight {
    from { background-color: var(--primary-200); }
    to { background-color: var(--primary-50); }
}

/* Language pseudo-class */
:lang(uz) { font-family: 'Uzbek Font', sans-serif; }
:lang(en) { font-family: 'English Font', sans-serif; }
```

### Pseudo-elements
```css
/* First letter and first line */
.article::first-letter {
    font-size: 3em;
    font-weight: bold;
    float: left;
    line-height: 1;
    margin-right: 0.1em;
    margin-top: 0.1em;
}

.article::first-line {
    font-variant: small-caps;
    font-weight: bold;
}

/* Selection */
::selection {
    background-color: var(--primary-100);
    color: var(--primary-900);
}

::-moz-selection {
    background-color: var(--primary-100);
    color: var(--primary-900);
}

/* Placeholder */
input::placeholder {
    color: var(--gray-400);
    opacity: 1;
}

input::-webkit-input-placeholder { color: var(--gray-400); }
input::-moz-placeholder { color: var(--gray-400); }
input:-ms-input-placeholder { color: var(--gray-400); }

/* Before and After (most powerful) */
.quote::before {
    content: """;
    font-size: 2em;
    color: var(--primary-300);
    position: absolute;
    left: -0.5em;
    top: -0.2em;
}

.quote::after {
    content: """;
    font-size: 2em;
    color: var(--primary-300);
    position: absolute;
    right: -0.5em;
    bottom: -0.5em;
}

/* Counter example */
.counter {
    counter-reset: step-counter;
}

.step::before {
    counter-increment: step-counter;
    content: "Qadam " counter(step-counter) ": ";
    font-weight: bold;
    color: var(--primary-500);
}

/* Advanced content property */
.external-link::after {
    content: " (" attr(href) ")";
    font-size: 0.8em;
    color: var(--gray-500);
}

.tooltip {
    position: relative;
}

.tooltip::before {
    content: attr(data-tooltip);
    position: absolute;
    bottom: 100%;
    left: 50%;
    transform: translateX(-50%);
    padding: 0.5rem;
    background: var(--gray-900);
    color: white;
    border-radius: var(--radius-base);
    font-size: var(--font-size-sm);
    white-space: nowrap;
    opacity: 0;
    pointer-events: none;
    transition: opacity var(--duration-normal);
}

.tooltip:hover::before {
    opacity: 1;
}

/* Checkbox ve Radio styling */
.custom-checkbox {
    position: relative;
}

.custom-checkbox input[type="checkbox"] {
    position: absolute;
    opacity: 0;
}

.custom-checkbox input[type="checkbox"] + label::before {
    content: "";
    display: inline-block;
    width: 1rem;
    height: 1rem;
    border: 2px solid var(--gray-300);
    border-radius: var(--radius-sm);
    margin-right: var(--space-2);
    vertical-align: middle;
    transition: all var(--duration-normal);
}

.custom-checkbox input[type="checkbox"]:checked + label::before {
    background-color: var(--primary-500);
    border-color: var(--primary-500);
}

.custom-checkbox input[type="checkbox"]:checked + label::after {
    content: "✓";
    position: absolute;
    left: 3px;
    top: -2px;
    color: white;
    font-size: 0.8rem;
}

.custom-checkbox input[type="checkbox"]:focus + label::before {
    outline: 2px solid var(--primary-300);
    outline-offset: 2px;
}
```

## 2.3 Modern Layout Systems

### CSS Grid - Advanced
```css
/* Grid Container Setup */
.grid-layout {
    display: grid;
    grid-template-columns: 
        [full-start] minmax(var(--space-4), 1fr)
        [main-start] repeat(12, [col-start] 1fr [col-end])
        [main-end] minmax(var(--space-4), 1fr) [full-end];
    grid-template-rows: auto 1fr auto;
    min-height: 100vh;
    gap: var(--space-4);
}

/* Named Grid Areas */
.grid-template {
    display: grid;
    grid-template-areas:
        "header header header"
        "sidebar main aside"
        "footer footer footer";
    grid-template-columns: 250px 1fr 200px;
    grid-template-rows: auto 1fr auto;
    gap: var(--space-4);
    min-height: 100vh;
}

.header { grid-area: header; }
.sidebar { grid-area: sidebar; }
.main { grid-area: main; }
.aside { grid-area: aside; }
.footer { grid-area: footer; }

/* Responsive Grid Areas */
@media (max-width: 768px) {
    .grid-template {
        grid-template-areas:
            "header"
            "main"
            "sidebar"
            "aside"
            "footer";
        grid-template-columns: 1fr;
    }
}

/* Advanced Grid Positioning */
.grid-item-featured {
    grid-column: col-start 1 / col-end 6;
    grid-row: 1 / 3;
}

.grid-item-span {
    grid-column: span 4;
    grid-row: span 2;
}

/* Implicit Grid */
.auto-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-auto-rows: minmax(200px, auto);
    gap: var(--space-4);
}

.auto-grid-dense {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    grid-auto-flow: dense;
    gap: var(--space-4);
}

/* Subgrid (Modern browsers) */
.subgrid-container {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: var(--space-4);
}

.subgrid-item {
    display: grid;
    grid-template-columns: subgrid;
    grid-column: span 2;
}

/* Grid Alignment */
.grid-center {
    display: grid;
    place-items: center;
    min-height: 100vh;
}

.grid-alignment {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: var(--space-4);
    
    /* Container alignment */
    justify-content: space-between;
    align-content: center;
    
    /* Items alignment */
    justify-items: stretch;
    align-items: start;
}

.grid-item-self {
    justify-self: end;
    align-self: center;
}
```

### Flexbox - Advanced
```css
/* Complex Flex Layouts */
.flex-complex {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: flex-start;
    align-content: space-around;
    gap: var(--space-4);
}

/* Flexible Navigation */
.nav-flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: var(--space-4);
}

.nav-brand {
    flex: 0 0 auto;
}

.nav-menu {
    display: flex;
    flex: 1 1 auto;
    justify-content: center;
    gap: var(--space-6);
}

.nav-actions {
    display: flex;
    flex: 0 0 auto;
    gap: var(--space-2);
}

/* Responsive Flex */
@media (max-width: 768px) {
    .nav-flex {
        flex-direction: column;
    }
    
    .nav-menu {
        order: 3;
        width: 100%;
        justify-content: space-around;
    }
    
    .nav-actions {
        order: 2;
    }
}

/* Flex Grow/Shrink Examples */
.sidebar {
    flex: 0 0 250px; /* Don't grow, don't shrink, 250px basis */
}

.main-content {
    flex: 1 1 0%; /* Grow, shrink, 0 basis */
}

.aside {
    flex: 0 1 200px; /* Don't grow, can shrink, 200px basis */
}

/* Holy Grail Layout with Flexbox */
.holy-grail {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

.holy-grail-header,
.holy-grail-footer {
    flex: 0 0 auto;
}

.holy-grail-body {
    display: flex;
    flex: 1 1 auto;
}

.holy-grail-content {
    flex: 1 1 auto;
    order: 2;
}

.holy-grail-nav {
    flex: 0 0 200px;
    order: 1;
}

.holy-grail-ads {
    flex: 0 0 150px;
    order: 3;
}

/* Responsive Holy Grail */
@media (max-width: 768px) {
    .holy-grail-body {
        flex-direction: column;
    }
    
    .holy-grail-nav,
    .holy-grail-ads {
        order: 0;
        flex: 0 0 auto;
    }
}

/* Flex utilities */
.flex { display: flex; }
.inline-flex { display: inline-flex; }

.flex-row { flex-direction: row; }
.flex-col { flex-direction: column; }
.flex-row-reverse { flex-direction: row-reverse; }
.flex-col-reverse { flex-direction: column-reverse; }

.flex-wrap { flex-wrap: wrap; }
.flex-nowrap { flex-wrap: nowrap; }
.flex-wrap-reverse { flex-wrap: wrap-reverse; }

.justify-start { justify-content: flex-start; }
.justify-end { justify-content: flex-end; }
.justify-center { justify-content: center; }
.justify-between { justify-content: space-between; }
.justify-around { justify-content: space-around; }
.justify-evenly { justify-content: space-evenly; }

.items-start { align-items: flex-start; }
.items-end { align-items: flex-end; }
.items-center { align-items: center; }
.items-baseline { align-items: baseline; }
.items-stretch { align-items: stretch; }

.flex-1 { flex: 1 1 0%; }
.flex-auto { flex: 1 1 auto; }
.flex-initial { flex: 0 1 auto; }
.flex-none { flex: none; }
```

### Container Queries (Modern CSS)
```css
/* Container Query Setup */
.card-container {
    container-type: inline-size;
    container-name: card;
}

/* Container Query Rules */
@container card (min-width: 300px) {
    .card {
        display: flex;
        gap: var(--space-4);
    }
    
    .card-image {
        flex: 0 0 120px;
    }
    
    .card-content {
        flex: 1;
    }
}

@container card (min-width: 500px) {
    .card {
        flex-direction: column;
    }
    
    .card-image {
        flex: none;
        aspect-ratio: 16 / 9;
    }
}

/* Multiple Container Queries */
.sidebar {
    container-type: inline-size;
    container-name: sidebar;
}

@container sidebar (max-width: 250px) {
    .sidebar-nav {
        display: none;
    }
    
    .sidebar-toggle {
        display: block;
    }
}
```

## 2.4 Advanced Typography

### Modern Typography System
```css
/* Typography Scale */
.text-xs { font-size: var(--font-size-xs); line-height: 1rem; }
.text-sm { font-size: var(--font-size-sm); line-height: 1.25rem; }
.text-base { font-size: var(--font-size-base); line-height: var(--line-height-normal); }
.text-lg { font-size: var(--font-size-lg); line-height: 1.75rem; }
.text-xl { font-size: var(--font-size-xl); line-height: 1.75rem; }
.text-2xl { font-size: var(--font-size-2xl); line-height: 2rem; }
.text-3xl { font-size: var(--font-size-3xl); line-height: 2.25rem; }
.text-4xl { font-size: var(--font-size-4xl); line-height: 2.5rem; }
.text-5xl { font-size: var(--font-size-5xl); line-height: 1; }
.text-6xl { font-size: var(--font-size-6xl); line-height: 1; }

/* Responsive Typography */
.responsive-text {
    font-size: clamp(1rem, 2.5vw, 2rem);
    line-height: 1.4;
}

.fluid-heading {
    font-size: clamp(var(--font-size-2xl), 5vw, var(--font-size-4xl));
}

/* Advanced Font Features */
.advanced-typography {
    font-feature-settings: 
        "liga" 1,      /* Ligatures */
        "kern" 1,      /* Kerning */
        "onum" 1,      /* Old-style numbers */
        "pnum" 1,      /* Proportional numbers */
        "smcp" 1;      /* Small caps */
    
    font-variant-numeric: oldstyle-nums proportional-nums;
    font-variant-ligatures: common-ligatures;
}

/* Text utilities */
.text-left { text-align: left; }
.text-center { text-align: center; }
.text-right { text-align: right; }
.text-justify { text-align: justify; }

.font-thin { font-weight: 100; }
.font-light { font-weight: var(--font-weight-light); }
.font-normal { font-weight: var(--font-weight-normal); }
.font-medium { font-weight: var(--font-weight-medium); }
.font-semibold { font-weight: var(--font-weight-semibold); }
.font-bold { font-weight: var(--font-weight-bold); }
.font-extrabold { font-weight: var(--font-weight-extrabold); }

.italic { font-style: italic; }
.not-italic { font-style: normal; }

.uppercase { text-transform: uppercase; }
.lowercase { text-transform: lowercase; }
.capitalize { text-transform: capitalize; }
.normal-case { text-transform: none; }

/* Line height utilities */
.leading-tight { line-height: var(--line-height-tight); }
.leading-normal { line-height: var(--line-height-normal); }
.leading-relaxed { line-height: var(--line-height-relaxed); }

/* Letter spacing */
.tracking-tight { letter-spacing: -0.025em; }
.tracking-normal { letter-spacing: 0; }
.tracking-wide { letter-spacing: 0.025em; }
.tracking-wider { letter-spacing: 0.05em; }
.tracking-widest { letter-spacing: 0.1em; }

/* Text decoration */
.underline { text-decoration: underline; }
.line-through { text-decoration: line-through; }
.no-underline { text-decoration: none; }

/* Advanced text effects */
.text-gradient {
    background: linear-gradient(135deg, var(--primary-500), var(--primary-600));
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.text-shadow-sm { text-shadow: 0 1px 2px rgb(0 0 0 / 0.05); }
.text-shadow { text-shadow: 0 1px 3px rgb(0 0 0 / 0.1); }
.text-shadow-lg { text-shadow: 0 15px 30px rgb(0 0 0 / 0.11); }

/* Reading optimization */
.reading-content {
    max-width: 65ch;
    line-height: var(--line-height-relaxed);
    font-size: var(--font-size-lg);
}

.reading-content h1,
.reading-content h2,
.reading-content h3 {
    max-width: 40ch;
}

/* Print typography */
@media print {
    body {
        font-family: var(--font-family-serif);
        font-size: 12pt;
        line-height: 1.5;
    }
    
    h1, h2, h3, h4, h5, h6 {
        page-break-after: avoid;
    }
    
    p, blockquote {
        orphans: 3;
        widows: 3;
    }
}
```

## 2.5 Advanced Animations and Transitions

### Keyframe Animations
```css
/* Utility animations */
@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes slideInRight {
    from {
        transform: translateX(100%);
    }
    to {
        transform: translateX(0);
    }
}

@keyframes bounce {
    0%, 100% {
        transform: translateY(-25%);
        animation-timing-function: cubic-bezier(0.8, 0, 1, 1);
    }
    50% {
        transform: translateY(0);
        animation-timing-function: cubic-bezier(0, 0, 0.2, 1);
    }
}

@keyframes pulse {
    0%, 100% {
        opacity: 1;
    }
    50% {
        opacity: 0.5;
    }
}

@keyframes spin {
    from {
        transform: rotate(0deg);
    }
    to {
        transform: rotate(360deg);
    }
}

@keyframes wiggle {
    0%, 100% { transform: rotate(-3deg); }
    50% { transform: rotate(3deg); }
}

/* Complex animations */
@keyframes morphShape {
    0% {
        border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
        transform: rotate(0deg);
    }
    25% {
        border-radius: 30% 60% 70% 40% / 50% 60% 30% 60%;
        transform: rotate(90deg);
    }
    50% {
        border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
        transform: rotate(180deg);
    }
    75% {
        border-radius: 30% 60% 70% 40% / 50% 60% 30% 60%;
        transform: rotate(270deg);
    }
    100% {
        border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
        transform: rotate(360deg);
    }
}

@keyframes typewriter {
    from { width: 0; }
    to { width: 100%; }
}

@keyframes blink {
    from, to { border-color: transparent; }
    50% { border-color: var(--primary-500); }
}

/* Animation classes */
.animate-fade-in {
    animation: fadeIn var(--duration-slow) var(--easing-ease-out);
}

.animate-fade-in-up {
    animation: fadeInUp var(--duration-slow) var(--easing-ease-out);
}

.animate-bounce {
    animation: bounce 1s infinite;
}

.animate-pulse {
    animation: pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
}

.animate-spin {
    animation: spin 1s linear infinite;
}

.animate-wiggle {
    animation: wiggle 1s ease-in-out infinite;
}

/* Hover animations */
.hover-lift {
    transition: transform var(--duration-normal) var(--easing-ease-out);
}

.hover-lift:hover {
    transform: translateY(-8px);
}

.hover-scale {
    transition: transform var(--duration-normal) var(--easing-ease-out);
}

.hover-scale:hover {
    transform: scale(1.05);
}

.hover-rotate {
    transition: transform var(--duration-normal) var(--easing-ease-out);
}

.hover-rotate:hover {
    transform: rotate(5deg);
}

/* Scroll animations */
.scroll-reveal {
    opacity: 0;
    transform: translateY(50px);
    transition: opacity 0.6s ease, transform 0.6s ease;
}

.scroll-reveal.revealed {
    opacity: 1;
    transform: translateY(0);
}

/* Loading animations */
.loading-spinner {
    width: 40px;
    height: 40px;
    border: 4px solid var(--gray-200);
    border-top: 4px solid var(--primary-500);
    border-radius: 50%;
    animation: spin 1s linear infinite;
}

.loading-dots {
    display: inline-flex;
    gap: 4px;
}

.loading-dots span {
    width: 8px;
    height: 8px;
    border-radius: 50%;
    background-color: var(--primary-500);
    animation: pulse 1.4s ease-in-out infinite both;
}

.loading-dots span:nth-child(1) { animation-delay: -0.32s; }
.loading-dots span:nth-child(2) { animation-delay: -0.16s; }

/* Performance optimization */
.gpu-accelerated {
    transform: translateZ(0);
    will-change: transform;
}

/* Reduce motion */
@media (prefers-reduced-motion: reduce) {
    .animate-bounce,
    .animate-pulse,
    .animate-spin,
    .animate-wiggle {
        animation: none;
    }
    
    .hover-lift:hover,
    .hover-scale:hover,
    .hover-rotate:hover {
        transform: none;
    }
}
```

### Advanced Transitions
```css
/* Complex transitions */
.complex-transition {
    transition: 
        background-color var(--duration-normal) var(--easing-ease-out),
        transform var(--duration-normal) var(--easing-bounce),
        box-shadow var(--duration-fast) var(--easing-ease-in-out),
        border-radius var(--duration-slow) var(--easing-ease-in);
}

/* Staggered animations */
.stagger-container .item {
    opacity: 0;
    transform: translateY(20px);
    animation: fadeInUp 0.6s forwards;
}

.stagger-container .item:nth-child(1) { animation-delay: 0.1s; }
.stagger-container .item:nth-child(2) { animation-delay: 0.2s; }
.stagger-container .item:nth-child(3) { animation-delay: 0.3s; }
.stagger-container .item:nth-child(4) { animation-delay: 0.4s; }
.stagger-container .item:nth-child(5) { animation-delay: 0.5s; }

/* Interactive animations */
.button {
    position: relative;
    overflow: hidden;
    transition: transform var(--duration-normal);
}

.button::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 0;
    height: 0;
    border-radius: 50%;
    background: rgba(255, 255, 255, 0.3);
    transform: translate(-50%, -50%);
    transition: width 0.6s, height 0.6s;
}

.button:active::before {
    width: 300px;
    height: 300px;
}
```

## 2.6 Modern CSS Features

### CSS Subgrid
```css
.main-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(3, auto);
    gap: var(--space-4);
}

.subgrid-item {
    display: grid;
    grid-column: span 2;
    grid-row: span 2;
    grid-template-columns: subgrid;
    grid-template-rows: subgrid;
    gap: inherit;
}
```

### CSS Scroll Snap
```css
.scroll-container {
    scroll-snap-type: x mandatory;
    overflow-x: auto;
    display: flex;
    gap: var(--space-4);
}

.scroll-item {
    scroll-snap-align: start;
    flex: 0 0 300px;
}

/* Scroll snap for vertical */
.vertical-scroll {
    height: 100vh;
    overflow-y: auto;
    scroll-snap-type: y mandatory;
}

.section {
    height: 100vh;
    scroll-snap-align: start;
}
```

### CSS Logical Properties
```css
.logical-layout {
    margin-block-start: var(--space-4);
    margin-block-end: var(--space-4);
    margin-inline-start: var(--space-2);
    margin-inline-end: var(--space-2);
    
    padding-block: var(--space-3);
    padding-inline: var(--space-6);
    
    border-block-start: 1px solid var(--gray-300);
    border-inline-end: 2px solid var(--primary-500);
    
    inset-block-start: 0;
    inset-inline-start: 0;
}
```

### CSS Aspect Ratio
```css
.aspect-ratio-16-9 {
    aspect-ratio: 16 / 9;
}

.aspect-ratio-square {
    aspect-ratio: 1;
}

.aspect-ratio-4-3 {
    aspect-ratio: 4 / 3;
}

/* Responsive aspect ratios */
.responsive-video {
    aspect-ratio: 16 / 9;
    width: 100%;
    object-fit: cover;
}
```

### CSS Gap Property
```css
.flex-gap {
    display: flex;
    gap: var(--space-4);
    row-gap: var(--space-2);
    column-gap: var(--space-6);
}

.grid-gap {
    display: grid;
    gap: var(--space-4) var(--space-2);
}
```

---

# 🚀 3-BO'LIM: PROFESSIONAL AMALIY LOYIHALAR

## 3.1 E-commerce Product Card
```html
<article class="product-card">
    <div class="product-image">
        <img src="product.jpg" alt="Mahsulot nomi" loading="lazy">
        <div class="product-badges">
            <span class="badge badge-sale">-20%</span>
            <span class="badge badge-new">Yangi</span>
        </div>
        <div class="product-actions">
            <button class="btn-icon" aria-label="Sevimlilar ro'yxatiga qo'shish">
                <span aria-hidden="true">♡</span>
            </button>
            <button class="btn-icon" aria-label="Tezkor ko'rish">
                <span aria-hidden="true">👁</span>
            </button>
        </div>
    </div>
    <div class="product-info">
        <h3 class="product-title">
            <a href="/products/123">Ajoyib mahsulot nomi</a>
        </h3>
        <div class="product-rating">
            <div class="stars">
                <span class="star filled" aria-hidden="true">★</span>
                <span class="star filled" aria-hidden="true">★</span>
                <span class="star filled" aria-hidden="true">★</span>
                <span class="star filled" aria-hidden="true">★</span>
                <span class="star" aria-hidden="true">★</span>
            </div>
            <span class="rating-count">(24 ta sharh)</span>
        </div>
        <div class="product-price">
            <span class="price-current">$89.99</span>
            <span class="price-original">$112.49</span>
        </div>
        <button class="btn btn-primary product-add-to-cart">
            <span aria-hidden="true">🛒</span>
            Savatga qo'shish
        </button>
    </div>
</article>
```

```css
.product-card {
    --card-padding: var(--space-4);
    --card-radius: var(--radius-lg);
    
    background: white;
    border-radius: var(--card-radius);
    box-shadow: var(--shadow-sm);
    overflow: hidden;
    transition: all var(--duration-normal);
    position: relative;
}

.product-card:hover {
    box-shadow: var(--shadow-lg);
    transform: translateY(-4px);
}

.product-image {
    position: relative;
    aspect-ratio: 4 / 3;
    overflow: hidden;
    background: var(--gray-50);
}

.product-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform var(--duration-slow);
}

.product-card:hover .product-image img {
    transform: scale(1.05);
}

.product-badges {
    position: absolute;
    top: var(--space-3);
    left: var(--space-3);
    display: flex;
    gap: var(--space-2);
    z-index: 2;
}

.badge {
    padding: var(--space-1) var(--space-2);
    border-radius: var(--radius-full);
    font-size: var(--font-size-xs);
    font-weight: var(--font-weight-semibold);
    text-transform: uppercase;
}

.badge-sale {
    background: var(--color-error);
    color: white;
}

.badge-new {
    background: var(--color-success);
    color: white;
}

.product-actions {
    position: absolute;
    top: var(--space-3);
    right: var(--space-3);
    display: flex;
    flex-direction: column;
    gap: var(--space-2);
    opacity: 0;
    transform: translateX(100%);
    transition: all var(--duration-normal);
}

.product-card:hover .product-actions {
    opacity: 1;
    transform: translateX(0);
}

.btn-icon {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background: rgba(255, 255, 255, 0.9);
    backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 255, 255, 0.2);
    display: flex;
    align-items: center;
    justify-content: center;
    transition: all var(--duration-normal);
}

.btn-icon:hover {
    background: white;
    transform: scale(1.1);
}

.product-info {
    padding: var(--card-padding);
}

.product-title {
    margin-bottom: var(--space-2);
}

.product-title a {
    color: var(--gray-900);
    text-decoration: none;
    font-weight: var(--font-weight-medium);
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 2;
    overflow: hidden;
    transition: color var(--duration-normal);
}

.product-title a:hover {
    color: var(--primary-600);
}

.product-rating {
    display: flex;
    align-items: center;
    gap: var(--space-2);
    margin-bottom: var(--space-3);
}

.stars {
    display: flex;
    gap: 2px;
}

.star {
    color: var(--gray-300);
    font-size: var(--font-size-sm);
}

.star.filled {
    color: #fbbf24;
}

.rating-count {
    font-size: var(--font-size-sm);
    color: var(--gray-500);
}

.product-price {
    display: flex;
    align-items: center;
    gap: var(--space-2);
    margin-bottom: var(--space-4);
}

.price-current {
    font-size: var(--font-size-xl);
    font-weight: var(--font-weight-bold);
    color: var(--primary-600);
}

.price-original {
    font-size: var(--font-size-base);
    color: var(--gray-400);
    text-decoration: line-through;
}

.product-add-to-cart {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: var(--space-2);
    padding: var(--space-3) var(--space-4);
    font-weight: var(--font-weight-medium);
    border-radius: var(--radius-base);
    transition: all var(--duration-normal);
}

.btn {
    border: none;
    cursor: pointer;
    text-decoration: none;
    display: inline-flex;
    align-items: center;
    justify-content: center;
    font-family: inherit;
    transition: all var(--duration-normal);
}

.btn-primary {
    background: var(--primary-500);
    color: white;
}

.btn-primary:hover {
    background: var(--primary-600);
    transform: translateY(-1px);
}

.btn-primary:active {
    transform: translateY(0);
}
```

## 3.2 Modern Navigation Menu
```html
<nav class="main-navigation" role="navigation" aria-label="Asosiy navigatsiya">
    <div class="nav-container">
        <!-- Logo -->
        <div class="nav-brand">
            <a href="/" aria-label="Bosh sahifaga qaytish">
                <img src="logo.svg" alt="Kompaniya logotipi" width="120" height="40">
            </a>
        </div>

        <!-- Desktop Navigation -->
        <div class="nav-menu" id="nav-menu">
            <ul class="nav-list">
                <li class="nav-item">
                    <a href="/" class="nav-link" aria-current="page">Bosh sahifa</a>
                </li>
                <li class="nav-item nav-item-dropdown">
                    <button class="nav-link nav-dropdown-toggle" aria-expanded="false" aria-haspopup="true">
                        Mahsulotlar
                        <span class="dropdown-icon" aria-hidden="true">▼</span>
                    </button>
                    <div class="nav-dropdown">
                        <div class="dropdown-content">
                            <div class="dropdown-section">
                                <h3 class="dropdown-title">Kategoriyalar</h3>
                                <ul class="dropdown-list">
                                    <li><a href="/laptops" class="dropdown-link">Noutbuklar</a></li>
                                    <li><a href="/phones" class="dropdown-link">Telefonlar</a></li>
                                    <li><a href="/tablets" class="dropdown-link">Planshetlar</a></li>
                                </ul>
                            </div>
                            <div class="dropdown-section">
                                <h3 class="dropdown-title">Brendlar</h3>
                                <ul class="dropdown-list">
                                    <li><a href="/apple" class="dropdown-link">Apple</a></li>
                                    <li><a href="/samsung" class="dropdown-link">Samsung</a></li>
                                    <li><a href="/xiaomi" class="dropdown-link">Xiaomi</a></li>
                                </ul>
                            </div>
                            <div class="dropdown-featured">
                                <img src="featured-product.jpg" alt="Tavsiya etilgan mahsulot">
                                <div class="featured-content">
                                    <h4>Yangi iPhone 15</h4>
                                    <p>Eng so'nggi texnologiya bilan</p>
                                    <a href="/iphone-15" class="btn btn-small">Ko'rish</a>
                                </div>
                            </div>
                        </div>
                    </div>
                </li>
                <li class="nav-item">
                    <a href="/about" class="nav-link">Biz haqimizda</a>
                </li>
                <li class="nav-item">
                    <a href="/contact" class="nav-link">Aloqa</a>
                </li>
            </ul>
        </div>

        <!-- Navigation Actions -->
        <div class="nav-actions">
            <button class="nav-search-toggle" aria-label="Qidiruvni ochish">
                <span aria-hidden="true">🔍</span>
            </button>
            <a href="/cart" class="nav-cart" aria-label="Savatni ko'rish">
                <span aria-hidden="true">🛒</span>
                <span class="cart-count">3</span>
            </a>
            <button class="nav-profile-toggle" aria-label="Profil menyusini ochish">
                <img src="avatar.jpg" alt="Foydalanuvchi avatari" class="profile-avatar">
            </button>
        </div>

        <!-- Mobile Menu Toggle -->
        <button class="mobile-menu-toggle" aria-expanded="false" aria-controls="nav-menu" aria-label="Menyuni ochish">
            <span class="hamburger-line"></span>
            <span class="hamburger-line"></span>
            <span class="hamburger-line"></span>
        </button>
    </div>

    <!-- Search Overlay -->
    <div class="search-overlay" id="search-overlay">
        <div class="search-container">
            <form class="search-form" role="search">
                <input 
                    type="search" 
                    placeholder="Mahsulot qidirish..."
                    class="search-input"
                    aria-label="Qidiruv so'zi"
                    autocomplete="off"
                >
                <button type="submit" class="search-submit" aria-label="Qidirish">
                    <span aria-hidden="true">🔍</span>
                </button>
            </form>
            <button class="search-close" aria-label="Qidiruvni yopish">
                <span aria-hidden="true">×</span>
            </button>
        </div>
        <div class="search-suggestions">
            <h3>Mashhur qidiruvlar</h3>
            <ul>
                <li><a href="/search?q=iphone">iPhone</a></li>
                <li><a href="/search?q=laptop">Laptop</a></li>
                <li><a href="/search?q=samsung">Samsung</a></li>
            </ul>
        </div>
    </div>
</nav>
```

```css
.main-navigation {
    position: sticky;
    top: 0;
    z-index: var(--z-sticky);
    background: rgba(255, 255, 255, 0.95);
    backdrop-filter: blur(10px);
    border-bottom: 1px solid var(--gray-200);
    transition: all var(--duration-normal);
}

.nav-container {
    max-width: var(--container-xl);
    margin: 0 auto;
    padding: 0 var(--space-4);
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 70px;
}

.nav-brand img {
    height: 40px;
    width: auto;
}

.nav-menu {
    display: flex;
    flex: 1;
    justify-content: center;
    margin: 0 var(--space-8);
}

.nav-list {
    display: flex;
    align-items: center;
    gap: var(--space-8);
    list-style: none;
}

.nav-link {
    color: var(--gray-700);
    text-decoration: none;
    font-weight: var(--font-weight-medium);
    padding: var(--space-2) 0;
    position: relative;
    transition: color var(--duration-normal);
    display: flex;
    align-items: center;
    gap: var(--space-1);
}

.nav-link[aria-current="page"] {
    color: var(--primary-600);
}

.nav-link::after {
    content: '';
    position: absolute;
    bottom: -8px;
    left: 0;
    width: 0;
    height: 2px;
    background: var(--primary-500);
    transition: width var(--duration-normal);
}

.nav-link:hover::after,
.nav-link[aria-current="page"]::after {
    width: 100%;
}

/* Dropdown */
.nav-item-dropdown {
    position: relative;
}

.nav-dropdown-toggle {
    background: none;
    border: none;
    cursor: pointer;
    font: inherit;
}

.dropdown-icon {
    font-size: 0.8em;
    transition: transform var(--duration-normal);
}

.nav-dropdown-toggle[aria-expanded="true"] .dropdown-icon {
    transform: rotate(180deg);
}

.nav-dropdown {
    position: absolute;
    top: 100%;
    left: 50%;
    transform: translateX(-50%);
    width: 600px;
    background: white;
    border-radius: var(--radius-lg);
    box-shadow: var(--shadow-xl);
    padding: var(--space-6);
    opacity: 0;
    visibility: hidden;
    transform: translateX(-50%) translateY(-10px);
    transition: all var(--duration-normal);
    margin-top: var(--space-4);
}

.nav-item-dropdown:hover .nav-dropdown,
.nav-dropdown-toggle[aria-expanded="true"] + .nav-dropdown {
    opacity: 1;
    visibility: visible;
    transform: translateX(-50%) translateY(0);
}

.dropdown-content {
    display: grid;
    grid-template-columns: 1fr 1fr auto;
    gap: var(--space-6);
}

.dropdown-section h3 {
    font-size: var(--font-size-sm);
    font-weight: var(--font-weight-semibold);
    text-transform: uppercase;
    color: var(--gray-500);
    margin-bottom: var(--space-3);
    letter-spacing: 0.05em;
}

.dropdown-list {
    list-style: none;
}

.dropdown-link {
    display: block;
    padding: var(--space-2) 0;
    color: var(--gray-700);
    text-decoration: none;
    transition: color var(--duration-normal);
}

.dropdown-link:hover {
    color: var(--primary-600);
}

.dropdown-featured {
    width: 200px;
    background: var(--gray-50);
    border-radius: var(--radius-base);
    padding: var(--space-4);
    text-align: center;
}

.dropdown-featured img {
    width: 100%;
    height: 80px;
    object-fit: cover;
    border-radius: var(--radius-base);
    margin-bottom: var(--space-3);
}

.featured-content h4 {
    margin-bottom: var(--space-2);
    font-size: var(--font-size-base);
}

.featured-content p {
    font-size: var(--font-size-sm);
    color: var(--gray-600);
    margin-bottom: var(--space-3);
}

/* Navigation Actions */
.nav-actions {
    display: flex;
    align-items: center;
    gap: var(--space-4);
}

.nav-search-toggle,
.nav-profile-toggle {
    background: none;
    border: none;
    cursor: pointer;
    padding: var(--space-2);
    border-radius: var(--radius-base);
    transition: background-color var(--duration-normal);
}

.nav-search-toggle:hover,
.nav-profile-toggle:hover {
    background: var(--gray-100);
}

.nav-cart {
    position: relative;
    padding: var(--space-2);
    border-radius: var(--radius-base);
    text-decoration: none;
    transition: background-color var(--duration-normal);
}

.nav-cart:hover {
    background: var(--gray-100);
}

.cart-count {
    position: absolute;
    top: 0;
    right: 0;
    background: var(--color-error);
    color: white;
    font-size: var(--font-size-xs);
    font-weight: var(--font-weight-bold);
    padding: 2px 6px;
    border-radius: var(--radius-full);
    min-width: 18px;
    height: 18px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.profile-avatar {
    width: 32px;
    height: 32px;
    border-radius: 50%;
    object-fit: cover;
}

/* Mobile Menu */
.mobile-menu-toggle {
    display: none;
    flex-direction: column;
    justify-content: space-around;
    width: 24px;
    height: 18px;
    background: none;
    border: none;
    cursor: pointer;
    padding: 0;
}

.hamburger-line {
    width: 100%;
    height: 2px;
    background: var(--gray-700);
    transition: all var(--duration-normal);
}

.mobile-menu-toggle[aria-expanded="true"] .hamburger-line:nth-child(1) {
    transform: rotate(45deg) translate(6px, 6px);
}

.mobile-menu-toggle[aria-expanded="true"] .hamburger-line:nth-child(2) {
    opacity: 0;
}

.mobile-menu-toggle[aria-expanded="true"] .hamburger-line:nth-child(3) {
    transform: rotate(-45deg) translate(6px, -6px);
}

/* Search Overlay */
.search-overlay {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(0, 0, 0, 0.8);
    z-index: var(--z-modal);
    opacity: 0;
    visibility: hidden;
    transition: all var(--duration-normal);
}

.search-overlay.active {
    opacity: 1;
    visibility: visible;
}

.search-container {
    max-width: 600px;
    margin: 100px auto 0;
    padding: 0 var(--space-4);
    position: relative;
}

.search-form {
    display: flex;
    background: white;
    border-radius: var(--radius-lg);
    box-shadow: var(--shadow-2xl);
    overflow: hidden;
}

.search-input {
    flex: 1;
    padding: var(--space-4);
    border: none;
    font-size: var(--font-size-lg);
    outline: none;
}

.search-submit {
    padding: var(--space-4);
    background: var(--primary-500);
    color: white;
    border: none;
    cursor: pointer;
    transition: background-color var(--duration-normal);
}

.search-submit:hover {
    background: var(--primary-600);
}

.search-close {
    position: absolute;
    top: -50px;
    right: 0;
    background: none;
    border: none;
    color: white;
    font-size: var(--font-size-2xl);
    cursor: pointer;
    padding: var(--space-2);
}

.search-suggestions {
    background: white;
    margin-top: var(--space-4);
    padding: var(--space-4);
    border-radius: var(--radius-lg);
    box-shadow: var(--shadow-lg);
}

.search-suggestions h3 {
    margin-bottom: var(--space-3);
    color: var(--gray-700);
}

.search-suggestions ul {
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    gap: var(--space-2);
}

.search-suggestions a {
    padding: var(--space-2) var(--space-3);
    background: var(--gray-100);
    border-radius: var(--radius-full);
    text-decoration: none;
    color: var(--gray-700);
    font-size: var(--font-size-sm);
    transition: all var(--duration-normal);
}

.search-suggestions a:hover {
    background: var(--primary-100);
    color: var(--primary-700);
}

/* Responsive Design */
@media (max-width: 768px) {
    .mobile-menu-toggle {
        display: flex;
    }

    .nav-menu {
        position: fixed;
        top: 70px;
        left: 0;
        right: 0;
        bottom: 0;
        background: white;
        transform: translateX(-100%);
        transition: transform var(--duration-normal);
        padding: var(--space-4);
        overflow-y: auto;
    }

    .nav-menu.active {
        transform: translateX(0);
    }

    .nav-list {
        flex-direction: column;
        align-items: stretch;
        gap: 0;
    }

    .nav-item {
        border-bottom: 1px solid var(--gray-200);
    }

    .nav-link {
        padding: var(--space-4) 0;
        justify-content: space-between;
    }

    .nav-dropdown {
        position: static;
        transform: none;
        width: 100%;
        box-shadow: none;
        background: var(--gray-50);
        margin: 0;
        max-height: 0;
        overflow: hidden;
        padding: 0 var(--space-4);
        transition: all var(--duration-normal);
    }

    .nav-dropdown-toggle[aria-expanded="true"] + .nav-dropdown {
        max-height: 500px;
        padding: var(--space-4);
    }

    .dropdown-content {
        grid-template-columns: 1fr;
        gap: var(--space-4);
    }

    .dropdown-featured {
        width: 100%;
    }

    .nav-actions {
        gap: var(--space-2);
    }

    .search-container {
        margin-top: 50px;
    }
}

@media (max-width: 480px) {
    .nav-container {
        padding: 0 var(--space-3);
    }

    .nav-actions {
        gap: var(--space-1);
    }
}
```

## 3.3 Advanced Modal System
```html
<!-- Modal Trigger -->
<button class="btn btn-primary" data-modal-target="example-modal">
    Modalni ochish
</button>

<!-- Modal Structure -->
<div class="modal-overlay" id="example-modal" role="dialog" aria-modal="true" aria-labelledby="modal-title" aria-hidden="true">
    <div class="modal-container">
        <div class="modal-content">
            <!-- Modal Header -->
            <header class="modal-header">
                <h2 id="modal-title" class="modal-title">Modal sarlavhasi</h2>
                <button class="modal-close" aria-label="Modalni yopish" data-modal-close>
                    <span aria-hidden="true">&times;</span>
                </button>
            </header>

            <!-- Modal Body -->
            <div class="modal-body">
                <p>Bu modal oyna tarkibi. Bu yerda har qanday HTML kontent bo'lishi mumkin.</p>
                
                <form class="modal-form">
                    <div class="form-group">
                        <label for="modal-name">Ismingiz</label>
                        <input type="text" id="modal-name" name="name" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="modal-email">Email</label>
                        <input type="email" id="modal-email" name="email" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="modal-message">Xabar</label>
                        <textarea id="modal-message" name="message" rows="4"></textarea>
                    </div>
                </form>
            </div>

            <!-- Modal Footer -->
            <footer class="modal-footer">
                <button class="btn btn-primary">Saqlash</button>
                <button class="btn btn-secondary" data-modal-close>Bekor qilish</button>
            </footer>
        </div>
    </div>
</div>

<!-- Different Modal Types -->
<!-- Confirmation Modal -->
<div class="modal-overlay modal-confirm" id="confirm-modal" role="dialog" aria-modal="true">
    <div class="modal-container modal-sm">
        <div class="modal-content">
            <div class="modal-icon">
                <span class="icon-warning">⚠️</span>
            </div>
            <h3 class="modal-title">Tasdiqlash</h3>
            <p class="modal-message">Ushbu amalni bajarishni xohlaysizmi?</p>
            <div class="modal-actions">
                <button class="btn btn-danger">Ha, davom etish</button>
                <button class="btn btn-secondary" data-modal-close>Yo'q</button>
            </div>
        </div>
    </div>
</div>

<!-- Image Modal -->
<div class="modal-overlay modal-image" id="image-modal" role="dialog" aria-modal="true">
    <div class="modal-container modal-image-container">
        <button class="modal-close modal-close-image" aria-label="Rasmni yopish" data-modal-close>
            <span aria-hidden="true">&times;</span>
        </button>
        <img src="" alt="" class="modal-image-content">
        <div class="modal-image-info">
            <h3 class="image-title"></h3>
            <p class="image-description"></p>
        </div>
    </div>
</div>
```

```css
/* Modal Base Styles */
.modal-overlay {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(0, 0, 0, 0.6);
    z-index: var(--z-modal);
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    visibility: hidden;
    transition: all var(--duration-normal);
    backdrop-filter: blur(4px);
}

.modal-overlay.active {
    opacity: 1;
    visibility: visible;
}

.modal-container {
    max-width: 90vw;
    max-height: 90vh;
    width: 100%;
    margin: var(--space-4);
    transform: scale(0.8) translateY(50px);
    transition: transform var(--duration-normal);
}

.modal-overlay.active .modal-container {
    transform: scale(1) translateY(0);
}

.modal-content {
    background: white;
    border-radius: var(--radius-lg);
    box-shadow: var(--shadow-2xl);
    max-height: 90vh;
    overflow: auto;
    position: relative;
}

/* Modal Sizes */
.modal-sm { max-width: 400px; }
.modal-md { max-width: 600px; }
.modal-lg { max-width: 800px; }
.modal-xl { max-width: 1200px; }
.modal-full { 
    max-width: 95vw;
    max-height: 95vh;
}

/* Modal Header */
.modal-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: var(--space-6) var(--space-6) 0;
    border-bottom: 1px solid var(--gray-200);
    padding-bottom: var(--space-4);
    margin-bottom: var(--space-6);
}

.modal-title {
    font-size: var(--font-size-xl);
    font-weight: var(--font-weight-semibold);
    color: var(--gray-900);
    margin: 0;
}

.modal-close {
    background: none;
    border: none;
    font-size: var(--font-size-2xl);
    color: var(--gray-400);
    cursor: pointer;
    padding: var(--space-1);
    border-radius: var(--radius-base);
    transition: all var(--duration-normal);
    line-height: 1;
    width: 32px;
    height: 32px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.modal-close:hover {
    background: var(--gray-100);
    color: var(--gray-600);
    transform: scale(1.1);
}

/* Modal Body */
.modal-body {
    padding: 0 var(--space-6);
    color: var(--gray-700);
    line-height: var(--line-height-relaxed);
}

.modal-form .form-group {
    margin-bottom: var(--space-4);
}

.modal-form label {
    display: block;
    margin-bottom: var(--space-2);
    font-weight: var(--font-weight-medium);
    color: var(--gray-700);
}

.modal-form input,
.modal-form textarea {
    width: 100%;
    padding: var(--space-3);
    border: 1px solid var(--gray-300);
    border-radius: var(--radius-base);
    font-family: inherit;
    font-size: var(--font-size-base);
    transition: border-color var(--duration-normal);
}

.modal-form input:focus,
.modal-form textarea:focus {
    outline: none;
    border-color: var(--primary-500);
    box-shadow: 0 0 0 3px var(--primary-100);
}

/* Modal Footer */
.modal-footer {
    display: flex;
    justify-content: flex-end;
    gap: var(--space-3);
    padding: var(--space-6);
    border-top: 1px solid var(--gray-200);
    margin-top: var(--space-6);
    padding-top: var(--space-4);
}

/* Confirmation Modal */
.modal-confirm .modal-content {
    text-align: center;
    padding: var(--space-8) var(--space-6);
}

.modal-icon {
    margin-bottom: var(--space-4);
    font-size: var(--font-size-5xl);
}

.modal-confirm .modal-title {
    margin-bottom: var(--space-4);
    font-size: var(--font-size-xl);
}

.modal-message {
    margin-bottom: var(--space-6);
    color: var(--gray-600);
    font-size: var(--font-size-lg);
}

.modal-actions {
    display: flex;
    justify-content: center;
    gap: var(--space-3);
}

/* Image Modal */
.modal-image {
    background: rgba(0, 0, 0, 0.9);
}

.modal-image-container {
    max-width: 95vw;
    max-height: 95vh;
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.modal-close-image {
    position: absolute;
    top: -50px;
    right: -50px;
    background: rgba(255, 255, 255, 0.9);
    color: var(--gray-900);
    z-index: 1;
}

.modal-image-content {
    max-width: 100%;
    max-height: 80vh;
    object-fit: contain;
    border-radius: var(--radius-base);
}

.modal-image-info {
    background: white;
    padding: var(--space-4);
    border-radius: var(--radius-base);
    margin-top: var(--space-4);
    text-align: center;
    max-width: 500px;
}

.image-title {
    margin-bottom: var(--space-2);
    font-size: var(--font-size-lg);
    font-weight: var(--font-weight-semibold);
}

.image-description {
    color: var(--gray-600);
    margin: 0;
}

/* Animation Classes */
.modal-fade-in {
    animation: modalFadeIn var(--duration-slow) var(--easing-ease-out);
}

@keyframes modalFadeIn {
    from {
        opacity: 0;
        transform: scale(0.8) translateY(50px);
    }
    to {
        opacity: 1;
        transform: scale(1) translateY(0);
    }
}

.modal-slide-up {
    animation: modalSlideUp var(--duration-slow) var(--easing-ease-out);
}

@keyframes modalSlideUp {
    from {
        transform: translateY(100%);
    }
    to {
        transform: translateY(0);
    }
}

/* Responsive */
@media (max-width: 768px) {
    .modal-container {
        margin: var(--space-2);
        max-height: 95vh;
    }
    
    .modal-header,
    .modal-body,
    .modal-footer {
        padding-left: var(--space-4);
        padding-right: var(--space-4);
    }
    
    .modal-footer {
        flex-direction: column-reverse;
        gap: var(--space-2);
    }
    
    .modal-footer .btn {
        width: 100%;
    }
    
    .modal-actions {
        flex-direction: column;
    }
    
    .modal-actions .
    