# Performance Report Builder for Analysts

Experience precision in performance reporting with the Performance Report Builder for Analysts app. Tailored for Digital Marketing Analysts, it allows you to define variables, leveraging AI to generate comprehensive, tailored reports. It illuminates performance metrics, reveals trends, analyses customer responses, and studies ROI across campaigns and market channels. It also offers actionable insights, crucial findings, and strategic recommendations for future endeavors. Ideal for strategic planning, it's a game-changer in the digital marketing industry.

To run this app online: [Performance Report Builder for Analysts Online](https://hero.page/app/performance-report-builder-for-analysts-tailored-analytics-for-digital-marketing/xeuEw87EeyWfGTY7z6UG)

[![Run Performance Report Builder for Analysts Online](/assets/run.svg)](https://hero.page/app/performance-report-builder-for-analysts-tailored-analytics-for-digital-marketing/xeuEw87EeyWfGTY7z6UG)

To learn more about AI Apps for Data Analyst use-cases in the Digital Marketing Agencies industry, read [How to Streamline Performance Reports, Data Analysis and KPI Reviews with AI Tools in Digital Marketing](https://hero.page/blog/ai/digital-marketing-agencies/how-to-streamline-performance-reports-data-analysis-and-kpi-reviews-with-ai-tools-in-digital-marketing/170840)

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
npx hero run ./performance_report_builder_for_analysts.heroml
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
hero run ./performance_report_builder_for_analysts.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./performance_report_builder_for_analysts.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./performance_report_builder_for_analysts.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./performance_report_builder_for_analysts.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

