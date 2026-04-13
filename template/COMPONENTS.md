# 🎨 Библиотека компонентов для презентаций

Готовые к использованию компоненты для быстрого создания профессиональных слайдов.

## 📦 Основные компоненты

### 1. Badge (Значок слайда)
**Использование**: Указание номера этапа или темы

```html
<div class="badge animate-on-view">
    <span class="badge-dot"></span>
    Этап 1
</div>
```

**Варианты**:
- С пульсирующей точкой (по умолчанию)
- Текст: Этап, Тема, Раздел, Информация

---

### 2. Glass Card (Стеклянная карточка)
**Использование**: Основной контейнер для информации

```html
<div class="glass-card accent">
    <div class="icon-circle">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
            <circle cx="12" cy="12" r="10"></circle>
            <path d="M12 6v6l4 2"></path>
        </svg>
    </div>
    <h4>Заголовок карточки</h4>
    <p>Описание или основная информация</p>
    <ul class="styled-list">
        <li>Пункт 1</li>
        <li>Пункт 2</li>
        <li>Пункт 3</li>
    </ul>
</div>
```

**Модификаторы**:
- `.glass-card` - базовая карточка
- `.glass-card.accent` - с цветной полоской сверху (при hover)

---

### 3. Иконка в круге
**Использование**: Визуальный элемент для карточек

```html
<div class="icon-circle">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
        <!-- SVG path здесь -->
    </svg>
</div>
```

**Рекомендуемые размеры SVG**: viewBox="0 0 24 24"

---

### 4. Сетка компонентов

#### Grid 2 (двухколонка)
```html
<div class="grid-2">
    <div class="glass-card">Колонка 1</div>
    <div class="glass-card">Колонка 2</div>
</div>
```

**Особенности**:
- Автоматически адаптируется на мобильных
- Минимальная ширина: 280px на элемент

#### Grid 3 (трехколонка)
```html
<div class="grid-3">
    <div class="stat-card">Элемент 1</div>
    <div class="stat-card">Элемент 2</div>
    <div class="stat-card">Элемент 3</div>
</div>
```

**Особенности**:
- Идеальна для статистики
- Минимальная ширина: 250px

#### Grid 4 (четырехколонка)
```html
<div class="grid-4">
    <div class="glass-card">Шаг 1</div>
    <div class="glass-card">Шаг 2</div>
    <div class="glass-card">Шаг 3</div>
    <div class="glass-card">Шаг 4</div>
</div>
```

---

### 5. Styled List (Стилизованный список)
**Использование**: Маркированные списки с стрелками

```html
<ul class="styled-list">
    <li>Первый пункт</li>
    <li>Второй пункт</li>
    <li>Третий пункт</li>
</ul>
```

**Особенности**:
- Стрелка (→) вместо точки
- Оптимальное расстояние между элементами
- Автоматическое масштабирование

---

### 6. Stat Card (Карточка статистики)
**Использование**: Отображение чисел и KPI

```html
<div class="stat-card">
    <div class="stat-number">99%</div>
    <div class="stat-label">Эффективность</div>
</div>
```

**Вариант с трёмя карточками**:
```html
<div class="grid-3">
    <div class="stat-card">
        <div class="stat-number">2023</div>
        <div class="stat-label">Год основания</div>
    </div>
    <div class="stat-card">
        <div class="stat-number">500+</div>
        <div class="stat-label">Студентов</div>
    </div>
    <div class="stat-card">
        <div class="stat-number">100%</div>
        <div class="stat-label">Качество</div>
    </div>
</div>
```

---

### 7. Process Flow (Процесс)
**Использование**: Показ этапов или последовательности

```html
<div class="process-flow">
    <div class="process-step">
        <div class="step-icon">1</div>
        <div class="step-label">Выбор темы</div>
    </div>
    <div class="process-arrow">→</div>
    <div class="process-step">
        <div class="step-icon">2</div>
        <div class="step-label">Анализ</div>
    </div>
    <div class="process-arrow">→</div>
    <div class="process-step">
        <div class="step-icon">3</div>
        <div class="step-label">Написание</div>
    </div>
    <div class="process-arrow">→</div>
    <div class="process-step">
        <div class="step-icon">4</div>
        <div class="step-label">Завершение</div>
    </div>
</div>
```

---

### 8. Key Point (Ключевой момент)
**Использование**: Выделение важной информации

```html
<div class="key-point">
    <div class="key-point-icon">💡</div>
    <div class="key-point-content">
        <h4>Совет</h4>
        <p>Начните подготовку за несколько недель до срока</p>
    </div>
</div>
```

**Варианты иконок**:
- 💡 - Совет/Идея
- ⚠️ - Предупреждение
- ✨ - Особенность
- ⏱️ - Время
- 🎯 - Цель

---

### 9. Author Card (Карточка автора)
**Использование**: Отображение информации об авторах

```html
<div class="author-card">
    <div class="author-avatar">А</div>
    <div class="author-name">Актанов Д.</div>
</div>
```

**В сетке авторов**:
```html
<div class="authors-grid stagger">
    <div class="author-card animate-on-view">
        <div class="author-avatar">А</div>
        <div class="author-name">Актанов Д.</div>
    </div>
    <div class="author-card animate-on-view">
        <div class="author-avatar">А</div>
        <div class="author-name">Ашенов К.</div>
    </div>
    <div class="author-card animate-on-view">
        <div class="author-avatar">Т</div>
        <div class="author-name">Тарасов С.</div>
    </div>
</div>
```

---

### 10. Group Badge (Групповой значок)
**Использование**: Показ группы и организации

```html
<div class="group-badge">
    <span>ИМ-32</span>
    <span>•</span>
    <span>Margulan University</span>
</div>
```

---

### 11. Divider (Разделитель)
**Использование**: Визуальное разделение контента

```html
<hr class="divider">
```

---

### 12. Animations (Анимации)

#### Появление при прокрутке
```html
<div class="animate-on-view">
    Этот элемент появится при прокрутке
</div>
```

#### Каскадная анимация
```html
<div class="stagger">
    <div class="animate-on-view">Первый элемент</div>
    <div class="animate-on-view">Второй элемент</div>
    <div class="animate-on-view">Третий элемент</div>
</div>
```

---

## 🎯 Примеры полных слайдов

### Слайд 1: Вводный
```html
<section id="slide-1">
    <div class="slide-content title-slide">
        <div class="badge animate-on-view">
            <span class="badge-dot"></span>
            Образование
        </div>
        <h1 class="animate-on-view">Заголовок презентации</h1>
        <p class="title-subtitle animate-on-view">Подзаголовок с кратким описанием</p>
        
        <hr class="divider animate-on-view">

        <div class="authors-grid stagger">
            <div class="author-card animate-on-view">
                <div class="author-avatar">А</div>
                <div class="author-name">Автор 1</div>
            </div>
        </div>

        <div class="group-badge animate-on-view">
            <span>Группа</span>
            <span>•</span>
            <span>Организация</span>
        </div>
    </div>
</section>
```

### Слайд 2: С двумя колонками
```html
<section id="slide-2">
    <div class="slide-content">
        <div class="badge animate-on-view">
            <span class="badge-dot"></span>
            Этап 1
        </div>
        <h2 class="animate-on-view">Название раздела</h2>
        <hr class="divider animate-on-view">

        <div class="grid-2 stagger">
            <div class="glass-card animate-on-view accent">
                <div class="icon-circle">
                    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                        <circle cx="12" cy="12" r="10"></circle>
                    </svg>
                </div>
                <h4>Левая часть</h4>
                <p>Описание левой части</p>
            </div>

            <div class="glass-card animate-on-view accent">
                <div class="icon-circle">
                    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                        <rect x="3" y="3" width="18" height="18" rx="2"></rect>
                    </svg>
                </div>
                <h4>Правая часть</h4>
                <p>Описание правой части</p>
            </div>
        </div>
    </div>
</section>
```

### Слайд 3: С процессом
```html
<section id="slide-3">
    <div class="slide-content">
        <h2 class="animate-on-view">Этапы</h2>
        
        <div class="process-flow animate-on-view">
            <div class="process-step">
                <div class="step-icon">1</div>
                <div class="step-label">Шаг 1</div>
            </div>
            <div class="process-arrow">→</div>
            <div class="process-step">
                <div class="step-icon">2</div>
                <div class="step-label">Шаг 2</div>
            </div>
            <div class="process-arrow">→</div>
            <div class="process-step">
                <div class="step-icon">3</div>
                <div class="step-label">Шаг 3</div>
            </div>
        </div>
    </div>
</section>
```

### Слайд 4: Со статистикой
```html
<section id="slide-4">
    <div class="slide-content">
        <h2 class="animate-on-view">Результаты</h2>

        <div class="grid-3 stagger">
            <div class="stat-card animate-on-view">
                <div class="stat-number">100+</div>
                <div class="stat-label">Проектов</div>
            </div>
            <div class="stat-card animate-on-view">
                <div class="stat-number">500</div>
                <div class="stat-label">Часов</div>
            </div>
            <div class="stat-card animate-on-view">
                <div class="stat-number">99%</div>
                <div class="stat-label">Успеха</div>
            </div>
        </div>
    </div>
</section>
```

### Слайд 5: Финальный
```html
<section id="slide-final">
    <div class="slide-content thank-you-slide">
        <h1 class="animate-on-view" style="background: var(--gradient); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;">
            Спасибо за внимание!
        </h1>
        <p class="animate-on-view">Вопросы и обсуждение</p>

        <div class="authors-grid stagger">
            <div class="author-card animate-on-view">
                <div class="author-avatar">А</div>
                <div class="author-name">Автор</div>
            </div>
        </div>
    </div>
</section>
```

---

## 🎨 CSS переменные для персонализации

```css
:root {
    --accent-1: #6366f1;        /* Основной цвет */
    --accent-2: #3b82f6;        /* Вторичный */
    --accent-3: #0ea5e9;        /* Третичный */
    --accent-4: #06b6d4;        /* Четвертичный */
    --text-primary: #fafafa;    /* Основной текст */
    --text-secondary: #a1a1aa;  /* Вторичный текст */
    --bg-dark: #09090b;         /* Фон */
}
```

---

## 📏 Рекомендации по использованию

1. **Grid 2** - для сравнения, до/после, левое/правое
2. **Grid 3** - для статистики, трех точек, результатов
3. **Grid 4** - для 4+ этапов, шагов процесса
4. **Glass Card** - для основного контента
5. **Stat Card** - только для чисел/статистики
6. **Key Point** - максимум 1-2 на слайд

---

**Версия**: 1.0  
**Последнее обновление**: 2026-04-13
