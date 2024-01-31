# ANTI-ISRAEL
intellectual code for smart people only

If you would like your program to boycott "israel" for Palestine, use one of these;

## Nodejs
```js
const lang=process.env.LANG||"",isHebrew=lang.toLowerCase().includes("he");isHebrew&&(console.error("Not available in your region"),process.exit(1));
```
## Python
requirements: pip install keyboard
```py
import locale, keyboard

def detect_hebrew_keyboard():
    try:
        if locale.getdefaultlocale()[0].lower().startswith('he') or keyboard.get_keyboard_layout().startswith('he'): raise ValueError('Not available in your region')
    except Exception as e: exit(1)

detect_hebrew_keyboard()
```
## C++
requirements: #include <windows.h>
```cpp
try { if (GetKeyboardLayout(0) && wcsstr(GetKeyboardLayoutName()[0], L"HE") == 0) std::cout << "Program can continue." << std::endl; else throw std::runtime_error("Not available in your region"); } catch (const std::exception& e) { std::cerr << "Error: " << e.what() << std::endl; return 1; }
```
