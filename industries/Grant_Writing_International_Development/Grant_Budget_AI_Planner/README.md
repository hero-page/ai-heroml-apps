# Grant Budget AI Planner

Discover the power of AI with Grant Budget AI Planner, a cutting-edge budgeting tool designed for professionals in the International Development industry. With the ability to specify variables, this app generates detailed, bespoke content, outlining a clearly structured grant budget that includes an executive summary, grant objectives, meticulously itemized costs, and a contingency plan, providing a complete financial overview. The app's unique aspect is its emphasis on a contingency plan with allocated funds, reflecting your organization's readiness to handle potential setbacks. This isn't just a budget; it illustrates your competency, efficiency, and preparedness for project management.

To run this app online: [Grant Budget AI Planner Online](https://hero.page/app/grant-budget-ai-planner-ai-powered-international-grant-planner/qJNhQ1MQnJ6qRYiLG3ew)

[![Run Grant Budget AI Planner Online](/assets/run.svg)](https://hero.page/app/grant-budget-ai-planner-ai-powered-international-grant-planner/qJNhQ1MQnJ6qRYiLG3ew)

To learn more about AI Apps for Grant Writer use-cases in the Grant Writing - International Development industry, read [How to Streamline International Development Proposals with AI Tools](https://hero.page/blog/ai/grant-writing-international-development/how-to-streamline-international-development-proposals-with-ai-tools/170921)

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
npx hero run ./grant_budget_ai_planner.heroml
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
hero run ./grant_budget_ai_planner.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./grant_budget_ai_planner.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./grant_budget_ai_planner.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./grant_budget_ai_planner.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

