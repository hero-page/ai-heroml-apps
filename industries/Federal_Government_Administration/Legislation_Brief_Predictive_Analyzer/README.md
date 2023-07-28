# Legislation Brief Predictive Analyzer

Legislation Brief Predictive Analyzer app intelligently employs AI to meticulously analyze and predict legislative impacts. It enables users to input specific variables, generating relevant findings. Boasting features like comprehensive legislative analyses, it uncovers a law's background, key components, allies and adversaries, and potential effects. The standout feature is its unique ability to predict if a bill will pass, factoring in variables like political climate and public sentiment. This offers an unmatched depth of knowledge, proving an indispensable tool for policy analysts.

To run this app online: [Legislation Brief Predictive Analyzer Online](https://hero.page/app/legislation-brief-predictive-analyzer-ai-powered-legislative-impact-prediction/zhUHr09zyAE7dB6UHCQg)

[![Run Legislation Brief Predictive Analyzer Online](/assets/run.svg)](https://hero.page/app/legislation-brief-predictive-analyzer-ai-powered-legislative-impact-prediction/zhUHr09zyAE7dB6UHCQg)

To learn more about AI Apps for Policy Analyst use-cases in the Federal Government Administration industry, read [How to Enhance Policy Analysis with AI in Federal Government](https://hero.page/blog/ai/federal-government-administration/how-to-enhance-policy-analysis-with-ai-in-federal-government/170870)

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
npx hero run ./legislation_brief_predictive_analyzer.heroml
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
hero run ./legislation_brief_predictive_analyzer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./legislation_brief_predictive_analyzer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./legislation_brief_predictive_analyzer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./legislation_brief_predictive_analyzer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

