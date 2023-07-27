# Brand Strategist Positioning Statement Creator

Leverage the AI-powered Brand Strategist Positioning Statement Creator app to craft tailored, high-quality content. Define variables to generate statements emphasizing the unique value of a Brand Strategist within the Brand Consultancies sector. Discover detailed insights like target market, value proposition, and competitive edge. The output is not just a general position description, but a thorough portrayal of the role, designed to highlight its unique attributes and value in a competitive industry.

To run this app online: [Brand Strategist Positioning Statement Creator Online](https://hero.page/app/brand-strategist-positioning-statement-creator-ai-powered-brand-strategist-profiler/sfS2NGV8TFcjEdMNNzuz)

[![Run Brand Strategist Positioning Statement Creator Online](/assets/run.svg)](https://hero.page/app/brand-strategist-positioning-statement-creator-ai-powered-brand-strategist-profiler/sfS2NGV8TFcjEdMNNzuz)

To learn more about AI Apps for Brand Strategist use-cases in the Brand Consultancies industry, read [How to Innovate Brand Strategy with AI Workflow Apps](https://hero.page/blog/ai/brand-consultancies/how-to-innovate-brand-strategy-with-ai-workflow-apps/170763)

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
npx hero run ./brand_strategist_positioning_statement_creator.heroml
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
hero run ./brand_strategist_positioning_statement_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./brand_strategist_positioning_statement_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./brand_strategist_positioning_statement_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./brand_strategist_positioning_statement_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Brand Strategist Positioning Statement Creator
```
Your task is to write a "Product Positioning Statement" for the "Brand Consultancies" industry, specifically for a "Brand Strategist". 

Let's start by creating an engaging, yet informative introduction about the product. The description should capture the essence of the product and its unique selling proposition.

Here's some more context about the Product Positioning Statement:
Product Description: {{product_description}}
Target Market: {{target_market}}
Value Proposition: {{value_proposition}}
Competitive Difference: {{competitive_difference}}

->>>>

Let's move on to the next step with our introduction at hand:

Introduction:
{{step_1}}

Now, identify and define the target market, highlighting its demographic and psychographic characteristics. This section will help match the product's unique features with the needs of the target market.

->>>>

Let's review what we have so far with the product introduction and market context:

Introduction:
{{step_1}}

Target market:
{{step_2}}

Next, explain your product’s unique value with respect to how it solves the pain points or enhances the lives of the defined target market. Remember, the value proposition should not be generic, but contextually aligned to the Brand Consultancy industry.

->>>>

Let's progress further. We have the product introduction, market context, and its value proposition:

Introduction:
{{step_1}}

Target market:
{{step_2}}

Value proposition:
{{step_3}}

Now, delve into a detailed comparison on how your product stands out from your competitors in the brand consultancy industry. This will help to define the unique space your product holds in the industry landscape.


```

