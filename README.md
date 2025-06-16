# 🧪✨ Fortran Project - Build & Run Guide (Visual Studio + Intel Fortran)

📌 *By [Abhisekh Nayek](https://github.com/AbhisekhNayek)*

---

This project contains Fortran source code that can be compiled and executed using **Microsoft Visual Studio** with the **Intel® Fortran Compiler** (oneAPI HPC Toolkit).

---

## ✅ Prerequisites

Make sure the following are installed:

- 💻 **Microsoft Visual Studio 2022** (Community or Professional)
- 🔧 **Intel® oneAPI HPC Toolkit** (includes Intel Fortran Compiler `ifx`)

---

## 📂 Folder Structure

```

project-folder/
│
├── source/
│   ├── main.for
│   ├── module1.for
│   └── ...
├── README.md

```

---

## 🧑‍💻 How to Compile & Run in Visual Studio

### 🔹 Step 1: Launch Visual Studio

- 🚀 Open **Visual Studio 2022**

### 🔹 Step 2: Create a New Project

- 📁 Go to `File → New → Project`
- 🧾 Choose **Console App** under **Intel Fortran**
- ⏭ Click **Next**

### 🔹 Step 3: Configure Project

- 📝 Name: `YourProjectName`
- 📂 Location: Point to your `source/` folder
- ✅ Click **Create**

### 🔹 Step 4: Add Source Files

- ➕ Right-click `Source Files` → `Add → Existing Item`
- 🗂 Select all `.for` / `.f90` files from `source/` and click **Add**

### 🔹 Step 5: Set Configuration

- ⚙️ Choose `Release` or `Debug`
- 💽 Set platform to `x64` (top toolbar)

### 🔹 Step 6: Build the Project

- 🛠 Go to `Build → Build Solution` or press `Ctrl + Shift + B`
- 📦 The `.exe` will be generated at:
```

project-folder\YourProjectName\x64\Release\\

````

### 🔹 Step 7: Run the Program

- ▶️ `Debug → Start Without Debugging` or press `Ctrl + F5`

---

## 💻 Optional: Build & Run via Command Line

If you prefer terminal:

```cmd
cd /d D:\path\to\source
ifx *.for /warn:all /traceback /debug:full -o run.exe
run.exe
````

🧠 *Use the "Intel oneAPI Command Prompt for Intel 64" (search in Start menu)*

---

## 💬 Support & Credits

For help:

* ✅ Confirm `ifx` is installed and available in your environment
* ✅ Refer: [Intel® Fortran Docs](https://www.intel.com/content/www/us/en/developer/tools/oneapi/fortran-compiler.html)

---

📘 **References:**

* 🔗 [Intel® Fortran Documentation](https://www.intel.com/content/www/us/en/developer/tools/oneapi/fortran-compiler.html)

✍️ *Compiled by: [Abhisekh Nayek](https://github.com/AbhisekhNayek)*
💡 *Ideal for hydrology, scientific modeling & academic research.*
