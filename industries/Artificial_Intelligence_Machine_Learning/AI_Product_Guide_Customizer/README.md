# AI Product Guide Customizer

AI Product Guide Customizer helps create tailored guides for Artificial Intelligence & Machine Learning Product Managers. With AI, it curates high-quality, custom content including product purpose, target audience, key features, user interface guide, troubleshooting guide, FAQS, product benefits, and support resources. Uniquely, it caters to specific industry needs, addressing challenges exclusive to AI & ML professionals.

To run this app online: [AI Product Guide Customizer Online](https://hero.page/app/ai-product-guide-customizer-custom-ai-product-management-guide/qZu1pOHQgfeBsynaH3BQ)

[![Run AI Product Guide Customizer Online](/assets/run.svg)](https://hero.page/app/ai-product-guide-customizer-custom-ai-product-management-guide/qZu1pOHQgfeBsynaH3BQ)

To learn more about AI Apps for Product Manager use-cases in the Artificial Intelligence & Machine Learning industry, read [How to Streamline AI Product Development with Essential Workflow Apps](https://hero.page/blog/ai/artificial-intelligence-and-machine-learning/how-to-streamline-ai-product-development-with-essential-workflow-apps/170733)

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
npx hero run ./ai_product_guide_customizer.heroml
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
hero run ./ai_product_guide_customizer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ai_product_guide_customizer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ai_product_guide_customizer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ai_product_guide_customizer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for AI Product Guide Customizer
```
Your task is to write a "User Guide" for the "Artificial Intelligence & Machine Learning" industry, specifically for a "Product Manager". 
Let's start with an introduction that defines the purpose of the artificial intelligence or machine learning product: {{product_purpose}}.

Here's some more context about the User Guide:
Product Purpose: {{product_purpose}}
Audience: {{audience}}
Product Features: {{product_features}}
Interface Usability: {{interface_usability}}
Integration: {{integration}}
Troubleshooting: {{troubleshooting}}
FAQs: {{FAQs}}
Product Benefits: {{product_benefits}}
Support Resources: {{support_resources}}

->>>>

We have a "User Guide" that's starting to take shape, and our introduction section is:

Introduction (Product Purpose):
{{step_1}}

Next, write down the target audience section, explaining who the primary users of the product are: {{audience}}.

->>>>

Our "User Guide" now has an introduction and a target audience section:

Introduction (Product Purpose):
{{step_1}}

Target Audience:
{{step_2}}

Moving forward, create a section on the product overview. Explain what the AI or ML product does and its core features: {{product_features}}.

->>>>

In the "User Guide", we have now defined the introduction, the target audience, and the product overview:

Introduction (Product Purpose):
{{step_1}}

Target Audience:
{{step_2}}

Product Overview:
{{step_3}}

Next, include a user-interface guide. Detail how to use the product's interface for maximum efficiency: {{interface_usability}}.

->>>>

For the "User Guide", we now have information on the introduction, target audience, product overview, and the user-interface guide:

Introduction (Product Purpose):
{{step_1}}

Target Audience:
{{step_2}}

Product Overview:
{{step_3}}

User-Interface Guide:
{{step_4}}

Continue with the guide by describing how to integrate the product into the existing workflows or systems, if applicable: {{integration}}.

->>>>

In our "User Guide" so far, we have information about the introduction, target audience, product overview, user-interface guide, and product integration:

Introduction (Product Purpose):
{{step_1}}

Target Audience:
{{step_2}}

Product Overview:
{{step_3}}

User-Interface Guide:
{{step_4}}

Product Integration:
{{step_5}}

Now, include a troubleshooting guide that addresses common issues and solutions a user may face with the product: {{troubleshooting}}.

->>>>

So far, the "User Guide" includes the introduction, target audience, product overview, user-interface guide, product integration, and troubleshooting guide:

Introduction (Product Purpose):
{{step_1}}

Target Audience:
{{step_2}}

Product Overview:
{{step_3}}

User-Interface Guide:
{{step_4}}

Product Integration:
{{step_5}}

Troubleshooting Guide:
{{step_6}}

Provide a comprehensive FAQ segment, focusing on regular queries that are related to the features, integration, and trouble-shooting: {{FAQs}}.

->>>>

In the "User Guide" so far, we have completed the introduction, target audience, product overview, user-interface guide, product integration, troubleshooting guide, and the FAQ section:

Introduction (Product Purpose):
{{step_1}}

Target Audience:
{{step_2}}

Product Overview:
{{step_3}}

User-Interface Guide:
{{step_4}}

Product Integration:
{{step_5}}

Troubleshooting Guide:
{{step_6}}

FAQs:
{{step_7}}

Reinforce the benefits and unique selling proposition of the AI/ML productin the conclusion: {{product_benefits}}.


```

