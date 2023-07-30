# Comprehensive Hotel Review with Staff Insights

Examine your hotel service with Comprehensive Hotel Review with Staff Insights app. This AI-powered platform helps you create specialized reviews by inputting variables in prompts, crafting a holistic analysis of your hotel service. It provides general overviews, specific guest experiences reviews, detailed evaluations of diverse service areas, and even in-house employee feedback. Its uniqueness lies in considering employee retrospection, an overlooked yet vital source of insights. Balancing customer and employee viewpoints helps identify hidden service delivery issues, contributing to effective service improvement strategies.

To run this app online: [Comprehensive Hotel Review with Staff Insights Online](https://hero.page/app/comprehensive-hotel-review-with-staff-insights-ai-powered-staff-insights-for-hotels/L9xLAKhRfc6KuJySqO4o)

[![Run Comprehensive Hotel Review with Staff Insights Online](/assets/run.svg)](https://hero.page/app/comprehensive-hotel-review-with-staff-insights-ai-powered-staff-insights-for-hotels/L9xLAKhRfc6KuJySqO4o)

To learn more about AI Apps for Hotel Manager use-cases in the Hospitality & Tourism industry, read [How to Elevate Guest Experience with AI Hotel Descriptions and Reviews](https://hero.page/blog/ai/hospitality-and-tourism/how-to-elevate-guest-experience-with-ai-hotel-descriptions-and-reviews/170982)

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
npx hero run ./comprehensive_hotel_review_with_staff_insights.heroml
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
hero run ./comprehensive_hotel_review_with_staff_insights.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./comprehensive_hotel_review_with_staff_insights.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./comprehensive_hotel_review_with_staff_insights.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./comprehensive_hotel_review_with_staff_insights.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

