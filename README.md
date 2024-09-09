# Keylogger with SMTP Email Sending in C#

## Overview

This project is a **C# Keylogger** that captures keystrokes, stores them in a file, and periodically sends the content of the file to an external email address using **SMTP**. The keylogger works silently in the background, capturing keyboard input and logging it to a file located in the user's **Documents** directory. Once a certain threshold is met (100 keystrokes in this example), the log file is sent via email to a configured Gmail account.

> **Note**: This software is intended for educational purposes only. Use of this software in unauthorized scenarios may violate privacy laws and other regulations.

## Features

- **Key Capture**: Monitors and captures keystrokes in real-time.
- **Console Output**: Displays captured keystrokes in the console.
- **Log Storage**: Saves keystrokes to a text file (`keystrokes.txt`) in the user's **Documents** folder.
- **Email Notification**: Sends the keystroke logs to a specified email every 100 keystrokes or at user-defined intervals.
- **System Information**: Sends system information such as the computer's IP address, username, and timestamp with each log.

## Requirements

- **.NET Framework**
- **Gmail Account** with a valid **App Password** (or SMTP server credentials).
- **Admin Privileges** (for certain keylogging functionalities).
  
### Libraries/Namespaces Used

- `System`
- `System.IO`
- `System.Net`
- `System.Net.Mail`
- `System.Runtime.InteropServices`
- `System.Threading`

## Setup

### Prerequisites

1. **Enable App Passwords on Gmail**:
   - Go to your [Google Account Security Settings](https://myaccount.google.com/security) and enable **2-Step Verification**.
   - Create an **App Password** for "Mail". This password will be used in the program to send emails.

2. **Install .NET Framework**: Make sure the .NET runtime is installed on your system.

### Using The Code
 **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/keylogger-csharp
```
## Future Improvements

-**Add encryption to the log file and email transmission for better security.**

-**Implement timed email sending instead of relying on keystroke count.**

-**Improve error handling and SMTP configuration flexibility.**
