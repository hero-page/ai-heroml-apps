# Automotive Product Plan Generator

The Automotive Product Plan Generator is a strategic automotive product development AI. Guided by the user's input, it incorporates a range of variables to create a comprehensive product development plan, specifically tailored for the automotive industry. The intuitive AI crafts a detailed analysis including an executive summary, market analysis, product description, innovation highlights, development roadmap, go-to-market strategy, and a financial projection. Its intricate focus on the automotive field helps deliver unique solutions to fill gaps or address problems in the industry, thus offering customized, high-quality content.

To run this app online: [Automotive Product Plan Generator Online](https://hero.page/app/automotive-product-plan-generator-strategic-automotive-product-development-ai/CZZJmA1OUhse4qyATG1Q)

[![Run Automotive Product Plan Generator Online](/assets/run.svg)](https://hero.page/app/automotive-product-plan-generator-strategic-automotive-product-development-ai/CZZJmA1OUhse4qyATG1Q)

To learn more about AI Apps for Product Manager use-cases in the Automotive Product Marketing industry, read [How to Refine Automotive Product Marketing with AI Tools](https://hero.page/blog/ai/automotive-product-marketing/how-to-refine-automotive-product-marketing-with-ai-tools/170747)

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
npx hero run ./automotive_product_plan_generator.heroml
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
hero run ./automotive_product_plan_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./automotive_product_plan_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./automotive_product_plan_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./automotive_product_plan_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Automotive Product Plan Generator
```
Your task is to write a "Product Development Plan" for the "Automotive Product Marketing" industry, specifically for a "Product Manager". 

Firstly, generate an executive summary for this product. The summary should offer an overview of the intended functionality of the product and the projected market space.

Here's some more context about the Product Development Plan:
Product Overview: {{product_overview}}
Market Analysis: {{market_analysis}}
Product Description: {{product_description}}
Tech Aspects: {{tech_aspects}}
Development Roadmap: {{development_roadmap}}

->>>>

We have started our Product Development Plan with an executive summary:

Executive Summary:
{{step_1}}

Now, conduct a detailed market analysis. Explain the situational context for this product, which includes an assessment of the overall market size, the potential target customer demographic, trends influencing demand, and the identification of direct and indirect competitors.

->>>>

Our Product Development Plan includes an executive summary and a market analysis:

Executive Summary:
{{step_1}}

Market Analysis:
{{step_2}}

Next, define the product. Specify its uses, features, and proposed specifications, and make it clear how it fulfills a distinct need within the market.

->>>>

For our Product Development Plan, we have an executive summary, market analysis, and a detailed product definition:

Executive Summary:
{{step_1}}

Market Analysis:
{{step_2}}

Product Definition:
{{step_3}}

Moving forward, write about the technology or innovation aspects of this product. Discuss the technological features of this product and how they address the industry's and customers' needs.

->>>>

In the Product Development Plan, we have defined the product and provided its technological aspects:

Product Definition:
{{step_3}}

Technological Aspects:
{{step_4}}

Now, let's create a product development roadmap. Include all stages of development starting from concept generation to testing, launch, and post-launch improvements. Be sure to address key milestones, anticipate possible challenges, and come up with contingency plans.

->>>>

So far in the Product Development Plan, we have discussed the technological aspects of the product and laid out a development roadmap:

Technological Aspects:
{{step_4}}

Development Roadmap:
{{step_5}}

Next, write in detail about your go-to-market strategy. This should include distribution, pricing, sales, marketing, and service strategies. The plan should be highly specific considering the competitive nature of the automotive product marketing industry.


```

