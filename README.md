# 🧪 Fortran Project - Build & Run Guide (Visual Studio + Intel Fortran)

This project contains Fortran source code that can be compiled and executed using **Microsoft Visual Studio** with the **Intel® Fortran Compiler** (oneAPI).

---

## ✅ Prerequisites

Make sure the following are installed:

- [x] Microsoft Visual Studio 2022 (Community or Professional)
- [x] Intel® oneAPI HPC Toolkit (includes the Intel Fortran Compiler `ifx`)

---

## 📁 Folder Structure

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

## 🛠 How to Compile & Run in Visual Studio

### 🔹 Step 1: Open Visual Studio
- Launch **Visual Studio 2022**

### 🔹 Step 2: Create a New Project
- Go to `File` → `New` → `Project`
- Choose **Console App** under **Intel Fortran**
- Click **Next**

### 🔹 Step 3: Configure Project
- Project Name: `YourProjectName`
- Location: Choose the folder containing the `source/` directory
- Click **Create**

### 🔹 Step 4: Add Existing Files
- In **Solution Explorer**, right-click `Source Files` → `Add` → `Existing Item`
- Navigate to the `source/` folder
- Select all `.for` or `.f90` files and click **Add**

### 🔹 Step 5: Set Build Configuration
- In the toolbar, make sure you select:
  - `Release` or `Debug`
  - `x64` platform

### 🔹 Step 6: Build the Project
- Go to `Build` → `Build Solution` (or press `Ctrl + Shift + B`)
- The `.exe` file will be created inside:
```

project-folder\YourProjectName\x64\Release\\

````

### 🔹 Step 7: Run the Program
- Go to `Debug` → `Start Without Debugging` (or press `Ctrl + F5`)

---

## 🧪 CLI Alternative (Optional)

If you want to build from terminal:

```cmd
cd /d path\to\source
ifx *.for /warn:all /traceback /debug:full -o myprogram.exe
myprogram.exe
````

---

## 💬 Support

For errors or questions, make sure:

* Visual Studio + Intel oneAPI environment is properly installed
* You opened the correct `x64 Native Tools Command Prompt for VS`


---

## 📄 Word Document Content (Copy-paste into Microsoft Word)

---

### 🧪 Fortran Project Setup, Build & Execution Guide

#### 📌 Purpose:
This guide helps you compile and execute Fortran applications using Microsoft Visual Studio with Intel® Fortran Compiler.

---

### ✅ Requirements:

| Software                   | Version     | Notes                          |
|----------------------------|-------------|---------------------------------|
| Microsoft Visual Studio    | 2022+       | Community/Professional          |
| Intel® oneAPI HPC Toolkit  | 2025.1+     | Includes Intel® Fortran Compiler (`ifx`) |

---

### 🛠 Step-by-Step Instructions

#### 1. Open Visual Studio
Launch Visual Studio from the Start Menu.

#### 2. Create New Fortran Console Project
- Go to `File > New > Project`
- Select `Console Application` under **Intel Fortran**
- Click `Next`

#### 3. Project Configuration
- Set Project Name and Location (should match your source folder)
- Click `Create`

#### 4. Add Existing Files
- Right-click `Source Files` → `Add > Existing Item`
- Select all `.for` or `.f90` files from your source folder

#### 5. Configure Build
- Select `Release` and `x64` from the toolbar dropdowns

#### 6. Build Solution
- Go to `Build > Build Solution` or press `Ctrl + Shift + B`
- If successful, the `.exe` is created in:
```

project-folder\ProjectName\x64\Release\\

````

#### 7. Run the Application
- Use `Debug > Start Without Debugging` or `Ctrl + F5`

---

### 📎 Optional: Run from Command Line

If you prefer the terminal:

```cmd
cd /d D:\path\to\source
ifx *.for /warn:all /traceback -o run.exe
run.exe
````

---

### ❗ Troubleshooting

* Ensure you use the `Intel oneAPI Command Prompt`
* Confirm the `.for` files are syntactically valid
* Always save and rebuild after any code change

