:root {
    --primary: #4CAF50;
    --secondary: #2196F3;
    --danger: #F44336;
    --warning: #FFC107;
    --dark: #333;
    --light: #f5f5f5;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    background-color: #f0f2f5;
}

.login-screen {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: var(--primary);
}

.login-box {
    background: white;
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    width: 90%;
    max-width: 400px;
    text-align: center;
}

.login-box h2 {
    margin-bottom: 1.5rem;
    color: var(--dark);
}

.login-box input {
    width: 100%;
    padding: 12px;
    margin: 8px 0;
    border: 1px solid #ddd;
    border-radius: 4px;
    font-size: 16px;
}

.login-box button {
    width: 100%;
    padding: 12px;
    background-color: var(--primary);
    color: white;
    border: none;
    border-radius: 4px;
    font-size: 16px;
    cursor: pointer;
    margin-top: 1rem;
}

.error {
    color: var(--danger);
    margin-top: 1rem;
}

.app-container {
    display: none;
    padding: 1rem;
    max-width: 1200px;
    margin: 0 auto;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 1.5rem;
}

.logout-btn {
    padding: 8px 16px;
    background-color: var(--danger);
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

.dashboard {
    margin-bottom: 2rem;
}

.balance-cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1rem;
    margin-bottom: 1.5rem;
}

.card {
    background: white;
    padding: 1.5rem;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.card h3 {
    font-size: 1rem;
    color: #666;
    margin-bottom: 0.5rem;
}

.card p {
    font-size: 1.8rem;
    font-weight: bold;
}

.quick-stats {
    background: white;
    padding: 1.5rem;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.quick-stats h2 {
    font-size: 1.2rem;
    margin-bottom: 1rem;
}

.stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    gap: 1rem;
}

.stat-item {
    text-align: center;
}

.stat-item span {
    display: block;
    color: #666;
    font-size: 0.9rem;
}

.stat-item p {
    font-size: 1.5rem;
    font-weight: bold;
    margin-top: 0.5rem;
}

.tabs {
    display: flex;
    border-bottom: 1px solid #ddd;
    margin-bottom: 1rem;
}

.tab-btn {
    padding: 12px 20px;
    background: none;
    border: none;
    cursor: pointer;
    font-size: 1rem;
    color: #666;
    position: relative;
}

.tab-btn.active {
    color: var(--primary);
    font-weight: bold;
}

.tab-btn.active::after {
    content: '';
    position: absolute;
    bottom: -1px;
    left: 0;
    width: 100%;
    height: 3px;
    background-color: var(--primary);
}

.tab-content {
    display: none;
    padding: 1rem;
    background: white;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.tab-content.active {
    display: block;
}

/* Add more styles for forms, tables, etc. */
