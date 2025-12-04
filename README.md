# 🧮 bigmathlib (NPM Package)

**bigmathlib** is a lightweight and fast arbitrary-precision decimal math library for Node.js and browser environments.  
It allows you to work with large numbers safely without losing precision — perfect for finance, blockchain, scientific computation, and any high-precision number operations.

---

## ✨ Features

- Arbitrary precision decimal arithmetic
- Supports add, subtract, multiply, divide, modulo, power, sqrt, comparison, rounding & formatting
- Configurable decimal places and rounding mode
- Zero dependency & highly optimized
- Works in **Node.js**, **Browser**, **TypeScript** environments

---

## 📦 Installation

```bash
npm install bigmathlib
# or
yarn add bigmathlib
# or
pnpm add bigmathlib
```

---

## 🚀 Usage

```javascript
import Big from "bigmathlib";

const a = new Big("12345678901234567890.12345");
const b = new Big("10");

console.log(a.plus(b).toString());   // → "12345678901234567900.12345"
console.log(a.times(b).toString());  // → "123456789012345678901.2345"
console.log(a.div(b).toString());    // → precise division result
console.log(a.sqrt().toString());    // → square root with high precision
```

---

## 🔧 Configuration

```javascript
Big.DP = 50;          // Decimal precision
Big.RM = Big.roundUp; // Rounding mode
```

---

## API Overview

| Method                                                        | Description               |
| ------------------------------------------------------------- | ------------------------- |
| `plus(y)` / `add(y)`                                          | Addition                  |
| `minus(y)` / `sub(y)`                                         | Subtraction               |
| `times(y)` / `mul(y)`                                         | Multiplication            |
| `div(y)`                                                      | Division (with precision) |
| `mod(y)`                                                      | Modulo                    |
| `pow(n)`                                                      | Power (integer exponent)  |
| `sqrt()`                                                      | Square root               |
| `cmp(y)`                                                      | Compare numbers           |
| `eq / gt / gte / lt / lte`                                    | Comparisons               |
| `toFixed / toPrecision / toExponential / toString / toNumber` | Format output             |

## 📄 License

Copyright (c) 2025 kristaclark55

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
