# ER Model to Text - Test Cases

This repository contains test cases for evaluating the transformation of ER (Entity-Relationship) models into textual descriptions using LLMs. Each test case consists of:

- A textual representation of the ER diagram
- The corresponding textual description of the ER model

## Table of Contents

- [Test Cases](#test-cases)
- [Structure of the Repository](#structure-of-the-repository)
- [How to Use](#how-to-use)
- [Contributing](#contributing)
- [License](#license)

## Test Cases

Below is a summary of the test cases included in this repository:

| Test Case | Application Domain                                                        |
| --------- | ------------------------------------------------------------------------- |
| Test 1    | Platform for multimedia content management                                |
| Test 2    | Library loan management                                                   |
| Test 3    | Boat rental                                                               |
| Test 4    | Management of radiological examinations                                   |
| Test 5v1  | Server management                                                         |
| Test 5v2  | Database for managing a cluster of servers                                |
| Test 6    | Collection of information about territorial control performed by officers |
| Test 7    | Online newspaper publisher                                                |
| Test 8    | Kitchen appliance stores                                                  |
| Test 9    | Museum restoration                                                        |
| Test 10   | Management of a free-floating e-scooter sharing rental company            |
| Test 11   | Online services such as movie rental, online music, and video games       |
| Test 12   | Airline company management                                                |

## Structure of the Repository

Each test case is stored in a separate folder under `test_cases/`, containing:

- `ER_model.txt`: A structured textual representation of the ER model.
- `description.txt`: A natural language description of the ER model.

Example structure:

```
/test_cases/
    /test_1/
        ER_model.txt
        description.txt
    /test_2/
        ER_model.txt
        description.txt
    ...
```

## How to Use

1. Clone this repository:
   ```bash
   git clone [https://github.com/your-repository/er-model-to-text.git](https://github.com/AndreaAvignone/ER2Text.git)
   ```
2. Navigate to the test cases folder:
   ```bash
   cd er-model-to-text/test_cases/
   ```
3. Open a specific test case folder to view its ER model and description.

## Contributing

We welcome contributions! To contribute:

1. Fork this repository.
2. Add new test cases following the existing structure.
3. Submit a pull request with a clear description of your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

