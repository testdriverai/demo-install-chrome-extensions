![TestDriver.ai](https://github.com/dashcamio/testdriver/assets/318295/2a0ad981-8504-46f0-ad97-60cb6c26f1e7)

# Using TestDriver to Install Chrome Extensions

See [TestDriver Quickstart](https://docs.testdriver.ai/overview/quickstart)

---

**What is TestDriver?**

Next generation autonomous AI agent for end-to-end testing of web & desktop

[Website](https://testdriver.ai) | [Docs](https://docs.testdriver.ai) | [GitHub Action](https://github.com/marketplace/actions/testdriver-ai) | [Join our Discord](https://discord.gg/a8Cq739VWn)

---

## Setup

First, [fork this repository](https://github.com/testdriverai/quickstart-web/fork).

Next, [create a GitHub secret](https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/store-information-in-variables#creating-configuration-variables-for-a-repository) named `TESTDRIVER_API_KEY` using your API key from the testdriver dashboard.

> TestDriver is more fun with an API key. [Get an API key by starting a trial here](https://testdriver.ai/pricing).

In the forked repository, [add a GitHub variable](https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/store-information-in-variables#creating-configuration-variables-for-an-environment) named `TD_EXTENSION_NAME` . The value should be name of the extension you want to add. This is optional (e.g., `ColorZilla`).

## Installing a Chrome extension

- Run the `/testdriver/chrome_extension.yaml` test by performing:

```bash
> testdriverai run testdriver/chrome_extension.yaml
```

- or deploy the test and use the GitHub Action
