# Craft Kit Description AI Writer

The Craft Kit Description AI Writer app is an AI-powered solution aimed at generating custom, high-quality descriptions for children's craft kits. Input specific variables and it'll present a catchy headline, detailed item list, instructions, appropriate age, safety advice, and purchase info. Its specificity to kids' craft kits sets it apart from commonplace product description generators.

To run this app online: [Craft Kit Description AI Writer Online](https://hero.page/app/craft-kit-description-ai-writer-ai-powered-child-craft-kit-guide/f2CiGdnm49wmETK41prw)

[![Run Craft Kit Description AI Writer Online](/assets/run.svg)](https://hero.page/app/craft-kit-description-ai-writer-ai-powered-child-craft-kit-guide/f2CiGdnm49wmETK41prw)

To learn more about AI Apps for Product Marketer use-cases in the Children's Crafts & Hobbies industry, read [How to Amplify Children's Crafts Marketing with AI Solutions](https://hero.page/blog/ai/children's-crafts-and-hobbies/how-to-amplify-children's-crafts-marketing-with-ai-solutions/170782)

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
npx hero run ./craft_kit_description_ai_writer.heroml
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
hero run ./craft_kit_description_ai_writer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./craft_kit_description_ai_writer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./craft_kit_description_ai_writer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./craft_kit_description_ai_writer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Craft Kit Description AI Writer
```
Your task is to write a "Craft Kit Description" for the "Children's Crafts & Hobbies" industry, specifically for a "Product Marketer". You should write this description in a playful, engaging style, ensuring it appeals to children and their parents. Let's start with creating an enticing headline.

Here's some more context about the Craft Kit Description:
Headline: {{headline}}
Kit Overview: {{kit_overview}}
Kit Contents: {{kit_contents}}
Kit Benefits: {{kit_benefits}}
Step By Step Instructions: {{step_by_step_instructions}}
Suitable Age: {{suitable_age}}
Safety Precautions: {{safety_precautions}}
Purchase Information: {{purchase_information}}

->>>>

Now, we have a catchy, fun headline for the craft kit:

Headline:
{{step_1}}

Next, let's write a short introduction that encapsulates the main elements and purpose of the craft kit.

->>>>

We have created an enticing headline and a brief introduction for the craft kit:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Now, let's describe each item included in this craft kit in a comprehensive and easy-to-digest manner.

->>>>

We have a catchy title, an engaging introduction, and a detailed list of the kit's contents:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Kit Contents:
{{step_3}}

Next, detail the benefits children will get from using this craft kit. Consider aspects like educational value, skill development, and creative exploration.

->>>>

We have listed the kit's contents and detailed the various benefits children will get from using this craft kit:

Kit Contents:
{{step_3}}

Kit Benefits:
{{step_4}}

Next, let's write step-by-step instructions on how to use the craft kit, ensuring they are simple and easily comprehensible for children.

->>>>

Now, we have the kit's benefits and a clear set of instructions on how to use the craft kit:

Kit Benefits:
{{step_4}}

Step-by-Step Instructions:
{{step_5}}

Next step is to clearly define the age suitability of the craft kit, in compliance with the manufacturer's guidelines.

->>>>

We have comprehensive instructions for using the craft kit, and a clearly defined the age suitability for the kit:

Step-by-Step Instructions:
{{step_5}}

Suitable Age:
{{step_6}}

Now, highlight any safety precautions or warnings attached to the craft kit to ensure parents are aware of potential hazards.


```

