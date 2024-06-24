<div id="typewriter">
    <div class="line" data-text="👋 Hi, I’m @LongHCyber"></div>
    <div class="line" data-text="👀 I’m interested in ..."></div>
    <div class="line" data-text="🌱 I’m currently learning ..."></div>
    <div class="line" data-text="💞️ I’m looking to collaborate on ..."></div>
    <div class="line" data-text="📫 How to reach me ..."></div>
    <div class="line" data-text="😄 Pronouns: ..."></div>
    <div class="line" data-text="⚡ Fun fact: ..."></div>
</div>

<style>
body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    padding: 20px;
}

#typewriter {
    max-width: 600px;
    margin: 0 auto;
    font-size: 24px;
    line-height: 1.5;
}

.line {
    white-space: nowrap;
    overflow: hidden;
    border-right: 0.15em solid orange;
    box-sizing: border-box;
    animation: typing 2s steps(40, end), blink-caret 0.75s step-end infinite;
    display: none;
}

@keyframes typing {
    from { width: 0; }
    to { width: 100%; }
}

@keyframes blink-caret {
    from, to { border-color: transparent; }
    50% { border-color: orange; }
}
</style>

<script>
document.addEventListener("DOMContentLoaded", () => {
    const lines = document.querySelectorAll('.line');
    let delay = 0;

    lines.forEach((line, index) => {
        setTimeout(() => {
            line.style.display = 'block';
            const text = line.getAttribute('data-text');
            let charIndex = 0;

            const typeInterval = setInterval(() => {
                if (charIndex < text.length) {
                    line.textContent += text[charIndex];
                    charIndex++;
                } else {
                    clearInterval(typeInterval);
                }
            }, 100); // Adjust typing speed here
        }, delay);

        delay += 3000; // Adjust delay between lines here
    });
});
</script>
