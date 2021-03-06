## Task

> (21.) Написать программу, в которой описана иерархия классов:
> функция от одной переменной (`синус`, `косинус`, `тангенс`).
> Описать класс для хранения коллекции функций (массива указателей на базовый класс),
> в котором перегрузить операцию "`[ ]`".
> Описать класс-итератор для итерации по элементам коллекции.
> Для базового класса и его потомков перегрузить операции "`==`", "`!=`", "`=`".
> Продемонстрировать работу операторов.

## Project tree

```bash
tree --charset ascii
```

```
.
|-- build            # Folder with the compiled project
|   |-- Debug        # Folder with the compiled project
|   |   `-- main.exe # Executable program (Windows)
|   |-- main         # Executable program (Linux)
|   |-- Makefile     # Compilation via make
|   |-- Project.cbp  # Launches CodeBlocks
|   `-- Project.sln  # Starts VisualStudio
|-- CMakeLists.txt   # Cmake configuration
|-- README*.md       # Repository information
`-- src              # Source code folder
    |-- **/*.c       # C source code
    |-- **/*.h       # C header files
    |-- **/*.cpp     # C++ source code
    `-- **/*.hpp     # C++ header files
```

## How to compile a project

To compile, you need 'cmake'.

```bash
mkdir build
```

```bash
cd build
```

```bash
cmake ..
# cmake .. -G "CodeBlocks - Unix Makefiles"
```

```bash
cmake --build .
```

```bash
./main
#./main.exe
# Debug/main.exe
```
