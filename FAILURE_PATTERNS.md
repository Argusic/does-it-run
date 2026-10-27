# Failure patterns

What the clean machine printed when a project was installed and run, grouped by kind. Computed from 10342 observed error lines in 4580 valid runs of 3333 tested subjects (generated 2026-10-27).

A line is placed in the first group below whose rule it matches, in the order shown; anything else is "Other". The percentages are shares of all observed error lines.

| Pattern | Error lines | Share | Subjects affected |
|---|---|---|---|
| Port already in use | 10 | 0.1% | 8 |
| Permission denied | 93 | 0.9% | 85 |
| Missing system library or header | 539 | 5.2% | 331 |
| Tool, runtime or component not installed | 1723 | 16.7% | 1173 |
| Version mismatch | 1083 | 10.5% | 799 |
| Missing configuration or secret | 221 | 2.1% | 200 |
| Source or download problem | 121 | 1.2% | 107 |
| Network, timeout or service unreachable | 200 | 1.9% | 178 |
| Dependency install or resolution failed | 1233 | 11.9% | 901 |
| Build or compile step failed | 455 | 4.4% | 367 |
| The project's own tests failed | 1137 | 11.0% | 709 |
| Expected file or data not present | 150 | 1.5% | 136 |
| Error inside the project's code | 126 | 1.2% | 114 |
| Other | 3251 | 31.4% | 1599 |

## Port already in use

A second process wanted a port that was already taken.

Example runs:

- bramble, attempt 1: https://argusic.com/run/86fee78c-2eeb-46ef-b0ac-e79d42644964
- express, attempt 2: https://argusic.com/run/4e43cf30-bc87-4838-8e48-9bc64db2f542
- gpt-image-canvas, attempt 1: https://argusic.com/run/d8d25e0d-d4ea-4810-a398-e3a7d32ae455

## Permission denied

The step needed rights the clean machine user does not have.

Example runs:

- agent-browser, attempt 1: https://argusic.com/run/5084027b-e339-48b7-8129-f7b2ed9cef9a
- agent-browser-cli, attempt 1: https://argusic.com/run/7afa98a3-8241-4f21-8f69-ff5adcf2854f
- agnix, attempt 2: https://argusic.com/run/666f100e-cd99-4ed7-881b-cbbfce5a6335

## Missing system library or header

A build or launch step needed a system package that was not installed.

Example runs:

- 0ad, attempt 2: https://argusic.com/run/19c34cdc-acd7-4d8f-ba3a-b6f02169729a
- addok, attempt 1: https://argusic.com/run/3ce89028-aef1-4fd5-840a-9a0c5bfebb20
- ADR, attempt 1: https://argusic.com/run/4cdad965-7d40-43bd-8309-0c026972680d

## Tool, runtime or component not installed

A language, tool or component the project needs was not present on the clean machine.

Example runs:

- 0ad, attempt 1: https://argusic.com/run/7c49b658-925d-4dc5-9752-5ad0a54e9d0b
- 10x, attempt 1: https://argusic.com/run/b1dd685d-6833-46e9-a645-306bfa854f57
- 4gaBoards, attempt 1: https://argusic.com/run/0a378b5b-de92-4e0a-b039-d56d6bd9e645

## Version mismatch

The tool or language version on the machine did not match what the project asks for.

Example runs:

- 0ad, attempt 2: https://argusic.com/run/19c34cdc-acd7-4d8f-ba3a-b6f02169729a
- 2fa, attempt 1: https://argusic.com/run/db3afea5-6210-4ddd-8230-a4cab1f62053
- 4gaBoards, attempt 1: https://argusic.com/run/0a378b5b-de92-4e0a-b039-d56d6bd9e645

## Missing configuration or secret

The project expected a setting, key or file that a fresh checkout does not carry.

Example runs:

- agent-browser, attempt 1: https://argusic.com/run/5084027b-e339-48b7-8129-f7b2ed9cef9a
- agent-scan, attempt 1: https://argusic.com/run/49f30766-040f-4153-9f53-70d186bc9a48
- agent-skills, attempt 1: https://argusic.com/run/ae5b1e9c-34b7-4fff-8c50-e757fdddf988

## Source or download problem

A repository, submodule or file could not be fetched as the instructions describe.

Example runs:

- Acode, attempt 1: https://argusic.com/run/f12291ec-ba07-4e6f-9bd1-af099631ebd1
- across, attempt 1: https://argusic.com/run/958a29d8-b4cd-486c-9440-3ea46fa473bb
- agents-universe, attempt 1: https://argusic.com/run/57845659-6dff-4f84-9779-a8f490ddfeef

## Network, timeout or service unreachable

A request or a service call did not complete in time or was refused.

Example runs:

- 10xProductivity, attempt 1: https://argusic.com/run/c40f7bbe-deed-4d3a-8fbc-1f980835bd12
- a-stock-data, attempt 1: https://argusic.com/run/d7dc86f0-383f-42e0-bf4e-8d8dbc1a38fd
- Acode, attempt 1: https://argusic.com/run/f12291ec-ba07-4e6f-9bd1-af099631ebd1

## Dependency install or resolution failed

Installing or resolving the project's dependencies did not finish cleanly.

Example runs:

- 4gaBoards, attempt 1: https://argusic.com/run/0a378b5b-de92-4e0a-b039-d56d6bd9e645
- 500-AI-Agents-Projects, attempt 1: https://argusic.com/run/230540eb-50de-4c61-ba6a-419e3094649b
- 9router, attempt 1: https://argusic.com/run/6c9de159-ad3b-4e6f-bf1e-43978c798ae8

## Build or compile step failed

A build, compile or import step stopped with an error.

Example runs:

- 0ad, attempt 2: https://argusic.com/run/a3f8b8d5-9983-4188-9476-ad481c6956eb
- acl, attempt 1: https://argusic.com/run/5d5a6c5b-4a2c-480c-9e88-8a7cb388f8e7
- agent-landing-zone, attempt 1: https://argusic.com/run/8c255909-4f2c-4fae-aaa3-bb0bf1b2f330

## The project's own tests failed

The project's test suite stopped with failures on the clean machine.

Example runs:

- 500-AI-Agents-Projects, attempt 1: https://argusic.com/run/230540eb-50de-4c61-ba6a-419e3094649b
- Acode, attempt 1: https://argusic.com/run/f12291ec-ba07-4e6f-9bd1-af099631ebd1
- action, attempt 1: https://argusic.com/run/5e4717b2-00cb-4af4-901c-1e3d5ffd8fb2

## Expected file or data not present

A file, build output or data set the instructions rely on was not there.

Example runs:

- agent-toolkit-for-aws, attempt 1: https://argusic.com/run/273a9e50-3438-4fbc-89f0-ccea6890f0ee
- ai-job-search, attempt 3: https://argusic.com/run/ea1709f1-2bef-47f0-ac95-92e5e5261b5a
- ai-moive-studio, attempt 1: https://argusic.com/run/3b920d5a-07fe-4be4-b8bd-ac56965ab347

## Error inside the project's code

The project itself raised an error while running.

Example runs:

- 500-AI-Agents-Projects, attempt 1: https://argusic.com/run/230540eb-50de-4c61-ba6a-419e3094649b
- agentset, attempt 2: https://argusic.com/run/0891f4ce-3494-4a09-bce4-0f6d666394fd
- agentsilex, attempt 2: https://argusic.com/run/e49bed62-78c5-4635-8bbd-cf188ec27213

## Other

Error lines that fit none of the groups above.

Example runs:

- 0ad, attempt 2: https://argusic.com/run/a3f8b8d5-9983-4188-9476-ad481c6956eb
- 4gaBoards, attempt 1: https://argusic.com/run/0a378b5b-de92-4e0a-b039-d56d6bd9e645
- 500-AI-Agents-Projects, attempt 1: https://argusic.com/run/230540eb-50de-4c61-ba6a-419e3094649b
