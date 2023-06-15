# CompilerDesign

Assignment of Compiler Design BITS-Pilani M-tech SE

## Authors
Rahul Anand - 2021HS70030
Tushar Saraj - 2021HS70029

## Description
This repository contains the assignment for Compiler Design in BITS-Pilani M-tech SE program. It includes a compiler implementation made by Rahul Anand and Tushar Saraj.

## Steps to Run the Compiler

### System Requirements
- macOS or Windows with Cygwin

### Installation (macOS)
1. Open the terminal.
2. If Homebrew (brew) is not installed, install it by running the following command:
    ```shell
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```
3. Install Flex by executing the command:
    ```shell
    brew install flex
    ```
4. Install Bison by executing the command:
    ```shell
    brew install bison
    ```

### Setup
Clone the project repository to your local machine.

### Run
1. Open the terminal.
2. Change the directory to the cloned repository.
3. Execute the following commands in order:
    ```shell
    bison -y -d simpleC.y
    flex simpleC.l
    gcc y.tab.c lex.yy.c calc3b.c -o calc3b.exe
    ./calc3b.exe
    ```

### Cleaning the Folder
To safely clean the folder and remove the generated files, follow these steps:
1. Copy the contents of the "clean" file.
2. Open the terminal and navigate to the directory where the generated files are located.
3. Paste the copied contents into the terminal.
4. Run the pasted command to clean the folder.

**Note:** Make sure the terminal's working directory (pwd) is set to the same location where all the generated files are present.
