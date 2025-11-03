# pass
Random Password Generator
# Random Password Generator

A simple Python script that generates a secure random password.

## Run
```bash
python main.py




---

### 🔐 **main.py**
```python
import random
import string

def generate_password(length=12):
    chars = string.ascii_letters + string.digits + "!@#$%^&*()?"
    return "".join(random.choice(chars) for _ in range(length))

if __name__ == "__main__":
    print("Your new password:", generate_password())
