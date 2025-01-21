<?php
session_start();

if ($_SERVER['REQUEST_METHOD'] === 'POST') {
    $start = isset($_POST['start']) ? (int)$_POST['start'] : null;
    $end = isset($_POST['end']) ? (int)$_POST['end'] : null;
    $exclude = isset($_POST['exclude']) ? array_map('intval', explode(',', $_POST['exclude'])) : [];

    if ($start !== null && $end !== null && $start < $end) {
        if (!isset($_SESSION['range']) || $_SESSION['range']['start'] !== $start || $_SESSION['range']['end'] !== $end) {
            $_SESSION['range'] = ['start' => $start, 'end' => $end];
            $_SESSION['remaining'] = range($start, $end);
        }
    }

    $_SESSION['exclude'] = $exclude;

    if (isset($_SESSION['remaining']) && !empty($_SESSION['remaining'])) {
        $_SESSION['remaining'] = array_diff($_SESSION['remaining'], $exclude);
        $_SESSION['remaining'] = array_values($_SESSION['remaining']);
    }

    if (isset($_SESSION['remaining']) && !empty($_SESSION['remaining'])) {
        $randomKey = array_rand($_SESSION['remaining']);
        $randomNumber = $_SESSION['remaining'][$randomKey];
        unset($_SESSION['remaining'][$randomKey]);
        $_SESSION['remaining'] = array_values($_SESSION['remaining']);
    } else {
        $randomNumber = 'No more unique numbers left in the range!';
    }
}
?>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Number Generator for DE314</title>
    <link rel="icon" href="https://seeklogo.com/images/L/lpu-sae-india-collegiate-club-logo-29B436A816-seeklogo.com.png">
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #ff7e5f, #feb47b);
            color: #333;
        }
        .header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: #333;
            padding: 15px 30px;
            color: #fff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .header h1 {
            font-size: 2.5rem;
            margin: 0;
            font-weight: bold;
            margin-left: 22%;
            letter-spacing: 1.5px;
            background: linear-gradient(to right, #ff7e5f, #feb47b);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .header img {
            height: 60px;
        }
        .container {
            position: absolute;
            left: 35%;
            margin-top: 7%;
            align-items: center;
            min-height: 100vh;
            padding: 30px;
            box-sizing: border-box;
        }
        .form-container {
            background: rgba(255, 255, 255, 0.9);
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 400px;
            text-align: center;
        }
        .form-container label {
            font-size: 1.2rem;
            color: #333;
            margin-bottom: 10px;
            display: block;
            font-weight: bold;
        }
        .form-container input {
            font-size: 1rem;
            padding: 10px;
            margin: 15px 0;
            border-radius: 8px;
            border: 1px solid #ccc;
            width: 100%;
            box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease-in-out;
        }
        .form-container input:focus {
            border-color: #ff7e5f;
            box-shadow: 0 0 8px rgba(255, 126, 95, 0.5);
        }
        .form-container button {
            padding: 12px 30px;
            font-size: 1.1rem;
            background: #333;
            color: #fff;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            transition: background 0.3s ease, transform 0.2s ease;
            width: 100%;
        }
        .form-container button:hover {
            background: #555;
            transform: scale(1.05);
        }
        .form-container .result {
            margin-top: 20px;
            font-size: 1.8rem;
            color: #006400;
            font-weight: bold;
        }
        footer {
            text-align: center;
            padding: 15px;
            background: #333;
            color: #fff;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>Random Number Generator for DE314</h1>
        <img src="https://images.seeklogo.com/logo-png/51/1/lovely-professional-university-logo-png_seeklogo-510818.png?v=1957919895149956000" alt="LPU Logo">
    </div>
    <div class="container">
        <div class="form-container">
            <form method="POST">
                <label for="start">Starting Roll No:</label>
                <input type="number" name="start" id="start" value="<?= isset($_SESSION['range']['start']) ? $_SESSION['range']['start'] : '' ?>" required>
                <br>
                <label for="end">Ending Roll No:</label>
                <input type="number" name="end" id="end" value="<?= isset($_SESSION['range']['end']) ? $_SESSION['range']['end'] : '' ?>" required>
                <br>
                <label for="exclude">Exclude Numbers (comma separated):</label>
                <input type="text" name="exclude" id="exclude" placeholder="E.g., 3, 7, 12" value="<?= isset($_POST['exclude']) ? htmlspecialchars($_POST['exclude']) : '' ?>">
                <br>
                <button type="submit">Generate Random Number</button>
            </form>
            <?php if (isset($randomNumber)): ?>
                <div class="result">
                    <?= is_numeric($randomNumber) ? "Random Number: $randomNumber" : $randomNumber ?>
                </div>
            <?php endif; ?>
        </div>
    </div>
    <footer>
        &copy; 2025 Lovely Professional University
    </footer>
</body>
</html>
