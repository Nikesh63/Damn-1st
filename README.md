
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





