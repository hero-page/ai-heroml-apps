# Email Campaign Performance Analyzer

Email Campaign Performance Analyzer is an exceptional app for detailed marketing analytics. With the power of AI, it lets users specify variables and generates custom, high-quality content. It provides comprehensive reports on email marketing campaign performance, including a summary, KPI analyses, campaign data such as sent emails, open rate, click-through rate, conversion rate, and unsubscribe rate. It aids in understanding trends, potential correlations, and behavior patterns. Apart from raw data, a thoughtful interpretation through demographic breakdowns and audience engagement reports provide nuanced insights for strategic planning of future campaigns.

To run this app online: [Email Campaign Performance Analyzer Online](https://hero.page/app/email-campaign-performance-analyzer-comprehensive-email-marketing-analytics/6VajBO2ibiBaVNZVq6zd)

[![Run Email Campaign Performance Analyzer Online](/assets/run.svg)](https://hero.page/app/email-campaign-performance-analyzer-comprehensive-email-marketing-analytics/6VajBO2ibiBaVNZVq6zd)

To learn more about AI Apps for Data Analyst use-cases in the Email Marketing Services industry, read [How to Elevate Email Marketing with AI-Driven Data Analysis](https://hero.page/blog/ai/email-marketing-services/how-to-elevate-email-marketing-with-ai-driven-data-analysis/170857)

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
npx hero run ./email_campaign_performance_analyzer.heroml
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
hero run ./email_campaign_performance_analyzer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./email_campaign_performance_analyzer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./email_campaign_performance_analyzer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./email_campaign_performance_analyzer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

