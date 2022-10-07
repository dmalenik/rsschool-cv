# DMYTRO MALIENIK

\+ 48 690 208 735 | dmalenik@gmail.com | [LinkedIn](https://www.linkedin.com/in/dmitriy-m-137a735b/) | [GitHub](https://github.com/dmalenik)

## Summary

Front-end developer. Looking for an internship.  
Core stack: HTML, CSS, JavaScript, TypeScript, React.

## Skills

### Programming languages

- JavaScript
- TypeScript

### Libraries

- React
- Jest.js
- Mocha.js

### Methodologies

- CI/ CD
- Scrum

### Version control

- Git

### Tools

- Node.js
- Windows CLI
- n8n

## Code examples

``` JavaScript
const nums = [3, 2, 1, 4, 6, 5, 7, 9, 8, 10];

const countDigits = (num, count = 0) => {
  return num ? countDigits(Math.floor(num / 10), ++count) : count;
};

const findDigitsArr = (arr, countFn) => arr.map(num => countFn(num));

const findMaxDigitNumber = digitsArr => Math.max(...digitsArr);

const getDigit = (num, i = 0) => {
  return Math.floor(Math.abs(num) / Math.pow(10, i)) % 10; 
};

const radixSort = numbers => {
  let i = 0;
  const maxDigitNumber = findMaxDigitNumber(findDigitsArr(numbers, countDigits));

  while (i < maxDigitNumber) {
    let buckets = Array.from({length: 10}, () => []);

    numbers.map(num => {
      let digit = getDigit(num, i);

      buckets[digit].push(num);
    });

    numbers = [].concat(...buckets);

    i++;
  }

  return numbers;
};
```

## Experience

2022-02-08 | [Currency converter](https://github.com/dmalenik/currencyconverter)

- *Single page application of currency converter reworked with React*

2022-01-23 | [Currency counter](https://github.com/dmalenik/project-4-220116.github.io)

- *Single page application of currency converter created with JavaScript*

2022-01-14 | [Home budget accountant](https://github.com/dmalenik/project-3-211210.github.io)

- *Single page application of personal finance accounting developed with JavaScript*

## Education

current | **JS/Frontend development course**

- [Rolling Scopes School](https://wearecommunity.io/events/rs-js-en-2022q3)

2022-01-23 | **JavaScript & React**

- [Future Collars](https://futurecollars.com/kursy/pakiet-frontend-developer/)

2021-11-06 | **English for IT**

- [Eklektika](https://eklektika.pl/en/learning-platform/english-for-it/)

2021-10-24 | **HTML/ CSS**

- [Future Collars](https://futurecollars.com/kursy/pakiet-frontend-developer/)

2019-11-28 | **Communication Skills**

- [EY Global Delivery Services Poland](https://www.ey.com/en_pl/careers/global-delivery-services)

2019-10-31 | **Creative Skills for Innovation**

- [PFR, Google](https://startup.pfr.pl/en/news/pfr-innovation-designers-register-free-design-thinking-workshop/)

## English

- B2 (read technical documentation, guidelines and handbooks, listen to tutorials)
