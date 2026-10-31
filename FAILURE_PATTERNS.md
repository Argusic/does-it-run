# Failure patterns

What the clean machine printed when a project was installed and run, grouped by kind. Computed from 11078 observed error lines in 4880 valid runs of 3604 tested subjects (generated 2026-10-31).

A line is placed in the first group below whose rule it matches, in the order shown; anything else is "Other". The percentages are shares of all observed error lines.

| Pattern | Error lines | Share | Subjects affected |
|---|---|---|---|
| Port already in use | 12 | 0.1% | 10 |
| Permission denied | 104 | 0.9% | 95 |
| Missing system library or header | 564 | 5.1% | 348 |
| Tool, runtime or component not installed | 1833 | 16.5% | 1261 |
| Version mismatch | 1154 | 10.4% | 860 |
| Missing configuration or secret | 238 | 2.1% | 216 |
| Source or download problem | 133 | 1.2% | 117 |
| Network, timeout or service unreachable | 212 | 1.9% | 189 |
| Dependency install or resolution failed | 1327 | 12.0% | 978 |
| Build or compile step failed | 481 | 4.3% | 391 |
| The project's own tests failed | 1212 | 10.9% | 758 |
| Expected file or data not present | 163 | 1.5% | 149 |
| Error inside the project's code | 136 | 1.2% | 123 |
| Other | 3509 | 31.7% | 1734 |

## Port already in use

A second process wanted a port that was already taken.

Example runs:

- bramble, attempt 1: https://argusic.com/run/86fee78c-2eeb-46ef-b0ac-e79d42644964
- CaddyProxyManager, attempt 1: https://argusic.com/run/05414b07-cac1-4717-a638-70535be860c3
- express, attempt 2: https://argusic.com/run/4e43cf30-bc87-4838-8e48-9bc64db2f542

## Permission denied

The step needed rights the clean machine user does not have.

Example runs:

- agent-browser, attempt 1: https://argusic.com/run/5084027b-e339-48b7-8129-f7b2ed9cef9a
- agent-browser-cli, attempt 1: https://argusic.com/run/7afa98a3-8241-4f21-8f69-ff5adcf2854f
- agent-purge, attempt 1: https://argusic.com/run/b2372950-4bb7-4d1e-8c1a-9ea339b5fced

## Missing system library or header

A build or launch step needed a system package that was not installed.

Example runs:

- 0ad, attempt 2: https://argusic.com/run/19c34cdc-acd7-4d8f-ba3a-b6f02169729a
- actsasindexed, attempt 1: https://argusic.com/run/36daae6d-2ae3-42d9-b136-bf1252f43773
- addok, attempt 1: https://argusic.com/run/3ce89028-aef1-4fd5-840a-9a0c5bfebb20

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

- 1JPM, attempt 1: https://argusic.com/run/def113cd-8d61-4ecc-aeec-a9e8b915b0fa
- Acode, attempt 1: https://argusic.com/run/f12291ec-ba07-4e6f-9bd1-af099631ebd1
- across, attempt 1: https://argusic.com/run/958a29d8-b4cd-486c-9440-3ea46fa473bb

## Network, timeout or service unreachable

A request or a service call did not complete in time or was refused.

Example runs:

- 10xProductivity, attempt 1: https://argusic.com/run/c40f7bbe-deed-4d3a-8fbc-1f980835bd12
- a-stock-data, attempt 1: https://argusic.com/run/d7dc86f0-383f-42e0-bf4e-8d8dbc1a38fd
- Acode, attempt 1: https://argusic.com/run/f12291ec-ba07-4e6f-9bd1-af099631ebd1

## Dependency install or resolution failed

Installing or resolving the project's dependencies did not finish cleanly.

Example runs:

- 1JPM, attempt 1: https://argusic.com/run/def113cd-8d61-4ecc-aeec-a9e8b915b0fa
- 4gaBoards, attempt 1: https://argusic.com/run/0a378b5b-de92-4e0a-b039-d56d6bd9e645
- 500-AI-Agents-Projects, attempt 1: https://argusic.com/run/230540eb-50de-4c61-ba6a-419e3094649b

## Build or compile step failed

A build, compile or import step stopped with an error.

Example runs:

- 0ad, attempt 2: https://argusic.com/run/a3f8b8d5-9983-4188-9476-ad481c6956eb
- acl, attempt 1: https://argusic.com/run/5d5a6c5b-4a2c-480c-9e88-8a7cb388f8e7
- act, attempt 1: https://argusic.com/run/b2232403-8fee-4f2d-98b0-11a4e1aa752b

## The project's own tests failed

The project's test suite stopped with failures on the clean machine.

Example runs:

- 500-AI-Agents-Projects, attempt 1: https://argusic.com/run/230540eb-50de-4c61-ba6a-419e3094649b
- Acode, attempt 1: https://argusic.com/run/f12291ec-ba07-4e6f-9bd1-af099631ebd1
- act, attempt 1: https://argusic.com/run/b2232403-8fee-4f2d-98b0-11a4e1aa752b

## Expected file or data not present

A file, build output or data set the instructions rely on was not there.

Example runs:

- agent-purge, attempt 1: https://argusic.com/run/b2372950-4bb7-4d1e-8c1a-9ea339b5fced
- agent-toolkit-for-aws, attempt 1: https://argusic.com/run/273a9e50-3438-4fbc-89f0-ccea6890f0ee
- ai-job-search, attempt 3: https://argusic.com/run/ea1709f1-2bef-47f0-ac95-92e5e5261b5a

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
- 1JPM, attempt 1: https://argusic.com/run/def113cd-8d61-4ecc-aeec-a9e8b915b0fa
- 4gaBoards, attempt 1: https://argusic.com/run/0a378b5b-de92-4e0a-b039-d56d6bd9e645
