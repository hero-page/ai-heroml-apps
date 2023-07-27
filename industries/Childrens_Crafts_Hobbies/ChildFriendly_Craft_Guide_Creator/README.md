# Child-Friendly Craft Guide Creator

Explore your child's creativity with the Child-Friendly Craft Guide Creator. This intuitive app uses AI to generate customized, kid-safe craft guides based on your specified variables. Ensuring your child's safety and interest, it creates comprehensive guides complete with catchy titles, an engaging project overview, age suitability indication, a detailed list of required materials and tools, easy-to-follow instructions with safety notes, and a practical conclusion offering creative ways to use the finished craft. Rely on it for unique, engaging, and safe crafting experiences.

To run this app online: [Child-Friendly Craft Guide Creator Online](https://hero.page/app/child-friendly-craft-guide-creator-customized-kid-safe-craft-guides/avvOE2H1pIR1KczWgC3H)

[![Run Child-Friendly Craft Guide Creator Online](/assets/run.svg)](https://hero.page/app/child-friendly-craft-guide-creator-customized-kid-safe-craft-guides/avvOE2H1pIR1KczWgC3H)

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
npx hero run ./child_friendly_craft_guide_creator.heroml
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
hero run ./child_friendly_craft_guide_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./child_friendly_craft_guide_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./child_friendly_craft_guide_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./child_friendly_craft_guide_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Child-Friendly Craft Guide Creator
```
Your task is to write a "Craft Project Description" for the "Children's Crafts & Hobbies" industry, specifically for a "Craft Author". 

Let's start with a captivating title that succinctly describes the craft project. Remember, this is what readers will see first.

Here's some more context about the Craft Project Description:
Craft Project Title: {{craft_project_title}}
Craft Project Overview: {{craft_project_overview}}
Age Suitability: {{age_suitability}}
Materials And Tools: {{materials_and_tools}}
Step By Step Instructions: {{step_by_step_instructions}}
Safety Notes: {{safety_notes}}
Usage Ideas: {{usage_ideas}}

->>>>

This is our catchy title for our craft project:

Craft Project Title:
{{step_1}}

Next, write a brief introduction that provides an overview of the craft project. This should be engaging, give a taste of what the project entails, and spark curiosity in the reader.

->>>>

So far, we have a title and an introduction for our craft project:

Craft Project Title:
{{step_1}}

Craft Project Overview:
{{step_2}}

Now, include an age suitability section. Since the industry is "Children's Crafts & Hobbies", this section should clearly inform the reader of the age group the craft is most suitable for.

->>>>

For our craft project, we have a title, an overview, and an age suitability section:

Craft Project Title:
{{step_1}}

Craft Project Overview:
{{step_2}}

Age Suitability:
{{step_3}}

Next, detail a materials and tools section. This list should contain all the necessary items needed for the completion of the craft project. Ensure to list everything in order of use.

->>>>

Our craft project so far has a title, an overview, an age suitability section and a materials and tools section:

Craft Project Title:
{{step_1}}

Craft Project Overview:
{{step_2}}

Age Suitability:
{{step_3}}

Materials and Tools:
{{step_4}}

Now, write a step-by-step instructions section. This should break down the craft process into clear, simple, and easy-to-follow steps.

->>>>

Our craft project now has a title, an overview, an age suitability section, a materials and tools list, and a step-by-step instruction section:

Craft Project Title:
{{step_1}}

Craft Project Overview:
{{step_2}}

Age Suitability:
{{step_3}}

Materials and Tools:
{{step_4}}

Step-by-Step Instructions:
{{step_5}}

Next, incorporate safety notes and an adult supervision advisory at the necessary steps of the instructions. These notes are crucial to help prevent accidents during the crafting process.


```

