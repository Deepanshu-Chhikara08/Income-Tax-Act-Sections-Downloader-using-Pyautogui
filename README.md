### **Income Tax Act Section Downloader**

Automate the process of downloading sections of the Income Tax Act as PDF files. This script, powered by PyAutoGUI, navigates through a web page, prints sections, saves them with unique names, and moves to the next section in a seamless loop.

---

## **Features**
- Automatically selects and prints sections from the [Income Tax Act](https://incometaxindia.gov.in/pages/acts/income-tax-act.aspx).
- Dynamically names PDF files (e.g., `section-1.pdf`, `section-2.pdf`, ...).
- Handles navigation and file saving without user intervention.
- Fully customizable to adapt to different screen resolutions and layouts.

---

## **Prerequisites**
1. **Install Python Libraries**:
   Install the required Python library:
   ```bash
   pip install pyautogui
   ```
2. **Environment Setup**:
   - Open the URL: [Income Tax Act](https://incometaxindia.gov.in/pages/acts/income-tax-act.aspx) in the **first tab** of your browser.
   - Ensure your screen resolution matches the coordinate system in the script or adjust accordingly.

---

## **Usage**
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd income-tax-act-downloader
   ```
2. Run the script:
   ```bash
   python income_tax_act_downloader.py
   ```

---

## **Code Workflow**
1. **Navigate to the First Tab**:
   - Clicks on the first tab in the browser to ensure the correct page is active is https://incometaxindia.gov.in/pages/acts/income-tax-act.aspx.
2. **Select the First Section**:
   - Initiates the process by selecting the first section of the Income Tax Act.
3. **Print Current Section**:
   - Opens the print dialog for the current section.
4. **Save as PDF**:
   - Clears the existing file name, assigns a new name (e.g., `section-1`), and saves the file.
5. **Navigate to Next Section**:
   - Closes the current tab and moves to the next section, repeating the process.

---

## **Customization**
- **Adjust Coordinates**:
  Use `pyautogui.position()` to find the correct screen coordinates for your setup and update the script accordingly.
- **Modify Delays**:
  Modify `time.sleep()` values to match your browser’s response times.

---

## **Important Notes**
- Ensure the screen resolution and browser window layout match the script coordinates.
- Test the script on a small range of sections before running the full loop.
- Use with care, as PyAutoGUI directly interacts with the screen and mouse.

---

## **License**
This project is licensed under the MIT License. Feel free to use and modify as needed.
