# Code-alpha
Basic Network Sniffer - CodeAlpha Cyber Security Internship
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    padding: 20px;
}

.container {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
}

.calculator {
    background: #2d2d2d;
    border-radius: 20px;
    box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
    padding: 20px;
    width: 100%;
    max-width: 300px;
}

.display {
    margin-bottom: 20px;
}

#result {
    width: 100%;
    padding: 20px;
    font-size: 28px;
    border: none;
    border-radius: 10px;
    background: #1a1a1a;
    color: #00ff00;
    text-align: right;
    font-weight: bold;
    margin-bottom: 10px;
}

#result::placeholder {
    color: #666;
}

.buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
}

.btn {
    padding: 20px;
    font-size: 18px;
    font-weight: bold;
    border: none;
    border-radius: 10px;
    background: #404040;
    color: #ffffff;
    cursor: pointer;
    transition: all 0.3s ease;
}

.btn:hover {
    background: #505050;
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
}

.btn:active {
    transform: translateY(0);
}

.btn.operator {
    background: #667eea;
    color: #ffffff;
}

.btn.operator:hover {
    background: #764ba2;
}

.btn.clear {
    background: #e74c3c;
    grid-column: 1;
}

.btn.clear:hover {
    background: #c0392b;
}

.btn.delete {
    background: #f39c12;
    grid-column: 4;
}

.btn.delete:hover {
    background: #e67e22;
}

.btn.equals {
    background: #27ae60;
    grid-column: 3 / 5;
    font-size: 20px;
}

.btn.equals:hover {
    background: #229954;
}

.btn.zero {
    grid-column: 1 / 3;
}

@media (max-width: 400px) {
    .calculator {
        padding: 15px;
    }

    .btn {
        padding: 15px;
        font-size: 16px;
    }

    #result {
        padding: 15px;
        font-size: 24px;
    }
}