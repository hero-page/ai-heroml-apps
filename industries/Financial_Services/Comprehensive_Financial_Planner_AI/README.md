# Comprehensive Financial Planner AI

Harness the power of AI with Comprehensive Financial Planner AI. Input variables to generate a custom-tailored, comprehensive financial plan for your clients. The AI crafts unique, high-quality content, including an executive summary, financial status snapshot, a detailed analysis of income, expenses, assets, and liabilities, personalized investment strategy, retirement planning, insurance assessment, and a tax strategy. Above all, it chucks out an action plan towards the achievement of predefined financial goals, ensuring the information remains clear, informative, and accessible, making it an ultimate financial planning tool.

To run this app online: [Comprehensive Financial Planner AI Online](https://hero.page/app/comprehensive-financial-planner-ai-ai-powered-customized-financial-planning/7FXiFCYXCDAsxz9QSOa2)

[![Run Comprehensive Financial Planner AI Online](/assets/run.svg)](https://hero.page/app/comprehensive-financial-planner-ai-ai-powered-customized-financial-planning/7FXiFCYXCDAsxz9QSOa2)

To learn more about AI Apps for Financial Planner use-cases in the Financial Services industry, read [How to Enhance Financial Planning with AI-Driven Investment Tools](https://hero.page/blog/ai/financial-services/how-to-enhance-financial-planning-with-ai-driven-investment-tools/170877)

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
npx hero run ./comprehensive_financial_planner_ai.heroml
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
hero run ./comprehensive_financial_planner_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./comprehensive_financial_planner_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./comprehensive_financial_planner_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./comprehensive_financial_planner_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

