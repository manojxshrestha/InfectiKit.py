# **InfectiKit - Android RAT (Remote Access Trojan)**

**InfectiKit** is a powerful tool designed for creating and managing Android RATs (Remote Access Trojans), allowing users to generate malicious APKs with reverse shell payloads using **msfvenom**. It also includes features for modifying APK files, such as changing version information and replacing strings, as well as uploading generated files to file-sharing services. This tool integrates with **Metasploit** to facilitate penetration testing and educational purposes related to Android security.

---

## **Features**
- **Generate Android RAT APKs**: Create custom Trojan APKs with reverse shell payloads using **msfvenom**.
- **Modify APK Version Information**: Change the `versionName` and `versionCode` in APK files.
- **Replace Strings in APK**: Replace specific strings in APK files for further customization.
- **Upload Files**: Upload generated APK files to file-sharing services like **transfer.sh** or **file.io**.

---

### Step 1: **Installation Process**

1. **Clone the repository** from GitHub:

    ```bash
    git clone https://github.com/manojxshrestha/InfectiKit.py.git
    ```

2. **Change to the project directory**:

    ```bash
    cd InfectiKit.py
    ```

### Step 2: **Set Up a Virtual Environment (Optional but Recommended)**
Creating a virtual environment for this project helps manage dependencies and avoid conflicts with your global Python packages.

1. **Create a virtual environment**:

    ```bash
    python3 -m venv infectikit-env
    ```

2. **Activate the virtual environment**:

    - On Linux/macOS:

      ```bash
      source infectikit-env/bin/activate
      ```

    - On Windows:

      ```bash
      .\infectikit-env\Scripts\activate
      ```

   Once activated, your prompt should change to `(infectikit-env)` indicating that you're working inside the virtual environment.

### Step 3: **Install Dependencies**
Since the `InfectiKit.py` repository may not include a `requirements.txt` file, you need to manually create one to install the necessary Python dependencies.

1. **Create the `requirements.txt` file** with the following content:

    ```bash
    nano requirements.txt
    ```

    Add these lines to the file:

    ```
    requests
    Pillow
    ```

    Save the file by pressing `CTRL + X`, then `Y`, and `Enter`.

2. **Install the dependencies** by running:

    ```bash
    pip install -r requirements.txt
    ```

### Step 4: **Run the Tool**
Once the dependencies are installed, you can run the `InfectiKit.py` tool.

1. **Run the tool** with the following command:

    ```bash
    python3 InfectiKit.py
    ```

2. The tool will start, and you’ll be presented with a menu to choose from various actions (e.g., generate APK, modify APK version, etc.).

### Step 5: **Follow On-Screen Instructions**
After running the tool, follow the on-screen instructions to use the tool effectively.

- You’ll likely be asked for input such as:
  - **Local IP Address and Port** to create a trojan APK using `msfvenom`.
  - Various modifications like changing the version or replacing strings in the APK.

---

### Troubleshooting
If you run into any errors or issues:
- Ensure that all dependencies are installed correctly.
- If any part of the script throws an error, check the Python version (`python3 --version`) and make sure you're running the script within the virtual environment.

---

This should be enough to get the tool up and running!
