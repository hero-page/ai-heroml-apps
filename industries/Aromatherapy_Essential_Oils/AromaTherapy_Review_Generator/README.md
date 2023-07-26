# AromaTherapy Review Generator

Explore the world of aromatherapy with AromaTherapy Review Generator, your AI-powered expert. Tailor your prompts to generate a detailed, high-caliber review of aromatherapy or essential oil products. AI insight brings you a comprehensive look at key features, personal experience, quality, suitability and potential risks, delivering an unbiased verdict on the product's worth. Go beyond basics thanks to our unique ability, producing in-depth reviews that delve into personal experiences and wellness routine compatibility.

To run this app online: [AromaTherapy Review Generator Online](https://hero.page/app/aromatherapy-review-generator-ai-powered-aromatherapy-review-expert/4RZZQHw4YXNrGhYmDcdh)

[![Run AromaTherapy Review Generator Online](/assets/run.svg)](https://hero.page/app/aromatherapy-review-generator-ai-powered-aromatherapy-review-expert/4RZZQHw4YXNrGhYmDcdh)

To learn more about AI Apps for Wellness Blogger use-cases in the Aromatherapy & Essential Oils industry, read [How to Enrich Your Aromatherapy Journey with AI Solutions](https://hero.page/blog/ai/aromatherapy-and-essential-oils/how-to-enrich-your-aromatherapy-journey-with-ai-solutions/170730)

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
npx hero run ./aromatherapy_review_generator.heroml
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
hero run ./aromatherapy_review_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./aromatherapy_review_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./aromatherapy_review_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./aromatherapy_review_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for AromaTherapy Review Generator
```
Your task is to write a "Product Review" for the "Aromatherapy & Essential Oils" industry, specifically for a "Wellness Blogger". Consider that the readers value sourced, realistic information and want to genuinely understand the product's effects. 

Let's start by writing a captivating introduction about the product: {{product_name}}. The introduction should grab the reader's attention and briefly explain why they might need the product.

Here's some more context about the Product Review:
Product Name: {{product_name}}
Reasons For Choose: {{reasons_for_choose}}
Usage Process: {{usage_process}}

->>>>

We have started our "Product Review" with a captivating introduction about {{product_name}}:

Introduction:
{{step_1}}

Now, we need to define what the product is. Include in this section basic details like the product name: {{product_name}}, its manufacturer, and the unique features that distinguish it from other products in the same category.

->>>>

After defining the product, we have:

Introduction:
{{step_1}}

Product Definition:
{{step_2}}

Next, we should outline why this product was chosen for review. The reasons could range from its popularity, its unique features, or the health benefits it supposedly provides.

->>>>

As per the explanation given, our product review has

Product Definition:
{{step_2}}

Reasons for Choosing:
{{step_3}}

Let's move on to present how the product was used, its positive aspects, and those features that could be improved. This section needs to be relatable and authentic, reinforcing the wellness aspect.

->>>>

Thus far, we have shared the reasons for choosing the product and how it was used:
    
Reasons for Choosing:
{{step_3}}

Usage and Evaluation:
{{step_4}}

Next, it's time to critically assess the product quality. Discuss the scent profile, potency, packaging and any noticeable effects of {{product_name}}.

->>>>

Now, we have both an evaluation based on personal usage and a critical quality assessment of {{product_name}}:

Usage and Evaluation:
{{step_4}}

Product Quality Assessment:
{{step_5}}

Now, let's discuss how the product aligns with your wellness routine or different wellness trends. This should offer your readers insights into the suitability of the product for different aromatherapy practices.

->>>>

Having assessed the product and its usage, we now have a discussion on its alignment with wellness routines or trends:

Product Quality Assessment:
{{step_5}}

Wellness Suitability Discussion:
{{step_6}}

Discuss any potential risks or side effects observed or researched related to the use of {{product_name}}, this is key information for wellness bloggers to share with their audience.

->>>>

Having understood the suitability of the product for wellness routines, we have described any potential risks or side effects:

Wellness Suitability Discussion:
{{step_6}}

Product Risks and Side-Effects:
{{step_7}}

Let's wrap up the review, offering a succinct summary of thoughts on the product: {{product_name}}. This should answer any pertinent question a potential buyer might have about the product.

->>>>

After listing potential risks and side effects, we have a wrap-up of the review:

Product Risks and Side-Effects:
{{step_7}}

Review Wrap-Up:
{{step_8}}

Finally, state whether or not the product, {{product_name}}, would be recommended to others. 


```

