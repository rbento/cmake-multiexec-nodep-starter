# cmake-multiexec-nodep

### About 

Template for CMake projects that are bare minimal, without any dependencies and which are expected to generate one separate executable per C source file

- Useful for projects containing multiple distinct code examples

- Each C source file is expected to have an entry point

### Usage

- Update project name in `CMakeLists.txt`

###### Visual Studio

- Open a local folder
- `Project` > `Generate cache for <project-name>`
- Right click a source file in the `Solution Explorer` and `Set as Startup Item`
- Build with `Ctrl+B`
- Debug with `F5`
