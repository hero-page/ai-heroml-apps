# Kids Art Supply Design Specifier

Perfect for creative minds, Kids Art Supply Design Specifier uses AI to deliver a custom design blueprint for children's art supplies. By adjusting variables, users comment on the product's purpose, key features, and material usage. But it doesn't stop there; safety, ergonomics, manufacture, and packaging guidelines are all included, ensuring a top-notch, user-friendly, and commercially viable product design. This app goes in-depth, amplifying your artful vision!

To run this app online: [Kids Art Supply Design Specifier Online](https://hero.page/app/kids-art-supply-design-specifier-custom-ai-children's-art-design/MqQzkNrnCCnS634UcdS8)

[![Run Kids Art Supply Design Specifier Online](/assets/run.svg)](https://hero.page/app/kids-art-supply-design-specifier-custom-ai-children's-art-design/MqQzkNrnCCnS634UcdS8)

To learn more about AI Apps for Product Designer use-cases in the Children's Art Supplies industry, read [How to Innovate Children's Art Supplies Design with AI Tools](https://hero.page/blog/ai/children's-art-supplies/how-to-innovate-children's-art-supplies-design-with-ai-tools/170775)

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
npx hero run ./kids_art_supply_design_specifier.heroml
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
hero run ./kids_art_supply_design_specifier.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./kids_art_supply_design_specifier.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./kids_art_supply_design_specifier.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./kids_art_supply_design_specifier.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Kids Art Supply Design Specifier
```
Your task is to create a "Design Specification" for a product in the "Children's Art Supplies" industry aimed at a "Product Designer". 

Let's begin by crafting a brief introduction that clearly defines the product, its primary function, as well as explaining why the specific children's art supply was chosen - named {{product_choice}}.

Here's some more context about the Design Specification:
Product Choice: {{product_choice}}
Product Objectives: {{product_objectives}}
Age Group: {{age_group}}
Material Choice: {{material_choice}}
Color Scheme: {{color_scheme}}
Assembly Process: {{assembly_process}}
Packaging Guidelines: {{packaging_guidelines}}

->>>>

We have an introduction for our design specification:

Introduction:
{{step_1}}

Next, in the purpose section, identify the main objectives for the design of this product branded as {{product_choice}}. Make sure to include the intended impact on children's creativity and learning: {{product_objectives}}.

->>>>

The introduction for a design specification is:

Introduction:
{{step_1}}

The objectives of designing the product and its potential impacts have been outlined:

Objectives and Impact:
{{step_2}}

Moving forward, provide key design considerations for the product named as {{product_choice}}. Make sure to mention the safety features and ergonomic design suitable for the intended age group. Ensure the design adheres to all relevant safety standards for children's toys and products: {{age_group}}.

->>>>

The objectives of the product and its designed impacts are:

Objectives and Impact:
{{step_2}}

Consideration for designing the product is as follows:

Design Considerations:
{{step_3}}

Next, describe in detail the product features, including the materials that will be used, their qualities, and the reasons for their selection. Include color schemes, shapes, or patterns to make the product more attractive and interesting for users.

->>>>

For our product, we have identified the design considerations:

Design considerations:
{{step_3}}

The detailed features of the product are:

Product Features:
{{step_4}}

Now, provide a thorough usage guideline illustrating how children should use the product, which is governed by its design considerations safely and correctly. Make sure to leave room for the imagination and creativity the product may inspire in its usage.

->>>>

The product has these detailed features:

Product Features:
{{step_4}}

The guidelines on how children might use the product are described:

Usage Guidelines:
{{step_5}}

Moving forward, describe any relevant manufacturing and assembly processes the product will undergo. This should include the methods of production and necessary steps in assembling the product: {{assembly_process}}. 


```

