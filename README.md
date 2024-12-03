# URL Encoder Application

## Overview
The `UrlEncoder` program is a simple Java Swing-based GUI application that allows users to encode and decode URLs using the `java.net.URLEncoder` and `java.net.URLDecoder` utilities. It provides an intuitive interface for performing these operations.

---

## Features
1. **Encode URL**: Converts a raw URL string to a URL-encoded format.
2. **Decode URL**: Converts an encoded URL back to its original raw format.
3. **Graphical User Interface (GUI)**: Provides a user-friendly interface to input and display results.
4. **Error Handling**: Logs exceptions in case of encoding/decoding failures.

---

## Installation
1. **Requirements**:
   - JDK 8 or higher.
   - Java Swing library (part of the JDK).
2. **Compilation**:
   Compile the program using the `javac` command:
   ```bash
   javac UrlEncoder.java
   ```
3. **Execution**:
   Run the application using the `java` command:
   ```bash
   java UrlEncoder
   ```

---

## Usage
### Steps to Encode a URL
1. Launch the application.
2. Enter the raw URL in the **Row URL** text field.
3. Click the **Encode** button.
4. The encoded URL will appear in the **Encoded URL** text field.

### Steps to Decode a URL
1. Enter an encoded URL in the **Encoded URL** text field.
2. Click the **Decode** button.
3. The decoded URL will appear in the **Row URL** text field.

---

## Example
**Input**:  
Row URL: `https://example.com/page?param=value`

**Action**: Click **Encode**

**Output**:  
Encoded URL: `https%3A%2F%2Fexample.com%2Fpage%3Fparam%3Dvalue`

**Input**:  
Encoded URL: `https%3A%2F%2Fexample.com%2Fpage%3Fparam%3Dvalue`

**Action**: Click **Decode**

**Output**:  
Row URL: `https://example.com/page?param=value`

---

## Logging
In case of errors during encoding or decoding, exceptions are logged using `java.util.logging`.

---

## Future Enhancements
- Add support for additional encoding formats.
- Improve error messages displayed to the user.
- Enhance the GUI with a more modern look and feel.

---

## License
This project is licensed under the MIT License.
