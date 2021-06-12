<h1 align = "center"> :fast_forward: Salary Calculator :rewind: </h1>

## 🖥 Preview
<p align = "center">
  <img src = "https://raw.githubusercontent.com/ecpieritz/SalaryCalculator/master/public/img/salary-calculator-print.jpg" width = "800">
</p>

---

## 📖 About
<p>Create, using React, an application named 'react-salario' that should be able to calculate the net salary from gross salary, considering the 2020 CLT rules.</p>

---

## 🛠 Technologies used
- CSS
- HTML
- Javascript
  - Class Components
- React
- Materialize
- Node.js

---

## 🔍Development Tips
- For the horizontal bar, use the Determinate Linear Preloader available on Materialize.

```
  <div class="progress">
      <div class="determinate" style="width: 20%"></div>
      <div class="determinate" style="width: 10%"></div>
  </div>
```

- As the bar shall be a sum of net salary and IRPF and INSS discounts, you can consider the background color as the net salary bar.
- For the other two bars, you will use the determinate class. Remember that the first one declared will be overlapped by the second. So a tip is to add the value to be presented in the latter to the former and set the calculated width to the former.
- For the percentages and currency formatting, use the Intl library.

```
const currencyFormatter = Intl.NumberFormat('pt-BR', { style: 'currency', currency: 'BRL' });
const percentageFormatter = Intl.NumberFormat('pt-BR', { style: 'percent', maximumFractionDigits: 2 });
```

---

## 🚀 How to execute the project
#### Clone the repository
git clone https://github.com/ecpieritz/SalaryCalculator.git

#### Enter directory
`cd SalaryCalculator`

#### Download dependencies
`npm install`

#### Run the server
`npm start`

#### That done, open your browser and go to `https://localhost:3000/`

---
Developed with 💙 by Emilyn C. Pieritz
