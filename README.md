# Scientific Calculator

A desktop scientific calculator built with Python and Tkinter. It has a standard mode for everyday arithmetic and a scientific mode that adds trigonometric, hyperbolic, logarithmic and other mathematical functions.

## Features

- **Basic arithmetic:** addition, subtraction, multiplication, division and modulus
- **Two modes:** switch between *Standard* and *Scientific* layouts from the **File** menu
- **Square root** and **sign toggle** (±)
- **Clear controls:** `C` clears the current entry, `CE` resets everything including the stored total
- **Constants:** π, 2π (tau) and e
- **Trigonometric functions:** sin, cos, tan
- **Hyperbolic functions:** sinh, cosh, tanh, asinh, acosh
- **Logarithms and exponentials:** log (natural), log10, log2, log1p, exp, expm1
- **Other functions:** log-gamma and radians-to-degrees conversion
- **Exit confirmation** dialog to prevent accidental closing

## Scientific Functions

| Button | Operation |
|--------|-----------|
| `pi` / `2pi` / `e` | Insert π, 2π (tau) or Euler's number |
| `sin`, `cos`, `tan` | Trigonometric functions (input in **degrees**) |
| `sinh`, `cosh`, `tanh` | Hyperbolic functions |
| `asinh`, `acosh` | Inverse hyperbolic functions |
| `log` | Natural logarithm (ln) |
| `log10`, `log2` | Base-10 and base-2 logarithms |
| `log1p` | ln(1 + x) |
| `exp`, `expm1` | eˣ and eˣ − 1 |
| `gamma` | Natural log of the gamma function |
| `deg` | Convert radians to degrees |
| `Mod` | Remainder of a division |

## Requirements

- Python 3.x
- Tkinter (included with most Python installations)

No third-party packages are needed.

> **Linux users:** if Tkinter is missing, install it with `sudo apt install python3-tk`.

## Installation and Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
   ```
2. Run the calculator:
   ```bash
   python Sci-Cal.py
   ```
3. To enable the scientific functions, open **File → Scientific**. To go back, choose **File → Standard**.

## Project Structure

```
.
├── Sci-Cal.py          # Main application
├── docs/
│   └── images/
│       └── screenshot.png
└── README.md
```

## How It Works

The app is built around a `Calc` class that holds the calculator's state (running total, current input, pending operation) and a method for each button. The interface is laid out with Tkinter's grid geometry manager, and the window switches between Standard (480×568) and Scientific (944×568) sizes to reveal or hide the extra function buttons.

## Known Limitations

- Division by zero and invalid inputs (for example, `log` of a negative number) are not yet handled gracefully.
- The **Edit** menu items (Cut, Copy, Paste) are placeholders and have no functionality yet.
- Trigonometric functions expect degrees, not radians.

## Future Improvements

- Error handling with on-screen messages
- Keyboard input support
- Working Cut/Copy/Paste
- Radian/degree toggle
- Calculation history

## Contributing

Contributions, issues and feature requests are welcome. Feel free to open an issue or submit a pull request.

## License

MIT License

Copyright (c) 2026 [Nikesh Budhathoki]

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






