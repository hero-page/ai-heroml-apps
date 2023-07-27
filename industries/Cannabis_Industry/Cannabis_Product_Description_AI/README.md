# Cannabis Product Description AI

Explore the power of AI with Cannabis Product Description AI, an advanced description generator specifically designed for cannabis products. Users can tailor prompts to create customized, high-quality content that meets industry requirements. Every output is rich in detail including unique selling points, strain type, physical and mental effects, medicinal benefits, and more. The app also ensures that all descriptions comply with regulations, making it a reliable tool for dispensary managers. Experience a uniquely efficient way of developing cannabis product descriptions.

To run this app online: [Cannabis Product Description AI Online](https://hero.page/app/cannabis-product-description-ai-ai-powered-cannabis-description-generator/CWYwialVrFQ8vFyohUai)

[![Run Cannabis Product Description AI Online](/assets/run.svg)](https://hero.page/app/cannabis-product-description-ai-ai-powered-cannabis-description-generator/CWYwialVrFQ8vFyohUai)

To learn more about AI Apps for Dispensary Manager use-cases in the Cannabis Industry industry, read [How to Amplify Cannabis Marketing with AI Tools](https://hero.page/blog/ai/cannabis-industry/how-to-amplify-cannabis-marketing-with-ai-tools/170770)

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
npx hero run ./cannabis_product_description_ai.heroml
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
hero run ./cannabis_product_description_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./cannabis_product_description_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./cannabis_product_description_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./cannabis_product_description_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Cannabis Product Description AI
```
Your task is to write a "Product Description" for the "Cannabis Industry" industry, specifically for a "Dispensary Manager". 

Let's start by an engaging introduction that captures the unique selling point of the product: {{product_unique_selling_point}}.

Here's some more context about the Product Description:
Product Unique Selling Point: {{product_unique_selling_point}}
Product Type: {{product_type}}
Product Characteristics: {{product_characteristics}}
Product Effects: {{product_effects}}
Medical Benefits: {{medical_benefits}}
Recommended Use: {{recommended_use}}
Product Pricing: {{product_pricing}}

->>>>

With the introduction of our product description, we have outlined the unique selling point:

Unique Selling Point:
{{step_1}}

Next, provide a brief overview about the strain or product type: {{product_type}}. This should be specific and detailed, covering the cannabis strain information or product function.

->>>>

With the unique selling point and a detailed strain or product information in place, we have:

Unique Selling Point:
{{step_1}}

Strain or Product Type Information:
{{step_2}}

Now, describe the basic characteristics of the item in question, including the appearance, color, texture, and scent: {{product_characteristics}}.

->>>>

So far for the product description, we have gathered information about its unique selling point, strain or product type, and now its basic characteristics:

Unique Selling Point:
{{step_1}}

Strain or Product Type Information:
{{step_2}}

Product Characteristics:
{{step_3}}

Proceed to describe the physical and mental effects to be expected from the product. This provides potential consumers with transparency and a clear outline of their potential experience: {{product_effects}}.

->>>>

For our product description, we have detailed the unique selling point, strain or product type, its characteristics, and now effects of usage:

Unique Selling Point:
{{step_1}}

Product Characteristics:
{{step_3}}

Product Effects:
{{step_4}}

After detailing the product's effects, it'll be imperative to add any medicinal benefits, if any. This could include relief from ailments or symptoms: {{medical_benefits}}.

->>>>

In our product description, we have defined the product's effects and medicinal benefits:

Product Effects:
{{step_4}}

Medicinal Benefits:
{{step_5}}

Let's include information on the recommended time of use (morning, afternoon, evening) and the right consumption method which enhances the product experience: {{recommended_use}}.

->>>>

So far in our product description, we have detailed the product's medicinal benefits along with recommended time of use and consumption method:

Medicinal Benefits:
{{step_5}}

Recommended Use and Consumption Method:
{{step_6}}

Finally, conclude the product description by imparting the pricing information and the available quantity: {{product_pricing}}. Make sure all provided information is accurate and compliant with all regulations.


```

