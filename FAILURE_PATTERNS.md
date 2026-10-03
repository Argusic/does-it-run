# Failure patterns

What the clean machine printed when a project was installed and run, grouped by kind. Computed from 4981 observed error lines in 2231 valid runs of 1309 tested subjects (generated 2026-10-03).

A line is placed in the first group below whose rule it matches, in the order shown; anything else is "Other". The percentages are shares of all observed error lines.

| Pattern | Error lines | Share | Subjects affected |
|---|---|---|---|
| Port already in use | 6 | 0.1% | 4 |
| Permission denied | 44 | 0.9% | 39 |
| Missing system library or header | 285 | 5.7% | 152 |
| Tool, runtime or component not installed | 874 | 17.5% | 520 |
| Version mismatch | 546 | 11.0% | 340 |
| Missing configuration or secret | 96 | 1.9% | 85 |
| Source or download problem | 58 | 1.2% | 48 |
| Network, timeout or service unreachable | 88 | 1.8% | 74 |
| Dependency install or resolution failed | 565 | 11.3% | 382 |
| Build or compile step failed | 224 | 4.5% | 171 |
| The project's own tests failed | 601 | 12.1% | 337 |
| Expected file or data not present | 74 | 1.5% | 62 |
| Error inside the project's code | 51 | 1.0% | 44 |
| Other | 1469 | 29.5% | 653 |

## Port already in use

A second process wanted a port that was already taken.

Example runs:

- express, attempt 2: https://argusic.com/run/4e43cf30-bc87-4838-8e48-9bc64db2f542
- offen, attempt 2: https://argusic.com/run/bbe24165-6271-4a91-a006-ba9316769132
- OpenCut, attempt 2: https://argusic.com/run/91607940-1d49-43dd-bf44-4f7b1373cac7

## Permission denied

The step needed rights the clean machine user does not have.

Example runs:

- agnix, attempt 2: https://argusic.com/run/666f100e-cd99-4ed7-881b-cbbfce5a6335
- astron-rpa, attempt 3: https://argusic.com/run/03b42d69-76f6-4d73-9a94-6e36fee73057
- bb-browser, attempt 1: https://argusic.com/run/c811c7ea-44af-497d-9464-4a3c04150f0e

## Missing system library or header

A build or launch step needed a system package that was not installed.

Example runs:

- 0ad, attempt 2: https://argusic.com/run/19c34cdc-acd7-4d8f-ba3a-b6f02169729a
- allgood, attempt 1: https://argusic.com/run/fd4fad73-65a7-45d8-8c19-a62adf5c8545
- Amphion, attempt 1: https://argusic.com/run/60fe3cb8-a6da-4543-b5fb-c091176947ad

## Tool, runtime or component not installed

A language, tool or component the project needs was not present on the clean machine.

Example runs:

- 0ad, attempt 1: https://argusic.com/run/7c49b658-925d-4dc5-9752-5ad0a54e9d0b
- abtop, attempt 1: https://argusic.com/run/741cba9c-2e37-4d91-a3cd-6bdc76d8ae95
- aci, attempt 1: https://argusic.com/run/de9b7d61-248b-48b4-a990-3b619e3cdcfe

## Version mismatch

The tool or language version on the machine did not match what the project asks for.

Example runs:

- 0ad, attempt 2: https://argusic.com/run/19c34cdc-acd7-4d8f-ba3a-b6f02169729a
- 9router, attempt 1: https://argusic.com/run/6c9de159-ad3b-4e6f-bf1e-43978c798ae8
- Ackee, attempt 1: https://argusic.com/run/bcb0030f-094a-4183-b4c6-2020aa8d30c7

## Missing configuration or secret

The project expected a setting, key or file that a fresh checkout does not carry.

Example runs:

- agent-scan, attempt 1: https://argusic.com/run/49f30766-040f-4153-9f53-70d186bc9a48
- aimeos, attempt 1: https://argusic.com/run/8e93e50a-7bc9-4131-9dfd-3f43f0c07f2e
- anything-llm, attempt 1: https://argusic.com/run/c8e4f9f4-6e3c-43a6-a31d-2da53120dc26

## Source or download problem

A repository, submodule or file could not be fetched as the instructions describe.

Example runs:

- Acode, attempt 1: https://argusic.com/run/f12291ec-ba07-4e6f-9bd1-af099631ebd1
- across, attempt 1: https://argusic.com/run/958a29d8-b4cd-486c-9440-3ea46fa473bb
- aiohttp, attempt 1: https://argusic.com/run/53427ea4-8d8e-4775-9b61-b00a216af5f3

## Network, timeout or service unreachable

A request or a service call did not complete in time or was refused.

Example runs:

- a-stock-data, attempt 1: https://argusic.com/run/d7dc86f0-383f-42e0-bf4e-8d8dbc1a38fd
- Acode, attempt 1: https://argusic.com/run/f12291ec-ba07-4e6f-9bd1-af099631ebd1
- ai-memory, attempt 1: https://argusic.com/run/66b4137f-49a9-4d1f-86f3-fffcbc55cd72

## Dependency install or resolution failed

Installing or resolving the project's dependencies did not finish cleanly.

Example runs:

- 500-AI-Agents-Projects, attempt 1: https://argusic.com/run/230540eb-50de-4c61-ba6a-419e3094649b
- 9router, attempt 1: https://argusic.com/run/6c9de159-ad3b-4e6f-bf1e-43978c798ae8
- a-stock-data, attempt 1: https://argusic.com/run/d7dc86f0-383f-42e0-bf4e-8d8dbc1a38fd

## Build or compile step failed

A build, compile or import step stopped with an error.

Example runs:

- 0ad, attempt 2: https://argusic.com/run/a3f8b8d5-9983-4188-9476-ad481c6956eb
- agent-scripts, attempt 1: https://argusic.com/run/db72e9e3-9662-4f35-abc3-2326bef4dd10
- analog, attempt 1: https://argusic.com/run/10d7236e-d3b1-4651-b544-6d6e759089c7

## The project's own tests failed

The project's test suite stopped with failures on the clean machine.

Example runs:

- 500-AI-Agents-Projects, attempt 1: https://argusic.com/run/230540eb-50de-4c61-ba6a-419e3094649b
- Acode, attempt 1: https://argusic.com/run/f12291ec-ba07-4e6f-9bd1-af099631ebd1
- adk-python, attempt 2: https://argusic.com/run/a33ce9d1-4407-4d89-a357-1749004308af

## Expected file or data not present

A file, build output or data set the instructions rely on was not there.

Example runs:

- agent-toolkit-for-aws, attempt 1: https://argusic.com/run/273a9e50-3438-4fbc-89f0-ccea6890f0ee
- ai-job-search, attempt 3: https://argusic.com/run/ea1709f1-2bef-47f0-ac95-92e5e5261b5a
- Amphion, attempt 1: https://argusic.com/run/60fe3cb8-a6da-4543-b5fb-c091176947ad

## Error inside the project's code

The project itself raised an error while running.

Example runs:

- 500-AI-Agents-Projects, attempt 1: https://argusic.com/run/230540eb-50de-4c61-ba6a-419e3094649b
- AI-Youtube-Shorts-Generator, attempt 1: https://argusic.com/run/4327a267-507e-4887-ae23-c0c4b70acad6
- auto-editor, attempt 3: https://argusic.com/run/cd82652e-f5fe-42fa-aabf-cb15e6088b2e

## Other

Error lines that fit none of the groups above.

Example runs:

- 0ad, attempt 2: https://argusic.com/run/19c34cdc-acd7-4d8f-ba3a-b6f02169729a
- 500-AI-Agents-Projects, attempt 1: https://argusic.com/run/230540eb-50de-4c61-ba6a-419e3094649b
- 9router, attempt 1: https://argusic.com/run/6c9de159-ad3b-4e6f-bf1e-43978c798ae8
