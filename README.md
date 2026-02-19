# Navratri
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Nav Ratri</title>
<style>
    body {
        margin: 0;
        font-family: Arial, sans-serif;
        background: radial-gradient(circle,#fc0 20%, #800000 40%, #4B0000 50%, #000080 100%);
  background-attachment: fixed;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        min-height: 100vh;
    }

    h1 {
        color:#ffbb00;
        margin-bottom: 20px;
    }
    .glow{
        color: #fff;
        text-shadow: 0 0 5px #fff,0 0 10px #fff,0 0 20px #fc0,0 0 30px #fc0,0 0 40px #f90,0 0 10px #f90;
    }

    .days {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 10px;
        margin-bottom: 20px;
    }

    .day-btn {
        padding: 10px 15px;
        border: none;
        border-radius: 5px;
        background-color: #ff6f91;
        color: white;
        cursor: pointer;
        font-size: 14px;
    }

    .day-btn:hover {
        background-color: #f9c506;
        color: #fff;
        box-shadow: 0 0 5px #fff,0 0 10px #fff,0 0 20px #fc0,0 0 30px #fc0,0 0 40px #f90,0 0 10px #f90;
    }

    .message {
        width: 80%;
        max-width: 400px;
        background: white;
        padding: 20px;
        border-radius: 10px;
        text-align: center;
        box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        min-height: 320px;
        font-size: 16px;
        color: #333;
    }

    .message img {
        width: 100%;
        max-width: 850px;
        margin-top: 15px;
        border-radius: 10px;
    }
    img{
        height: 10cm;
    }
    
  .particle {
  position: fixed;
  bottom: -10px;
  width: 8px; height: 8px;
  background: radial-gradient(circle, #ffd700, #ffcc33); /* Golden glow */
  border-radius: 50%;
  pointer-events: none;
  animation: floatUp 8s linear infinite;
}

@keyframes floatUp {
  0% { transform: translateY(0) translateX(0); opacity: 0; }
  20% { opacity: 0.8; }
  100% { transform: translateY(-110vh) translateX(100px); opacity: 0; }
}
.confetti {
  position: fixed;
  width: 4px; height: 12px; /* Rectangular shape */
  top: -20px;
  z-index: 999;
  pointer-events: none;
  animation: fall linear forwards;
}

@keyframes fall {
  0% { transform: translateY(0) rotate(0deg); opacity: 1; }
  100% { transform: translateY(100vh) rotate(720deg); opacity: 0; } /* Vanishes at bottom */
}

/* Styling for falling flowers */
.flower {
  position: fixed;
  top: -20px;
  font-size: 20px; /* Adjust size of flowers */
  user-select: none;
  pointer-events: none;
  z-index: 1000;
  animation: flowerFall linear forwards;
}

@keyframes flowerFall {
  0% { transform: translateY(0) rotate(0deg); opacity: 1; }
  100% { transform: translateY(100vh) rotate(360deg); opacity: 0; }
}
</style>
</head>
<body>

<h1 class="glow">Nav Ratri</h1>
<div class="particle"></div>

<div class="days">

    <button class="day-btn" data-msg="Nav Durga " data-img="nd2.jpg" >Days in 2026</button>
    <button class="day-btn" data-msg="॥ देवी शैलपुत्री ॥
वन्दे वाञ्छितलाभाय चन्द्रार्धकृतशेखराम्।
वृषारूढां शूलधरां शैलपुत्रीं यशस्विनीम्॥ १॥" data-img="D01.jfif ">Day 1</button>
    <button class="day-btn" data-msg="॥ देवी ब्रह्मचारिणी ॥    
दधाना करपद्माभ्यामक्षमालाकमण्डलू।
देवी प्रसीदतु मयि ब्रह्मचारिण्यनुत्तमा॥ २॥  💌" data-img="Maa Bramhacharni.jfif">Day 2</button>
    <button class="day-btn" data-msg="॥ देवी चन्द्रघण्टा ॥
पिण्डजप्रवरारूढा चण्डकोपास्त्रकैर्युता।
प्रसादं तनुते मह्यं चन्द्रघण्टेति विश्रुता॥ ३॥" data-img="Maa Chandraghanta🙏🏻.jfif">Day 3</button>
    <button class="day-btn" data-msg="॥ देवी कूष्माण्डा ॥
सुरासम्पूर्णकलशं रुधिराप्लुतमेव च।
दधाना हस्तपद्माभ्यां कूष्माण्डा शुभदास्तु मे॥ ४॥ " data-img="Navratri Day 4_ Maa Kushmanda 🌞✨__Maa Kushmanda….jfif">Day 4</button>
    <button class="day-btn" data-msg="॥ देवी स्कन्दमाता ॥
सिंहासनगता नित्यं पद्माश्रितकरद्वया।
शुभदास्तु सदा देवी स्कन्दमाता यशस्विनी॥ ५॥" data-img="download.jfif">Day 5</button>
    <button class="day-btn" data-msg="॥ देवी कात्यायनी ॥
चन्द्रहासोज्ज्वलकरा शार्दूलवरवाहना।
कात्यायनी शुभं दद्याद्देवी दानवघातिनी॥ ६॥" data-img="D06.jfif">Day 6</button>
    <button class="day-btn" data-msg="॥ देवी कालरात्रि ॥
एकवेणी जपाकर्णपूरा नग्ना खरास्थिता।
लम्बोष्ठी कर्णिकाकर्णी तैलाभ्यक्तशरीरिणी॥
वामपादोल्लसल्लोहलताकण्टकभूषणा।
वर्धनमूर्धध्वजा कृष्णा कालरात्रिर्भयङ्करी॥ ७॥ " data-img="D07.jfif">Day 7</button>
    <button class="day-btn" data-msg="॥ देवी महागौरी ॥
श्वेते वृषे समारूढा श्वेताम्बरधरा शुचिः।
महागौरी शुभं दद्यान्महादेवप्रमोददा॥ ८॥ " data-img="D08.jfif">Day 8</button>
    <button class="day-btn" data-msg="॥ देवी सिद्धिदात्री ॥
सिद्धगन्धर्वयक्षाद्यैरसुरैरमरैरपि।
सेव्यमाना सदा भूयात् सिद्धिदा सिद्धिदायिनी॥ ९॥" data-img="D09.jfif">Day 9</button>
    <button class="day-btn" data-msg="॥ इति श्री नवदुर्गा स्तोत्रम् सम्पूर्णम् ॥ " data-img="D10 (2).jfif">Day of Victory</button>
</div>

<div class="message" id="message">
    Select a day to see your special message
</div>

<script>
    
for (let i = 0; i < 40; i++) 
{
  const p = document.createElement('div');
  p.className = 'particle';
  p.style.left = Math.random() * 100 + "vw";
  p.style.animationDuration = (Math.random() * 5 + 5) + "s"; // Random speeds
  p.style.animationDelay = Math.random() * 8 + "s"; // Random starts
  p.style.filter = `blur(${Math.random() * 2}px)`; // Soft glow effect
  document.body.appendChild(p);
}
function triggerConfetti() {
  const colors = ['#ff0055', '#ffd700', '#00ff00', '#00e5ff', '#ffffff', '#800000'];
  for (let i = 0; i < 150; i++) {
    const c = document.createElement('div');
    c.className = 'confetti';
    c.style.left = Math.random() * 100 + "vw";
    c.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
    c.style.animationDuration = (Math.random() * 2 + 1) + "s"; // Fast fall
    c.style.animationDelay = Math.random() * 0.5 + "s";
    document.body.appendChild(c);
    
    // Remove from DOM after animation finishes to prevent lag
    setTimeout(() => { c.remove(); }, 3000);
  }
}

// Trigger on every button click
document.querySelectorAll('button').forEach(btn => {
  btn.addEventListener('click', triggerConfetti);
});

// Function to trigger 200 falling flowers on click
function triggerFlowers() {
  const flowers = ['🌸', '🌼', '🌹', '🌺', '🌻'];
  for (let i = 0; i < 100; i++) {
    const f = document.createElement('div');
    f.className = 'flower';
    f.innerText = flowers[Math.floor(Math.random() * flowers.length)];
    f.style.left = Math.random() * 100 + "vw";
    f.style.animationDuration = (Math.random() * 3 + 2) + "s";
    f.style.fontSize = (Math.random() * 15 + 15) + "px";
    document.body.appendChild(f);
    
    // Automatically removes element after it touches the end line
    setTimeout(() => { f.remove(); }, 5000);
  }
}

// Attach to all buttons
document.querySelectorAll('button').forEach(btn => {
  btn.addEventListener('click', triggerFlowers);
});

const buttons = document.querySelectorAll('.day-btn');
const messageDiv = document.getElementById('message');

buttons.forEach(btn => {
    btn.addEventListener('click', () => {
        const msg = btn.getAttribute('data-msg');
        const img = btn.getAttribute('data-img');

        messageDiv.innerHTML = `
            <p>${msg}</p>
            <img src="${img}" alt="Valentine Image">
        `;
    });
});
</script>

</body>
</html>
