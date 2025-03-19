
![GmVQSYxbkAAaW8C(1)](https://github.com/user-attachments/assets/07fd9476-0661-4843-b1c6-92d2885dfcb7)

# E3Tech Integration tests

- We’re thrilled to share our investment in E3Tech, a company applying AI and operational excellence to industries where technology adoption has lagged, creating new opportunities for efficiency and growth.
Leading this vision is seasoned entrepreneur Rudy Adolf, who previously founded and successfully exited a leading investment advisory firm.

# BSC Chain ​​Proposal

- test_wallet = ""

## Smoke tests

- Should always be run on a freshly cloned project (i.e. no local changes)
- Building and installing is part of the test
- No configuration required
- To run: `pnpm run smokeTests`

## Integration tests

- You need to configure your .env file before running (currently at least `OPENAI_API_KEY` is required)
- How to use:
    1. Install project dependencies and build the project as described in top-level `README`
    2. To run all the tests: `pnpm run integrationTests`

## Integration test library

- For simplicity, integration tests are written in plain JavaScript (ESM)
- Currently this is just a "proof of concept" (single test), please reach out if you would like to contribute.

## Using in GitHub CI/CD

- Settings -> Secrets and variables -> Actions:
- Create an environment
- Add repository secret `OPENAI_API_KEY`
- Refer to https://docs.github.com/en/actions/security-for-github-actions/security-guides/using-secrets-in-github-actions for more information
