# Pet Library (Static & Shared)

This project demonstrates how to create and use **static** and **shared libraries** in C. It includes basic functions for handling **dog** and **cat** operations.

## 📁 Project Structure
```
├── src/        # Source files (cat.c, dog.c, main.c)
├── inc/        # Header files (cat.h, dog.h)
├── obj/        # Compiled object files
├── lib/        # Static & shared libraries
│   ├── static/
│   ├── shared/
├── bin/        # Executables
└── Makefile    # Build automation
```

## 🚀 Build & Run

### 1️⃣ Compile with **Static Library**
```sh
make all_static
./bin/use-static-lib
```

### 2️⃣ Compile with **Shared Library**
```sh
make all_shared
export LD_LIBRARY_PATH=$(pwd)/lib/shared:$LD_LIBRARY_PATH
./bin/use-shared-lib
```

## 🧹 Clean Build Files
```sh
make clean
```

## 🛠 Features
- Uses **Makefile** for automation
- Supports both **static (`.a`)** & **shared (`.so`)** libraries
- Demonstrates basic function calling in C
