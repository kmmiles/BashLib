# Readme

## Project structure

The source files are located in `src/`, examples in `examples/` and tests in `tests/`.
Files in `examples/`, `src/` and `tests/` rely on files in `src/` only.  No other directional dependency is permitted (and no cycles!).

```
.
├── examples
│   ├── logging
│   └── string
│       ├── case
│       ├── pad
│       └── repeat
├── src
│   ├── logging
│   ├── runner
│   ├── string
│   │   ├── case
│   │   ├── pad
│   │   └── repeat
│   └── testing
└── tests
    ├── logging
    └── string
        ├── case
        ├── pad
        └── repeat
```


## Installation

Set the env variable BashLib to the src directory of this project

```
cd project/src
export BashLib="$PWD"
```


## Usage

If you wish to use the ucase function which is defined in string/case, do this:

```
source "${BashLib}/case"

ucase 'Some text'
```

## Library contents

### Functions

- logging
   - echo\_info
   - echo\_warn
   - echo\_err
- string
  - case
    - lcase
    - ucase
  - repeat
    - repeat
  - pad
    - string\_pad\_left
    - string\_pad\_right
    - string\_pad\_inner
    - string\_pad\_outer


## Contributions

- Feature submittions must be supplied to a new branch, with comprehensive tests, all in a single commit per feature.  If this condition is not met, the request will immediately be rejected.
- Bug reports must be accompanied by the necessary tests to recreate the issue.  This will help identify the cause of the issue, and prevent regressions in the future.


##  Disclaimers

This library is:

- not guaranteed to work
- not guaranteed to be free of bugs
- made in our free time
- shared with you with no expectation of recompence

