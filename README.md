# Calculator App - Built Using Algorand AlgoKit SDK

This application performs basic calculator operations: **Addition**, **Subtraction**, **Multiplication**, and **Division**.

---

## Project Structure

This project uses AlgoKit's workspace structure. By default:
- Projects are stored in the `projects` directory.
- You can create new projects using the `algokit init` command.

---

## Steps to Create and Deploy the Calculator App  

### 1. Initialize the Project  
1. Open your terminal or command prompt.  
2. Navigate to your desired directory.  
3. Run the following command to initialize an AlgoKit project:  
   ```bash
   algokit init
   ```
4. During initialization, provide the following details when prompted:
    *Project type*: Smart Contract
    *Language*: Python
    *Project name*: hello
    *Name of project type*: hello-world (default)
    *Template*: starter
    *Bootstrap Git Repo*: Yes (installs dependencies)

### 2. Install Dependencies (if needed)
- If dependencies are missing or not properly installed, use this command:
   ```bash
   algokit bootstrap all
   ```

### 3. Navigate to the Project Directory
- The project structure will look like this:
  ```bash
  Calculator-App-Algorand/
  └── projects/
      └── calculator/
          ├── smart_contracts/
          │   └── calculator/
          │       ├── contract.py       # Smart contract logic
          │       └── deploy_config.py  # Deployment configuration
  ```

### 4. Build and Initialize the Project
- Run the following command to build and initialize the project:
  ```bash
  algokit project run build
  ```
### 5. Start Docker Engine
- Ensure Docker is installed and running on your system to use the local Algorand network.

### 6. Reset the Local Network (Optional)
- If needed, reset the local network using:

  ```bash
  algokit localnet reset
  ```
  
### 7. Deploy the Smart Contract
- Deploy and execute the smart contract in the local network using:

  ```bash
  algokit project localnet deploy
  ```
  
- Once deployed, the smart contract will execute, and the results of the calculator operations will be displayed.

## Summary of Commands

### 1. Initialize Project:
    ```bash
    algokit init
    ```

### 2. Install Dependencies (if needed):
    ```bash
    algokit bootstrap all
    ```
    
### 3. Build Project:
     ```bash
    algokit project run build
    ```

### 4. Reset Local Network (Optional):
     ```bash
    algokit localnet reset
    ```

### 5. Deploy and Run Smart Contract:
     ```bash
    algokit project localnet deploy
    ```


## Getting Started

1. Refer to the `README.md` files in the `projects` directory for more details about specific sub-projects.  
2. To learn more about AlgoKit, visit the [AlgoKit Documentation](https://github.com/algorandfoundation/algokit-cli/blob/main/docs/algokit.md).

---

## GitHub Codespaces (Optional)

If you're using GitHub Codespaces:
1. Run `algokit generate devcontainer` to configure the repository for Codespaces.  
2. Inside a Codespace, run `algokit init` to create a new AlgoKit project.

---
