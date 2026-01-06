# Praktikum2-Penjualan
body {
    margin: 0;
    height: 100vh;
    background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: Arial, sans-serif;
}

.scene {
    width: 300px;
    height: 200px;
    perspective: 800px;
}

.card {
    width: 100%;
    height: 100%;
    position: relative;
    transform-style: preserve-3d;
    transition: transform 0.8s;
}

.scene:hover .card {
    transform: rotateY(180deg);
}

.card__face {
    position: absolute;
    width: 100%;
    height: 100%;
    border-radius: 15px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    backface-visibility: hidden;
    color: white;
}

.card__face--front {
    background: #00c6ff;
}

.card__face--back {
    background: #ff416c;
    transform: rotateY(180deg);
}

