# Ex06 BMI Calculator
## Date: 29/10/2025

## AIM
To create a BMI calculator using React Router 

## ALGORITHM
### STEP 1 State Initialization
Manage the current page (Home or Calculator) using React Router.

### STEP 2 User Input
Accept weight and height inputs from the user.

### STEP 3 BMI Calculation
Calculate the BMI based on user input.

### STEP 4 Categorization
Classify the BMI result into categories (Underweight, Normal weight, Overweight, Obesity).

### STEP 5 Navigation
Navigate between pages using React Router.

## PROGRAM
## APP.JSX
```
import React, { useState } from 'react';
import './App.css';

function App() {
  const [weight, setWeight] = useState('');
  const [height, setHeight] = useState('');
  const [bmi, setBmi] = useState(null);
  const [message, setMessage] = useState('');

  const calculateBMI = () => {
    if (weight && height) {
      const heightInMeters = height / 100;
      const calculatedBMI = (weight / (heightInMeters * heightInMeters)).toFixed(2);
      setBmi(calculatedBMI);
      getBMICategory(calculatedBMI);
    } else {
      alert('Please enter valid height and weight.');
    }
  };

  const getBMICategory = (bmi) => {
    if (bmi < 18.5) setMessage('Underweight');
    else if (bmi >= 18.5 && bmi < 24.9) setMessage('Normal weight');
    else if (bmi >= 25 && bmi < 29.9) setMessage('Overweight');
    else setMessage('Obese');
  };

  const resetFields = () => {
    setWeight('');
    setHeight('');
    setBmi(null);
    setMessage('');
  };

  return (
    <div className="wrapper">
      <div className="container">
        <h1>BMI Calculator</h1>

        <div className="input-group">
          <label>Weight (kg):</label>
          <input
            type="number"
            value={weight}
            onChange={(e) => setWeight(e.target.value)}
            placeholder="Enter weight"
          />
        </div>

        <div className="input-group">
          <label>Height (cm):</label>
          <input
            type="number"
            value={height}
            onChange={(e) => setHeight(e.target.value)}
            placeholder="Enter height"
          />
        </div>

        <button onClick={calculateBMI}>Calculate</button>
        <button className="reset" onClick={resetFields}>Reset</button>

        {bmi && (
          <div className="result">
            <h2>Your BMI: {bmi}</h2>
            <p className="message">{message}</p>
          </div>
        )}

        <footer> BY Lokesh Reddy A</footer>
      </div>
    </div>
  );
}

export default App;
```

## APP.CSS
```

.wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background: linear-gradient(135deg, #ffafbd, #ffc3a0);
}

.container {
  width: 350px;
  background: rgba(255, 255, 255, 0.85);
  padding: 25px;
  text-align: center;
  border-radius: 12px;
  box-shadow: 0px 0px 20px rgba(0,0,0,0.3);
  backdrop-filter: blur(4px);
}
.input-group {
  text-align: left;
  margin-bottom: 15px;
}

input {
  width: 100%;
  padding: 10px;
  margin-top: 5px;
  border-radius: 6px;
  border: 1px solid #ccc;
}

button {
  width: 100%;
  padding: 10px;
  margin-top: 10px;
  border: none;
  background: #007bff;
  color: white;
  border-radius: 6px;
  cursor: pointer;
  font-size: 16px;
  transition: 0.3s;
}

button:hover {
  opacity: 0.8;
}

.reset {
  background: #ff4d4d;
}

.result {
  margin-top: 20px;
  padding: 15px;
  background: #ffffffc7;
  border-radius: 10px;
}

footer {
  margin-top: 20px;
  font-size: 14px;
}
```

## OUTPUT

<img width="1920" height="1080" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/eca58e89-66be-4faf-8cf0-7a2fec583b74" />

<img width="1920" height="1080" alt="Screenshot (51)" src="https://github.com/user-attachments/assets/6c39a357-2f03-4cdd-80fb-47d6057539e5" />


## RESULT
The program for creating BMI Calculator using React Router is executed successfully.
