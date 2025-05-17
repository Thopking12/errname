# Errname: Sentinel Error Linter for Golang

![GitHub release](https://img.shields.io/github/release/Thopking12/errname.svg) ![GitHub issues](https://img.shields.io/github/issues/Thopking12/errname.svg) ![GitHub stars](https://img.shields.io/github/stars/Thopking12/errname.svg)

## Overview

Welcome to **Errname**, the Golang linter designed to ensure that your sentinel errors follow best practices. This tool checks that sentinel errors are prefixed with `Err` and that error types are suffixed with `Error` or `Errors`. By adhering to these conventions, you can improve the readability and maintainability of your code.

## Table of Contents

1. [Features](#features)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Configuration](#configuration)
5. [Contributing](#contributing)
6. [License](#license)
7. [Contact](#contact)

## Features

- **Static Analysis**: Errname performs static analysis on your Go code to identify errors that do not meet the naming conventions.
- **Customizable Rules**: Adjust the linter settings to fit your project's specific needs.
- **Easy Integration**: Integrate Errname into your existing workflow seamlessly.
- **Detailed Reporting**: Get clear feedback on the errors detected, making it easier to fix them.

## Installation

To install Errname, you can download the latest release from our [Releases page](https://github.com/Thopking12/errname/releases). Download the appropriate binary for your operating system, and follow the instructions to execute it.

```bash
# Example for Linux
wget https://github.com/Thopking12/errname/releases/download/v1.0.0/errname-linux-amd64
chmod +x errname-linux-amd64
sudo mv errname-linux-amd64 /usr/local/bin/errname
```

## Usage

Once you have installed Errname, you can run it against your Go files. Use the following command to lint your code:

```bash
errname path/to/your/code
```

Errname will analyze the specified files and output any errors it finds. You can also specify multiple files or directories.

## Configuration

Errname supports configuration through a `.errname.yaml` file. You can place this file in your project root to customize the linter's behavior. Here’s an example configuration:

```yaml
rules:
  sentinel_prefix: "Err"
  error_suffix: ["Error", "Errors"]
```

## Contributing

We welcome contributions to Errname! If you have suggestions for improvements or want to report issues, please open an issue or submit a pull request. Ensure that your code adheres to the project's coding standards.

### Steps to Contribute

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Make your changes and commit them.
4. Push your changes to your forked repository.
5. Open a pull request.

## License

Errname is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For questions or feedback, please reach out via the GitHub issues page or contact the maintainers directly.

For more information, visit our [Releases page](https://github.com/Thopking12/errname/releases) to stay updated on new features and improvements. 

---

Thank you for checking out Errname! We hope it helps you maintain clean and effective Go code.