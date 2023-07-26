# Automotive Specs AI for Marketers

Automotive Specs AI for Marketers is a tool designed for marketing professionals in the automotive industry. Powered by advanced AI, it aids in creating comprehensive, customized 'Product Specifications' documents for distinct car models. The app details on a range of aspects ranging from physical traits and technical specifications to warranty information and unique selling points. Its stand-out feature is that it goes beyond simple specs, offering in-depth analysis of a vehicle's unique selling points. Making your marketing campaigns more effective and targeted.

To run this app online: [Automotive Specs AI for Marketers Online](https://hero.page/app/automotive-specs-ai-for-marketers-ai-powered-custom-auto-specs/yarYc1gTNBqA09L142VA)

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
npx hero run ./automotive_specs_ai_for_marketers.heroml
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
hero run ./automotive_specs_ai_for_marketers.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./automotive_specs_ai_for_marketers.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./automotive_specs_ai_for_marketers.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./automotive_specs_ai_for_marketers.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Automotive Specs AI for Marketers
```
Your task is to write a "Product Specifications" for the "Automotive Product Marketing" industry, specifically for a "Product Marketer".

Let's start by creating an introductory section for the product specifications, where we explain the car model: {{car_model}}.

Here's some more context about the Product Specifications:
Car Model: {{car_model}}
Physical Characteristics: {{physical_characteristics}}
Technical Specifications: {{technical_specifications}}
Interior Features: {{interior_features}}
Warranty Service: {{warranty_service}}
Unique Selling Points: {{unique_selling_points}}

->>>>

Our introductory section for the "Product Specifications" now provides an explanation for the car model:

Introduction:
{{step_1}}

Next, outline the physical characteristics of the car, detailing elements such as size, weight, color options, and type (SUV, Sedan, sports, etc).

->>>>

The details about the car model are as follows:

Introduction:
{{step_1}}

Physical Characteristics:
{{step_2}}

Continuing on, let's write a section covering the key technical aspects such as engine type, horsepower, fuel efficiency, type of transmission, and safety features.

->>>>

The physical and technical aspects of the car model are as follows:

Physical Characteristics:
{{step_2}}

Technical Specifications:
{{step_3}}

Next, dedicate a section to interior and comfort features such as the seating material, infotainment system, air conditioning, passenger capacity, and cargo space.

->>>>

The technical specifications and interior features of the car model are:

Technical Specifications:
{{step_3}}

Interior and Comfort Features:
{{step_4}}

Now, include a section on warranty information and after-sales service offers. Detail the warranty period, what it includes, and any extra benefits the buyer would receive.

->>>>

The interior features and warranty information of the car model are as follows:

Interior and Comfort Features:
{{step_4}}

Warranty and Service Offers:
{{step_5}}

Lastly, wrap up the "Product Specifications" by highlighting the unique selling points that set the vehicle apart from its competitors in the market. These features could include groundbreaking technology, superior comfort, unrivaled performance, or cost-effectiveness. 


```

