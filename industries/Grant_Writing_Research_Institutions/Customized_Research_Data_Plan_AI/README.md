# Customized Research Data Plan AI

Explore the power of AI with our app, Customized Research Data Plan AI. Tailored for industry-specific needs, this tool allows researchers to specify variables and receive comprehensive data management plans. Focused on the Grant Writing - Research Institutions industry, it covers data collection, documentation, storage, protection, access, sharing, and preservation. The output is elaborate, employing relevant terms, and emphasizes on proper data management's importance within the scientific community. The unique aspect is its specificity and practical usefulness for the intended audience.

To run this app online: [Customized Research Data Plan AI Online](https://hero.page/app/customized-research-data-plan-ai-industry-specific-research-data-management/KYbhxddioeXFG1fbgv9i)

[![Run Customized Research Data Plan AI Online](/assets/run.svg)](https://hero.page/app/customized-research-data-plan-ai-industry-specific-research-data-management/KYbhxddioeXFG1fbgv9i)

To learn more about AI Apps for Researcher use-cases in the Grant Writing - Research Institutions industry, read [How to Transform Grant Writing with AI: Methodology, Results, Data Plans](https://hero.page/blog/ai/grant-writing-research-institutions/how-to-transform-grant-writing-with-ai:-methodology-results-data-plans/170930)

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
npx hero run ./customized_research_data_plan_ai.heroml
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
hero run ./customized_research_data_plan_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./customized_research_data_plan_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./customized_research_data_plan_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./customized_research_data_plan_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

