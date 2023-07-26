# AI AgTech Product Management Analyzer

AI AgTech Product Management Analyzer is a smart tool that uses AI capabilities to generate a customized Market Analysis Report. Specifically tailored for Product Managers in the AgTech industry, the app enables users to pinpoint variables, delivering high-quality insights covering target markets, product portfolios, competitors, trends, opportunities and risks. The comprehensive and targeted information equips users with strategic intel for effective product development, positioning, and marketing, enhancing overall decision-making in AgTech.

To run this app online: [AI AgTech Product Management Analyzer Online](https://hero.page/app/ai-agtech-product-management-analyzer-tailored-agtech-market-analysis/76CwC1r15kzq6VKQ0Eg5)

To learn more about AI Apps for Product Manager use-cases in the Agricultural Technology industry, read [How to Elevate AgTech with AI for Product Roadmap and Market Analysis](https://hero.page/blog/ai/agricultural-technology/how-to-elevate-agtech-with-ai-for-product-roadmap-and-market-analysis/170723)

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
npx hero run ./ai_agtech_product_management_analyzer.heroml
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
hero run ./ai_agtech_product_management_analyzer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ai_agtech_product_management_analyzer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ai_agtech_product_management_analyzer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ai_agtech_product_management_analyzer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for AI AgTech Product Management Analyzer
```
Your task is to write a "Market Analysis Report" for the "Agricultural Technology" industry, specifically for a "Product Manager". 

Let's begin with an executive summary that provides an overview of the market situation in the Agricultural Technology industry.

Here's some more context about the Market Analysis Report:
Market Overview: {{market_overview}}
Industry Context: {{industry_context}}
Current Market: {{current_market}}
Target Market: {{target_market}}
Product Analysis: {{product_analysis}}
Competition Analysis: {{competition_analysis}}
Market Trends: {{market_trends}}
Opportunities Challenges: {{opportunities_challenges}}
Strategy Recommendation: {{strategy_recommendation}}

->>>>

We have our executive summary for the Market Analysis Report:

Executive Summary:
{{step_1}}

Next, we'll create an introduction that provides contextual information about the Agricultural Technology industry and details the objectives of the market analysis.

->>>>

We now have both the executive summary and introduction for our report:

Executive Summary: 
{{step_1}}

Introduction:
{{step_2}}

Moving on, let's discuss the current market condition, identifying key players, market share, market growth, and segmentation.

->>>>

So far, we've covered the executive summary, introduction, and current market condition in our report:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Current Market Condition:
{{step_3}}

Now, let's identify the characteristics of the target market, including specific behaviours and preferences unique to the Agricultural Technology industry.

->>>>

So far, we have identified the target market for our report:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Current Market Condition:
{{step_3}}

Target Market:
{{step_4}}

Next, in the product analysis section, provide detailed information about the current product portfolio, performance, pricing strategy, and how it aligns with overall company goals and vision.

->>>>

The product analysis has been added to our report:

Current Market Condition:
{{step_3}}

Target Market:
{{step_4}}

Product Analysis:
{{step_5}}

Let's proceed with an analysis of the competition in the Agricultural Technology field, addressing their strengths, weaknesses, product offerings, market strategies, and other important factors.

->>>>

With the competition analysis, our report has the following sections:

Target Market:
{{step_4}}

Product Analysis:
{{step_5}}

Competition Analysis:
{{step_6}}

Next, let's explore both global and local market trends and how they impact the specific area of product management in the Agricultural Technology industry.

->>>>

Now, our report includes market trends:

Product Analysis:
{{step_5}}

Competition Analysis:
{{step_6}}

Market Trends:
{{step_7}}

Now, let's conclude the report with a section on opportunities and challenges, highlighting potential areas of growth and risks within the market, with a specific focus on their implications for product management.


```

