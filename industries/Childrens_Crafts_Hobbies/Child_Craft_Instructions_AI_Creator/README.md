# Child Craft Instructions AI Creator

Discover the magic of AI with Child Craft Instructions AI Creator, a unique app providing tailored kids craft guides. With the ability to specify variables in prompts, users can access custom, high-quality content generation for engaging and simple craft guides. These comprehensive instructions include a catchy title, craft overview, difficulty level, material list, and step-by-step process, alongside crafty tips and alternatives. Culminating with a summary and customisation ideas, these guides are specifically designed for children, striking a perfect balance between information and engagement. Enhance your child's craft-making journey today.

To run this app online: [Child Craft Instructions AI Creator Online](https://hero.page/app/child-craft-instructions-ai-creator-tailored-kids-craft-guides/pbNwNCCDCLAPU6Y9Vazz)

[![Run Child Craft Instructions AI Creator Online](/assets/run.svg)](https://hero.page/app/child-craft-instructions-ai-creator-tailored-kids-craft-guides/pbNwNCCDCLAPU6Y9Vazz)

To learn more about AI Apps for Craft Author use-cases in the Children's Crafts & Hobbies industry, read [How to Elevate Children's Craft Projects using Innovative AI Apps](https://hero.page/blog/ai/children's-crafts-and-hobbies/how-to-elevate-children's-craft-projects-using-innovative-ai-apps/170780)

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
npx hero run ./child_craft_instructions_ai_creator.heroml
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
hero run ./child_craft_instructions_ai_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./child_craft_instructions_ai_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./child_craft_instructions_ai_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./child_craft_instructions_ai_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Child Craft Instructions AI Creator
```
Your task is to write "Step-by-step Instructions" for the "Children's Crafts & Hobbies" industry for a "Craft Author". 

Let's begin by crafting a catchy title that accurately describes the craft.

Here's some more context about the Step-by-step Instructions:
Craft Title: {{craft_title}}
Craft Overview: {{craft_overview}}
Difficulty Level: {{difficulty_level}}
Materials Needed: {{materials_needed}}
Step By Step Instructions: {{step_by_step_instructions}}
Tips And Tricks: {{tips_and_tricks}}
Craft Conclusion: {{craft_conclusion}}

->>>>

For your "Step-by-step Instructions", we have created a catchy title:

Craft Title:
{{step_1}}

Next, write an introduction for the craft, briefly describing what it is and giving an overview of the process to stimulate the child's interest.

->>>>

For your instructions, we now have a catchy title and an interesting introduction:

Craft Title:
{{step_1}}

Craft Introduction:
{{step_2}}

Let's go to the next step, where we identify the difficulty level of the craft. This will ensure that the child is aware of the complexity of the activity they are going to undertake.

->>>>

In addition to a catchy title and introductory brief, we now have an identified difficulty level:

Craft Title:
{{step_1}}

Craft Introduction:
{{step_2}}

Difficulty Level:
{{step_3}}

Next, provide a detailed list of all the necessary materials and tools needed to complete the craft. If possible, specify the exact quantity.

->>>>

Now we have a catchy title, introductory brief, a difficulty level, and a list of required materials and tools for the craft:

Craft Title:
{{step_1}}

Craft Introduction:
{{step_2}}

Difficulty Level:
{{step_3}}

Materials Needed:
{{step_4}}

For the next step, provide detailed step-by-step instructions on how to create the craft. Ensure each step logically progresses from the previous one, using clear and concise language.

->>>>

We have a catchy title, introduction, difficulty level, list of materials, and now step-by-step instructions:

Craft Title:
{{step_1}}

Craft Introduction:
{{step_2}}

Difficulty Level:
{{step_3}}

Materials Needed:
{{step_4}}

Step-by-Step Instructions:
{{step_5}}

Next, give tips and tricks relevant to the craft. Highlight potential difficulty spots within the steps or suggest alternative methods or materials to improve the child's experience.

->>>>

With the catchy title, introduction, difficulty level, list of materials, step-by-step instructions, and tips and tricks, we're almost done:

Craft Title:
{{step_1}}

Craft Introduction:
{{step_2}}

Difficulty Level:
{{step_3}}

Materials Needed:
{{step_4}}

Step-by-Step Instructions:
{{step_5}}

Tips and Tricks:
{{step_6}}

To complete your craft instructions, write a conclusion. This should summarize what the child has achieved, and propose additional ideas on how they can further use or customize the craft.


```

