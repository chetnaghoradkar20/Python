# Python

### Project Overview:
The provided code is a Python script utilizing the Selenium library for web automation. Its primary objective is to navigate a website (https://ABC.com), log in, interact with various dropdowns and filters, capture screenshots, and compile these screenshots into PDFs based on different filter combinations.

### Libraries and Tools Utilized:
- **Selenium**: Used for web automation, interaction with web elements, and capturing screenshots.
- **PIL (Python Imaging Library)**: Utilized for handling images.
- **ReportLab**: Used to generate PDFs.
- **Base64**: Used to handle image data.
- **OS and Time**: For handling file paths and implementing time delays.
- **WebDriverWait, Expected Conditions**: Utilized for synchronizing script actions with page elements.
- **ActionChains**: Employed for performing complex interactions (like mouse movements, keyboard actions) on the webpage.
- **ChromeOptions**: Configured Chrome browser options (e.g., full-screen mode, zoom level).
  
### Functionality Overview:
1. **Login Mechanism**:
    - The script navigates to the specified URL and automates the login process by providing the username and password.
  
2. **Dropdown Selection and Filtering**:
    - Interacts with dropdowns to select various options (Option A, Option B, etc.).
    - Filters data based on Filter3 and a combination of Filter1 and Filter2 options.

3. **Screenshot Capture**:
    - Takes screenshots of filtered results for different Filter1 and Filter2 combinations.
  
4. **PDF Compilation**:
    - Groups the captured screenshots based on dropdown options and combinations of Filter1 and Filter2 into respective PDFs.
    - Utilizes ReportLab to convert images to PDF format.

### Key Functions:
- **`click_element_by_xpath()`**: Clicks an element identified by its XPath after waiting for it to be clickable.
- **`send_keys_to_element_by_xpath()`**: Sends keys to an element identified by its XPath after waiting for it to be visible.
- **`set_value_in_input()`**: Sets values in input fields identified by their XPaths after ensuring they are clickable.
- **`capture_screenshot()`**: Captures and saves a screenshot of the current webpage based on layout metrics obtained via Chrome DevTools Protocol (CDP).
- **`generate_combinations()`**: Generates combinations of Filter1 and Filter2 options for screenshot names.
- **`convert_images_to_pdf()`**: Compiles existing images into a PDF document based on dropdown options and Filter1/Filter2 combinations.

### Browser Configuration:
- Chrome options are set to start the browser in full-screen mode and with a specific zoom level.

### Loop and Execution:
- Iterates through different dropdown options and, for each option, performs filtering, captures screenshots, and compiles them into PDFs.

### Conclusion:
The script automates a complex process involving website navigation, data filtering, screenshot capture, and PDF generation. It showcases the capabilities of Selenium for web automation and provides a robust framework for handling multiple interactions and document generation based on user-defined parameters and web elements.
