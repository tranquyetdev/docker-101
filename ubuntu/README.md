# Ubuntu

This is my Ubuntu PC, with a pre-configured environment for software development. It includes essential tools, packages, and Python libraries to get started quickly. So I can easily set up my development environment on any machine, without the need to install everything from scratch.

## Packages

| Name                       | Description                                                                                                 |
| -------------------------- | ----------------------------------------------------------------------------------------------------------- |
| build-essential            | A package that provides the essential tools for building software, including GCC and make.                  |
| git                        | A distributed version control system to track changes in source code during software development.           |
| curl                       | A command-line tool used to transfer data from or to a server, supporting various protocols.                |
| wget                       | A command-line tool used to download files from the web via HTTP, HTTPS, and FTP.                           |
| ca-certificates            | A package that includes common CA certificates to ensure SSL connections are trusted.                       |
| software-properties-common | A set of tools for managing software properties and repositories in Ubuntu.                                 |
| python3                    | The default Python 3 programming language interpreter.                                                      |
| python3-pip                | A package manager for Python 3 used to install and manage Python packages.                                  |
| python3-venv               | A tool to create isolated Python environments for projects, preventing dependency conflicts.                |
| python3-dev                | A package providing the necessary header files and libraries to build Python modules.                       |
| python3-setuptools         | A package that includes tools for distributing Python packages, primarily for development.                  |
| python3-wheel              | A package to build and provide wheels (a built package format) for Python distribution.                     |
| libssl-dev                 | Development files needed for applications that use the Secure Sockets Layer (SSL) protocol.                 |
| libffi-dev                 | Development files needed for applications that use the Foreign Function Interface (FFI) for calling C code. |

### Python

| Name    | Description                                                                                                               |
| ------- | ------------------------------------------------------------------------------------------------------------------------- |
| ipython | An enhanced interactive Python shell with additional features such as auto-completion, history, and debugging.            |
| pylint  | A static code analysis tool for Python that checks for coding errors, enforces coding standards, and detects code smells. |
| black   | An uncompromising Python code formatter that reformats code to follow consistent style, ensuring uniformity.              |
| flake8  | A tool that checks Python code for compliance with PEP 8 style guidelines, linting errors, and complexity.                |

## Getting Started

```bash
# Change the directory to the ubuntu folder
cd ubuntu

# Build the image
docker build -t tranquyet/myubuntu .

# Run the container right away
docker run --rm --name myubuntu -it tranquyet/myubuntu bash

# Check the Python version
python3 --version

# Have fun!
exit

# Push the image to Docker Hub
docker push tranquyet/myubuntu
```
