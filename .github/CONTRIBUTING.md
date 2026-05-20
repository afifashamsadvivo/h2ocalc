# Contributing to h2ocalc

Thank you for your interest in helping build **The Ultimate H₂O Calculator 3000**! We welcome contributions from developers of all skill levels. To ensure a smooth development process, please take a moment to review these guidelines before submitting code.

## ⚡ Core Architectural Rules
Before you write any code, please note our strict project guardrails:
1. **Zero `eval()` Policy:** Under no circumstances will structural patches using `eval()`, `Function()`, or `setTimeout/setInterval` with string arguments be merged. All parsing adjustments must be integrated natively into the existing tokenized Shunting-Yard arithmetic core.
2. **Decimal Precision Guard:** Code alterations must respect or improve floating-point thresholding routines to prevent classic IEEE 754 precision errors.
3. **No Dependencies:** This project targets lean, semantic Web standards. Do not introduce runtime framework dependencies, build layers, or external compilation utilities.

## 🚀 How to Contribute

### 🐛 Reporting Bugs
* Open a GitHub issue describing the anomaly clearly.
* Provide the exact mathematical string that induced the layout failure or evaluation bug.
* Mention your operational environment (e.g., Desktop Chrome, Mobile Safari).

### 💡 Suggesting Enhancements
* Open an issue outlining the target functional tier or mathematical operator you wish to append.
* Explain how the addition serves operators or engineers in basic, scientific, or computing workflows.

### 📥 Submitting Pull Requests
1. Fork the repository and create your feature branch:
   ```bash
   git checkout -b feature/amazing-new-operator
   ```
2. Implement your logic, keeping changes clean, semantic, and highly readable.
3. Verify your modifications against basic desktop and responsive mobile touch displays.
4. Commit your changes with a punchy message:
   ```bash
   git commit -m "feat: integrate safe hyperbolic sine parsing path"
   ```
5. Push to your branch and open a clean Pull Request targeting our main branch.
