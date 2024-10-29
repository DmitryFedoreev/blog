---
title: "Мои проекты"
date: 2024-05-27
draft: false
---

<div id="typed-text" style="display: inline;"></div> <!-- Здесь будет печатающий текст -->
<span id="cursor" style="display: inline-block;">|</span> <!-- Палочка -->

<script>
document.addEventListener("DOMContentLoaded", function() {
    const texts = ["Здесь вы найдете некоторые из моих проектов, над которыми я работал."];
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

В каждый проект можно зайти и ознакомиться с деталями более подробно.