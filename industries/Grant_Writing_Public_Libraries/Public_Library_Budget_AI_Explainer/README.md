# Public Library Budget AI Explainer

Public Library Budget AI Explainer is an AI-powered app that tailors complex budget explanations for public libraries. Users can customize variables for high-quality outputs, which offer comprehensive analysis of the proposed budget that aligns with the library's mission. Features include categorical budget breakdowns, in-depth justifications, highlighting significant financial changes, and providing industry-specific data, all proofread for clarity and accuracy. The app's standout feature is its detailed scrutiny of public library budgets, offering insights into how they further community growth and service provision.

To run this app online: [Public Library Budget AI Explainer Online](https://hero.page/app/public-library-budget-ai-explainer-ai-powered-public-library-budget-guide/fubRmCiHK7BuxIRG1dt6)

[![Run Public Library Budget AI Explainer Online](/assets/run.svg)](https://hero.page/app/public-library-budget-ai-explainer-ai-powered-public-library-budget-guide/fubRmCiHK7BuxIRG1dt6)

To learn more about AI Apps for Grant Writer use-cases in the Grant Writing - Public Libraries industry, read [How to Ace Library Grant Proposals with AI-Assisted Writing](https://hero.page/blog/ai/grant-writing-public-libraries/how-to-ace-library-grant-proposals-with-ai-assisted-writing/170927)

### What is HeroML?
HeroML is an AI Prompt Chain/Workflow interpreter for Apps built on https://hero.page 

To see other apps, visit the [Hero Apps](https://hero.page/apps) page or explore [AI Apps for all industries](https://hero.page/blog) in the blog section

For more documentation, visit [Hero docs, and learn about AI App Workflows](https://hero.page/tutorials/introduction-to-heroml)

Download [VSCode Syntax Highlighter Ext. here](https://marketplace.visualstudio.com/items?itemName=hero-page.heroml)

## Run with HeroCLI (Requires OpenAI Token)

#### Installation

To install the HeroML CLI tool, you need to have Node.js and npm (comes with Node.js) installed on your machine. If you don't have these, please install them first. 

Then, run the following command in your terminal:

```bash
npm install -g heroml
```

This will install the HeroML CLI tool globally on your system, allowing you to use the `hero` command from any directory.

If you don't want to install it globally, you can run:

```bash
npm install heroml
```

and use it like:

```bash
npx hero run ./public_library_budget_ai_explainer.heroml
```

We'll be using `hero run ...` in this tutorial for simplicity.

#### Configuration

Before using the HeroML CLI tool, you need to configure your OpenAI API key. 

Create a `heroconfig.json` file in your home directory with the following content:

```json
{
  "openaiApiKey": "your-openai-api-key"
}
```

Replace `"your-openai-api-key"` with your actual OpenAI API key.

#### Usage

To run a HeroML script, use the `run` command followed by the path to your script:

```bash
hero run ./public_library_budget_ai_explainer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./public_library_budget_ai_explainer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./public_library_budget_ai_explainer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./public_library_budget_ai_explainer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

