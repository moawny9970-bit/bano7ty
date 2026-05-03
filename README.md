<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>❤️ لينا</title>
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700;900&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Cairo', sans-serif;
    background: #0f0f0f;
    color: white;
    overflow: hidden;
    text-align: center;
}

/* 🎬 Intro - أسود زي ما طلبت */
#intro {
    position: fixed;
    width: 100%;
    height: 100%;
    background: black;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    z-index: 9999;
}

.glow {
    width: 20px;
    height: 20px;
    background: #ff4d6d;
    border-radius: 50%;
    animation: grow 2.5s forwards;
    position: absolute;
    box-shadow: 0 0 30px #ff4d6d;
}

@keyframes grow {
    0% {
        transform: scale(1);
        opacity: 1;
    }
    100% {
        transform: scale(50);
        opacity: 0;
    }
}

#introText {
    position: relative;
    font-size: 26px;
    font-weight: 900;
    z-index: 10;
    text-shadow: 0 2px 15px rgba(255,77,109,0.8);
    animation: fadeIn 1s ease-in;
    color: white;
}

@keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
}

/* 🔐 Password - ثيم آيفون */
#lock {
    display: none;
    height: 100vh;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    background: #000;
    background-image: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
}

.lock-title {
    font-size: 22px;
    font-weight: 700;
    margin-bottom: 40px;
    opacity: 0.9;
}

.display {
    height: 30px;
    margin-bottom: 50px;
    display: flex;
    gap: 20px;
    justify-content: center;
    align-items: center;
}

.dot {
    width: 14px;
    height: 14px;
    border: 2px solid rgba(255,255,255,0.4);
    border-radius: 50%;
    transition: .3s;
}

.dot.filled {
    background: white;
    border-color: white;
    box-shadow: 0 0 10px rgba(255,255,255,0.5);
}

.keys {
    display: grid;
    grid-template-columns: repeat(3, 80px);
    gap: 20px;
    justify-content: center;
}

.key {
    width: 80px;
    height: 80px;
    background: rgba(255,255,255,0.1);
    backdrop-filter: blur(10px);
    border-radius: 50%;
    cursor: pointer;
    transition:.2s;
    font-size: 32px;
    font-weight: 300;
    border: 1px solid rgba(255, 255, 255, 0.1);
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
}

.key:active {
    transform: scale(0.9);
    background: rgba(255,255,255,0.3);
}

.key.empty {
    background: transparent;
    border: none;
    cursor: default;
}

.key.delete {
    font-size: 24px;
}

.key.delete:active {
    background: rgba(255, 77, 109, 0.3);
}

#error {
    color: #ff4d6d;
    margin-top: 25px;
    height: 20px;
    font-size: 16px;
    font-weight: 700;
}

/* 💌 message */
#message {
    display: none;
    padding: 30px;
    font-size: 22px;
    line-height: 2;
    height: 100vh;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    background: #0f0f0f;
}

/* 😏 kiss */
#kiss {
    display: none;
    height: 100vh;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 20px;
    background: #0f0f0f;
}

/* ❤️ hearts */
.heart {
    position: fixed;
    color: #ff4d6d
