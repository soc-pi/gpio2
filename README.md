# gpio2

## Description
A simple kernel module with a user-space application.

## Project Structure
```
gpio2/
├── kernel_module/
│   ├── src/
│   │   └── gpio2.c
│   ├── include/
│   │   └── gpio2.h
│   └── Makefile
└── application/
    ├── main.c
    └── CMakeLists.txt
```

## Build

### Kernel Module
```bash
cd gpio2/kernel_module
make
```

### Application
```bash
cd gpio2/application
cmake .
make
```

## Usage

### Kernel Module
```bash
sudo insmod gpio2/kernel_module/gpio2.ko
# Do something with the module
sudo rmmod gpio2
```

### Application
```bash
cd gpio2/application
./test_app
```

## License
GPL
