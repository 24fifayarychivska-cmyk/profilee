# Style Guide - Social Links Profile

## 🎨 Кольорова схема

### Основні кольори

```css
--clr-bg: #0f1419;                    /* Фон сторінки */
--clr-card-bg: #1a1f2e;               /* Фон карточки */
--clr-text-primary: #ffffff;          /* Основний текст */
--clr-text-secondary: #c4c9db;        /* Вторинний текст */
```

### Акцентні кольори

```css
--clr-accent-green: #00d084;          /* Зелений (основний) */
--clr-accent-purple: #7d5aed;         /* Фіолетовий */
--clr-accent-red: #ff5757;            /* Червоний */
--clr-accent-yellow: #fcd34d;         /* Жовтий */
--clr-accent-blue: #3b82f6;           /* Синій */
--clr-focus: #00d084;                 /* Колір для focus стану */
--clr-hover-overlay: rgba(0, 208, 132, 0.1);  /* Overlay при hover */
```

### Соціальні мережі (Брендові кольори)

| Платформа | Колір | Hex |
|-----------|-------|-----|
| Facebook  | Синій | #1877F2 |
| Twitter/X | Синій | #1DA1F2 |
| Instagram | Градієнт Рожевий | #E4405F → #f09433 → #e6683c → #dc2743 → #cc2366 → #bc1888 |
| LinkedIn  | Синій | #0A66C2 |
| GitHub    | Сірий | #333333 |

### Light Mode (автоматичні при prefers-color-scheme: light)

```css
--clr-bg: #f8f9fa;                    /* Світлий фон */
--clr-card-bg: #ffffff;               /* Біла карточка */
--clr-text-primary: #1a1f2e;          /* Темний текст */
--clr-text-secondary: #666778;        /* Сірий текст */
```

## 🔤 Типографія

### Шрифт

```css
--ff-primary: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
```

**Основний шрифт**: Inter (з fallbacks на системні шрифти)

### Розміри шрифтів

```css
--fs-sm: 0.875rem;      /* 14px - Малий (labels, small text) */
--fs-base: 1rem;        /* 16px - Стандартний */
--fs-lg: 1.25rem;       /* 20px - Великий */
--fs-xl: 1.5rem;        /* 24px - Дуже великий (статистика) */
--fs-2xl: 2rem;         /* 32px - Заголовок профілю */
```

### Ваги шрифтів

```css
--fw-regular: 400;      /* Звичайний текст */
--fw-medium: 500;       /* Посилені labels */
--fw-semibold: 600;     /* Títиньки розділів */
--fw-bold: 700;         /* Профільне ім'я, заголовки */
```

## 📐 Інтервали (Spacing)

```css
--spacing-xs: 0.25rem;  /* 4px */
--spacing-sm: 0.5rem;   /* 8px */
--spacing-md: 1rem;     /* 16px */
--spacing-lg: 1.5rem;   /* 24px */
--spacing-xl: 2rem;     /* 32px */
--spacing-2xl: 3rem;    /* 48px */
```

## 🎯 Скруглення кутів (Border Radius)

```css
--br-sm: 0.375rem;      /* 6px - Малі елементи */
--br-md: 0.5rem;        /* 8px - Кнопки, інпути */
--br-lg: 1rem;          /* 16px - Карточка */
--br-full: 9999px;      /* Повністю круглі елементи (badges) */
```

## 💫 Тіні (Shadows)

```css
--shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.05);       /* Легка тінь */
--shadow-md: 0 4px 6px rgba(0, 0, 0, 0.1);       /* Середня тінь */
--shadow-lg: 0 10px 15px rgba(0, 0, 0, 0.3);     /* Велика тінь (карточка) */
```

## ⏱️ Переходи (Transitions)

```css
--transition-fast: 150ms ease-in-out;     /* Швидкі ефекти (hover) */
--transition-base: 250ms ease-in-out;     /* Стандартна тривалість */
--transition-slow: 350ms ease-in-out;     /* Повільні анімації */
```

## 🎬 Анімації

### slideIn
Анімація при завантаженні сторінки для профільної карточки:
- **Тривалість**: 0.6s
- **Timing**: ease-out
- **Початок**: Прозорість 0%, зсув вниз на 20px
- **Кінець**: Прозорість 100%, нормальна позиція

## 🎮 Компоненти

### Профільна карточка
- **Фон**: Градієнт `linear-gradient(135deg, var(--clr-card-bg) 0%, rgba(125, 90, 237, 0.1) 100%)`
- **Padding**: 3rem 2rem (desktop), 2rem 1rem (mobile)
- **Border-radius**: 1rem
- **Тінь**: var(--shadow-lg)
- **Бордер**: 1px solid rgba(125, 90, 237, 0.2)

### Аватар
- **Розмір**: 100px × 100px (desktop), 80px × 80px (mobile)
- **Border-radius**: 50% (повний круг)
- **Фон**: Градієнт `linear-gradient(135deg, var(--clr-accent-purple), var(--clr-accent-green))`
- **Тінь**: 0 0 30px rgba(0, 208, 132, 0.3)
- **Hover**: scale(1.05)

### Соціальні кнопки
- **Padding**: 1.5rem
- **Border**: 2px solid
- **Border-radius**: 0.5rem
- **Hover ефекти**:
  - Піднятто: translateY(-4px)
  - Колір: Змінюється на брендовий
  - Тінь: 0 10px 20px rgba(color, 0.3)
  - Letter-spacing: +0.5px
- **Focus**: 3px solid outline
- **Active**: translateY(-2px)

### Акційні кнопки
- **Padding**: 1rem 1.5rem
- **Border**: 2px solid var(--clr-accent-green)
- **Border-radius**: 0.5rem
- **Font-weight**: 600
- **Text-transform**: uppercase
- **Letter-spacing**: 0.5px

**Первинна кнопка (.btn-primary)**:
- **Фон**: var(--clr-accent-green)
- **Колір**: var(--clr-bg)

**Вторинна кнопка (.btn-secondary)**:
- **Фон**: transparent
- **Колір**: var(--clr-accent-green)
- **Hover**: Фон змінюється на зелений, колір на чорний

### Статистика
- **Grid**: 3 колони
- **Gap**: 1rem
- **Фон**: rgba(0, 0, 0, 0.3)
- **Padding**: 1.5rem
- **Border-radius**: 0.5rem
- **Бордер**: 1px solid rgba(0, 208, 132, 0.1)

### Skill Badges
- **Padding**: 0.5rem 1.5rem
- **Border-radius**: 9999px (повний круг)
- **Фон**: rgba(0, 208, 132, 0.15)
- **Колір**: var(--clr-accent-green)
- **Бордер**: 1px solid rgba(0, 208, 132, 0.3)
- **Hover**: 
  - Фон: rgba(0, 208, 132, 0.25)
  - Піднятто: translateY(-2px)
  - Тінь: 0 4px 12px rgba(0, 208, 132, 0.2)

## 📱 Брейкпойнти

```css
/* Desktop (за замовчуванням) */
max-width: 600px для контейнера

/* Mobile (max-width: 480px) */
- Аватар: 80px (з 100px)
- Профільне ім'я: 1.5rem (з 2rem)
- Соціальні кнопки: 2 колони (з auto-fit)
- Акційні кнопки: flex-direction column
```

## ♿ Доступність

### Focus Stany
- **Outline**: 3px solid var(--clr-accent-green)
- **Outline-offset**: 2px
- **Видимість**: Всі інтерактивні елементи мають видимий focus

### ARIA labels
- Профільна карточка: `role="region" aria-label="User profile"`
- Аватар: `role="img" aria-label="Alina Yarychivska profile picture"`
- Соціальні посилання: `aria-label` для кожної платформи
- Кнопки: `aria-label` описує дію

### Skip Link
- Позиція: абсолютна, top: -40px
- На фокусі: top: 0
- Фон: var(--clr-accent-green)
- Дозволяє користувачам пропустити навігацію

### prefers-reduced-motion
Всі анімації та переходи мають `duration: 0.01ms` при увімкненому reduced-motion

## 🎨 Рекомендації

1. **Консистентність**: Использовать CSS змінні з :root для простоти змін
2. **Контраст**: Всі текстові елементи мають контраст не менше 4.5:1
3. **Інтерактивність**: Hover та focus стани мають бути видимими й інтуїтивними
4. **Адаптивність**: Тестувати на мобільних пристроях
5. **Доступність**: Тестувати з клавіатурою та скрін-рідерами

## 📋 Контрольний список для розробки

- [x] Кольорова схема
- [x] Типографія
- [x] Інтервали
- [x] Скруглення
- [x] Тіні
- [x] Переходи
- [x] Анімації
- [x] Компоненти
- [x] Адаптивність
- [x] Доступність
