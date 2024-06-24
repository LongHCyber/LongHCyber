# Hi there 👋

<div id="typewriter">
    <div class="line">👀 I’m interested in ...</div>
    <div class="line">🌱 I’m currently learning ...</div>
    <div class="line">💞️ I’m looking to collaborate on ...</div>
    <div class="line">📫 How to reach me ...</div>
    <div class="line">😄 Pronouns: ...</div>
    <div class="line">⚡ Fun fact: ...</div>
</div>

<style>
#typewriter {
    font-family: Arial, sans-serif;
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
    width: 0;
    animation: typing 3s steps(40, end) forwards, blink-caret 0.75s step-end infinite;
    display: block;
    margin: 0;
}

.line:nth-child(1) {
    animation-delay: 1s;
}

.line:nth-child(2) {
    animation-delay: 5s;
}

.line:nth-child(3) {
    animation-delay: 9s;
}

.line:nth-child(4) {
    animation-delay: 13s;
}

.line:nth-child(5) {
    animation-delay: 17s;
}

.line:nth-child(6) {
    animation-delay: 21s;
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
