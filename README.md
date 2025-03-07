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

Each ER_model.txt contains the comment for specific structures (e.g., Relationships, Generalizations) to support the reader and optionally provide a hint for the LLM.

```
/* Relationships: */
FROM ( AIRPORT: one..many, FLIGHT: one..one) 
TO ( FLIGHT: one..one, AIRPORT: one..many) 
OF ( GROUND_STAFF: one..many, SHIFT: one..one external) 
AT ( AIRPORT: one..many, SHIFT: one..one) 
HAS ( FLIGHT: one..many, TICKET: one..one external) 
```

```
/* Generalizations: */ 
STAFF <= { GROUND_STAFF, CABIN_CREW} (total, exclusive) 
```

## How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/AndreaAvignone/ER2Text.git
   ```
2. Navigate to the test cases folder:
   ```bash
   cd ER2Text/test_cases/
   ```
3. Open a specific test case folder to view its ER model and description.

## Contributing

We welcome contributions! To contribute:

1. Fork this repository.
2. Add new test cases following the existing structure.
3. Submit a pull request with a clear description of your changes.


## Citation

This work is currently under review for publication. If you use this code or the ideas presented in this repository, please temporarily cite it as follows:

```bibtex
@misc{ER2Text_2025,
  author = {Andrea Avignone, Alessia Tierno, Alessandro Fiori, Silvia Chiusano},
  title = {ER2Text},
  year = {2025},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/AndreaAvignone/ER2Text.git}},
  note = {Work under review}
}
```

## License

This project is licensed under the Apache-2.0 license - see the [LICENSE](LICENSE) file for details.

