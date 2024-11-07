---
title: "About"
date: 2024-10-24
draft: false
---

<div id="typed-text" style="display: inline;"></div> <!-- Здесь будет печатающий текст -->
<span id="cursor" style="display: inline-block;">|</span> <!-- Палочка -->

<script>
document.addEventListener("DOMContentLoaded", function() {
    const texts = ["Инструменты которые я использую в работе"];
    let index = 0;
    let charIndex = 0;
    const typedText = document.getElementById("typed-text");
    const cursor = document.getElementById("cursor");

    function type() {
        if (charIndex < texts[index].length) {
            typedText.textContent += texts[index].charAt(charIndex);
            charIndex++;
            setTimeout(type, 100); // Задержка между печатью символов
        } else {
            // Запускаем мигание палочки после завершения печати
            cursor.style.animation = "blink 1s step-start infinite"; 
        }
    }

    // Начинаем печатать текст при загрузке страницы
    type(); 

    // Создаем анимацию мигания для палочки
    const style = document.createElement('style');
    style.innerHTML = `
        @keyframes blink {
            50% {
                opacity: 0;
            }
        }
    `;
    document.head.appendChild(style);
});
</script>



- Рекламные платформы: <code>Яндекс Директ</code>, <code>ВК</code>, <code>MyTarget</code>, <code>TargetHunter</code>.
  
- Веб-аналитика: <code>Яндекс Метрика</code>, <code>Google Analytics</code>.

- Сквозная аналитика: <code>Roistat</code>.

- Создание дашбордов: <code>Datalens</code>.

- Анализ данных: <code>SQL</code>, <code>Python</code> (отчеты в <code>Google Docs</code>).

- Управление сайтами и CRM:
  <code>Bitrix24</code>,
  <code>Tilda</code>,
  <code>WordPress</code>.

- Дизайн и мультимедиа:
  <code>Figma</code>,
  <code>Photoshop</code>,
  <code>Blender</code>,
  <code>Premiere Pro</code>,
  <code>After Effects</code>.

- Планирование и организация: 
  <code>Google Tasks</code>.

- Опыт управления: Руководство командой до 10 человек.

### Увлечения:

- Бег
- Лыжи
- Походы в горы