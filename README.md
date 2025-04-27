# random-caption-generator
# HTML code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random caption Generator</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>Random caption Generator</h1>
        <blockquote id="caption">"Click the button to generate a caption!"</blockquote>
        <button id="new-caption">New caption</button>
    </div>
    <script src="script.js"></script>
</body>
</html>


# css code
body {
    font-family: Arial, sans-serif;
    background-color: white;
    margin: 0;
    padding: 0;
}

.container {
    text-align: center;
    background: white;
    padding: 20px;
}

h1 {
    color: white;
    background-color: brown;
    font-weight: bold;
    margin: 4cm 0 2cm 0;
    padding: 10px 0;
    text-align: center;
}

blockquote {
    font-size: 28px;
    margin: 0 0 2cm 0;
    color: #555;
    height: 4.5em;
    overflow: hidden;
}

button {
    display: block;
    margin: 0 auto;
    padding: 10px 20px;
    font-size: 1em;
    border: none;
    border-radius: 5px;
    background-color: #007BFF;
    color: white;
    cursor: pointer;
}

button:hover {
    background-color: #0056b3;
}

# java code
const caption = [
    "Lost in a world only I can see.",
    "Golden hours and soft thoughts.",
    "Moonchild in a sunlit world.",
    "Waves whispered, I listened.",
    "Chaos, but make it beautiful.",
    "Gentle with myself, fierce with my dreams.",
    "Sipping on sunsets and soft moments.",
    "Kind heart, wild soul, soft touch.",
    "Where flowers bloom, so does hope.",
    "Less perfection, more authenticity.",
    "Muted tones, loud dreams.",
    "Simplicity speaks louder.",
    "Inhale peace, exhale chaos.",
    "In the quiet, I found myself.",
    "Writing chapters they will never read.",
    "Somewhere between dreaming and living.",
    "Bloom softly, even when no one notices.",
    "Polaroids of a life well lived.",
    "Retro soul with a modern glow.",
    "Lost in another era.",
    "Old souls find new beginnings.",
];

const captionElement = document.getElementById('caption');
const button = document.getElementById('new-caption');

button.addEventListener('click', () => {
    const randomIndex = Math.floor(Math.random() * caption.length);
    captionElement.textContent = caption[randomIndex];
});
