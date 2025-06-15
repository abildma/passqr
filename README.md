# PassQR

A simple command-line tool to generate secure passwords and display them as QR codes.

## Features

- Generate secure passwords with customizable length
- Display password as a scannable QR code in the terminal
- Option to save QR code as a high-resolution PNG file
- Clean, simple interface with no external dependencies beyond Python standard library

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/passqr.git
   cd passqr
   ```

2. **Set up a virtual environment** (recommended)
   
   **Linux/macOS:**
   ```bash
   # Create virtual environment
   python3 -m venv venv
   
   # Activate the environment
   # For bash/zsh:
   source venv/bin/activate
   
   # For fish shell:
   # source venv/bin/activate.fish
   ```

   **Windows:**
   ```cmd
   :: Create virtual environment
   python -m venv venv
   
   :: Activate the environment
   .\venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Make the script executable** (Linux/macOS)
   ```bash
   chmod +x passqr
   ```

## Usage

```
./passqr [OPTIONS]

Options:
  --length N     Password length (default: 32)
  --no-animation Skip QR code animation
  -o, --output   Save QR code as PNG file
  --size N       PNG size in pixels (default: 768)
  -h, --help     Show help message
```

## Examples

```bash
# Generate a password with default settings
./passqr

# Generate a 24-character password
./passqr --length 24

# Skip the animation
./passqr --no-animation

# Save QR code as a PNG file
./passqr -o my_password.png

# Custom size for the PNG (1024x1024)
./passqr -o my_password.png --size 1024
```

## License

MIT
