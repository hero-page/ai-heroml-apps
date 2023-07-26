# Automotive Marketing Competitive Analysis AI

Automotive Marketing Competitive Analysis AI app delivers detailed reports compiled by AI, offering customized automotive analysis. Users specify variables and get comprehensive, high-quality content. Features like executive summary, product and market overview, competitor and product analysis, trending industry insights, and strategic marketing recommendations are included. The uniqueness lies in its use of strategic tools (PESTEL, SWOT) and tailored results for automotive product marketers. Suitable for robust strategy building.

To run this app online: [Automotive Marketing Competitive Analysis AI Online](https://hero.page/app/automotive-marketing-competitive-analysis-ai-ai-powered-custom-automotive-analysis/nUz6Q3WWSk3h2vrm8LhT)

[![Run Automotive Marketing Competitive Analysis AI Online](/assets/run.svg)](https://hero.page/app/automotive-marketing-competitive-analysis-ai-ai-powered-custom-automotive-analysis/nUz6Q3WWSk3h2vrm8LhT)

To learn more about AI Apps for Product Marketer use-cases in the Automotive Product Marketing industry, read [How to Elevate Automotive Marketing with AI for Specs, Email, Analysis](https://hero.page/blog/ai/automotive-product-marketing/how-to-elevate-automotive-marketing-with-ai-for-specs-email-analysis/170745)

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
npx hero run ./automotive_marketing_competitive_analysis_ai.heroml
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
hero run ./automotive_marketing_competitive_analysis_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./automotive_marketing_competitive_analysis_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./automotive_marketing_competitive_analysis_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./automotive_marketing_competitive_analysis_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Automotive Marketing Competitive Analysis AI
```
Your task is to write a "Competitive Analysis" for the "Automotive Product Marketing" industry for a "Product Marketer". 

Start with the creation of an executive summary, which provides a brief overview of the content that the report will include.

Here's some more context about the Competitive Analysis:
Executive Summary: {{executive_summary}}
Product Background: {{product_background}}
Marketer Requirements: {{marketer_requirements}}
Purpose: {{purpose}}
Competitor Products: {{competitor_products}}
Competitor Marketing Strategies: {{competitor_marketing_strategies}}
Product Vs Competitors: {{product_vs_competitors}}
Recommendations: {{recommendations}}
Conclusion: {{conclusion}}

->>>>

With our executive summary at hand:

Executive Summary:
{{step_1}}

It's time to write an introduction that explains the background of the automotive product to be marketed, the requirements of the product marketer, and the purpose of this report.

->>>>

Now our report has an executive summary and an introduction:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Next, identify the key competitors and their products in the automotive industry. Provide an in-depth analysis of each competitor's product, focusing on factors such as price, performance, unique selling points, market share, customer base, and user reviews.

->>>>

We have an executive summary, introduction, and analysis of competitors' products for our report:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Competitor Products Analysis:
{{step_3}}

Let's proceed by analyzing the marketing strategies of the competitors' products. Consider aspects like distribution channels, advertising methods, brand positioning, pricing strategies, and customer relationship management practices.

->>>>

Moving forward in our report, we have analyzed the competitor's marketing strategies:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Competitor Products Analysis:
{{step_3}}

Competitor Marketing Strategies Analysis:
{{step_4}}

Now, examine the external environment of the market using a PESTEL analysis model, which covers the political, economic, social, technological, environmental, and legal factors impacting the automotive industry.

->>>>

We have further expanded our report with a PESTEL analysis:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Competitor Products Analysis:
{{step_3}}

Competitor Marketing Strategies Analysis:
{{step_4}}

PESTEL Analysis:
{{step_5}}

Next, evaluate the competitive positioning of the product marketer's product in relation to the competitors' products. Discuss strengths, weaknesses, opportunities, and threats (SWOT analysis).

->>>>

After our analysis, we now have a SWOT analysis:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Competitor Products Analysis:
{{step_3}}

Competitor Marketing Strategies Analysis:
{{step_4}}

PESTEL Analysis:
{{step_5}}

SWOT Analysis:
{{step_6}}

Further elaborate the analysis by suggesting industry-specific factors related to automotive product marketing such as technology trends, environmental regulations, fuel economy standards, or electric vehicle adoption rates.

->>>>

With the inclusion of industry-specific factors, our report is becoming increasingly comprehensive:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Competitor Products Analysis:
{{step_3}}

Competitor Marketing Strategies Analysis:
{{step_4}}

PESTEL Analysis:
{{step_5}}

SWOT Analysis:
{{step_6}}

Industry-Specific Factors:
{{step_7}}

Let's add a comparative discussion on how the product marketer's product stands against each competitor's product, considering its competitive advantages and areas for improvement.

->>>>

Now, our report includes a comparison of the product marketer's product against competitor products:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Competitor Products Analysis:
{{step_3}}

Competitor Marketing Strategies Analysis:
{{step_4}}

PESTEL Analysis:
{{step_5}}

SWOT Analysis:
{{step_6}}

Industry-Specific Factors:
{{step_7}}

Product Vs Competitor Products:
{{step_8}}

Let's build on this analysis and recommend action plans for the product marketing strategy based on the collected insights. These can be ways to exploit the competitors' weaknesses, buffer against threats, capitalize on opportunities, or improve the product's weaknesses.

->>>>

Incorporating our suggested actions, our competitive analysis now comprises:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Competitor Products Analysis:
{{step_3}}

Competitor Marketing Strategies Analysis:
{{step_4}}

PESTEL Analysis:
{{step_5}}

SWOT Analysis:
{{step_6}}

Industry-Specific Factors:
{{step_7}}

Product Vs Competitor Products:
{{step_8}}

Recommended Actions:
{{step_9}}

Finally, let's tie it all together with a conclusion that encapsulates the main points of the analysis, restates its purpose, and proves its relevance and utility for the product marketer.


```

