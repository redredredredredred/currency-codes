# currency-codes-form-iban
Obtain the latest data of currency- Codes from the official website of an international bank



## 🔨 Usage
Enter the following code in the console of the website to obtain the latest currency-Codes data

```
let a = [];
Object.values(document.getElementsByTagName("tbody")[0].children).map(
  (item) => {
    a.push({
      "country-name": item.children[0].innerText,
      "currency-unit": item.children[1].innerText,
      "currency-code": item.children[2].innerText,
    });
  }
);
a;
```

## 🔗 Links

- [iban website - currency codes page](https://www.iban.hk/currency-codes)
- [wikipedia - currency codes](https://zh.m.wikipedia.org/zh-hans/ISO_4217)
