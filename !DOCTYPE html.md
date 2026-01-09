<!DOCTYPE html>  
<html lang="en">  
<head>  
  <meta charset="UTF-8" />  
  <title>Jah’s Pound Service</title>  
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />  
  <style>  
    body {  
      font-family: Arial, sans-serif;  
      background: #0f172a;  
      color: #e5e7eb;  
      display: flex;  
      justify-content: center;  
      align-items: center;  
      min-height: 100vh;  
    }  
  
    .card {  
      background: #020617;  
      padding: 25px;  
      border-radius: 12px;  
      width: 100%;  
      max-width: 420px;  
      box-shadow: 0 0 20px rgba(0,0,0,0.6);  
    }  
  
    h1 {  
      text-align: center;  
      margin-bottom: 5px;  
    }  
  
    p {  
      font-size: 14px;  
      color: #9ca3af;  
      text-align: center;  
      margin-bottom: 20px;  
    }  
  
    label {  
      display: block;  
      margin-top: 15px;  
      font-weight: bold;  
    }  
  
    select, input[type="range"], textarea, button {  
      width: 100%;  
      margin-top: 8px;  
    }  
  
    textarea {  
      height: 70px;  
      border-radius: 6px;  
      padding: 8px;  
    }  
  
    button {  
      margin-top: 20px;  
      padding: 12px;  
      background: #22c55e;  
      border: none;  
      border-radius: 8px;  
      font-size: 16px;  
      cursor: pointer;  
    }  
  
    button:hover {  
      background: #16a34a;  
    }  
  
    .result {  
      text-align: center;  
      margin-top: 20px;  
      display: none;  
    }  
  </style>  
</head>  
<body>  
  
  <div class="card">  
    <h1>Jah’s Pound Service</h1>  
    <p>Anonymous • Honest • 18+</p>  
  
    <form id="ratingForm">  
      <label>Did he move correctly?</label>  
      <select required>  
        <option value="">Choose one</option>  
        <option>Yes, perfectly 😮‍💨</option>  
        <option>Mostly good</option>  
        <option>Needs improvement</option>  
      </select>  
  
      <label>Rhythm (1 = off, 10 = elite)</label>  
      <input type="range" min="1" max="10" value="5" />  
  
      <label>Communication during the moment</label>  
      <select required>  
        <option value="">Choose one</option>  
        <option>Very good</option>  
        <option>Okay</option>  
        <option>Could be better</option>  
      </select>  
  
      <label>Overall satisfaction</label>  
      <input type="range" min="1" max="10" value="6" />  
  
      <label>Would you recommend?</label>  
      <select required>  
        <option value="">Choose one</option>  
        <option>Yes, 100%</option>  
        <option>Maybe</option>  
        <option>No</option>  
      </select>  
  
      <label>Would you do it again?</label>  
      <select required>  
        <option value="">Choose one</option>  
        <option>Absolutely 👀</option>  
        <option>Maybe</option>  
        <option>No</option>  
      </select>  
  
      <label>Extra comments (optional)</label>  
      <textarea placeholder="Any final thoughts..."></textarea>  
  
      <button type="submit">Submit Rating</button>  
    </form>  
  
    <div class="result" id="result">  
      <h2>Feedback received 😌</h2>  
      <p>Thanks for rating Jah’s Pound Service.</p>  
    </div>  
  </div>  
  
  <script>  
    const form = document.getElementById("ratingForm");  
    const result = document.getElementById("result");  
  
    form.addEventListener("submit", function(e) {  
      e.preventDefault();  
      form.style.display = "none";  
      result.style.display = "block";  
    });  
  </script>  
  
</body>  
</html>  
