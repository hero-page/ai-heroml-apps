# Craft Materials & Guide Generator

Discover crafting with Craft Materials & Guide Generator. Uniquely designed for craft enthusiasts & beginners, this app unlocks an AI-powered, customized content generation experience. Specify requirements and let our AI create an engaging guide for your project. Guides provide a detailed overview, materials list, safety protocols, maintenance advice, and varied project ideas, all explained in user-friendly language. Welcome to your comprehensive guide to crafting.

To run this app online: [Craft Materials & Guide Generator Online](https://hero.page/app/craft-materials-and-guide-generator-comprehensive-beginner-friendly-craft-guide/8s3fhFWG87uRjximdg3l)

[![Run Craft Materials & Guide Generator Online](/assets/run.svg)](https://hero.page/app/craft-materials-and-guide-generator-comprehensive-beginner-friendly-craft-guide/8s3fhFWG87uRjximdg3l)

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
npx hero run ./craft_materials_and_guide_generator.heroml
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
hero run ./craft_materials_and_guide_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./craft_materials_and_guide_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./craft_materials_and_guide_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./craft_materials_and_guide_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Craft Materials & Guide Generator
```
Your task is to create a "Materials List" for the "Children's Crafts & Hobbies" industry for a "Craft Author". Let's start with an introduction that describes the craft project: {{craft_project}}. This introduction should give a brief overview of the craft project and why it is engaging and fun for kids.

Here's some more context about the Materials List:
Craft Project: {{craft_project}}
Core Materials: {{core_materials}}
Material Preparation: {{material_preparation}}
Safety Considerations: {{safety_considerations}}
Care Maintenance: {{care_maintenance}}
Project Variations: {{project_variations}}

->>>>

Based on the description of the specific craft project:

Craft Project Description:
{{step_1}}

Next, identify and list all the core materials needed for the craft project. This list should include the quantity of each material, distinguishing attributes (color, size, etc.), and any optional items that could enhance the craft but are not mandatory.

->>>>

Building upon the craft project description:

Craft Project Description:
{{step_1}}

We have identified the necessary core materials for this craft project:

Core Materials List:
{{step_2}}

Now, create an organized, step-by-step guide on how to gather and prepare the materials. Explain where to purchase them, how to choose the best quality, and any necessary preparation such as washing, drying or trimming the materials.

->>>>

We have learned about our craft project and listed its core materials:

Craft Project Description:
{{step_1}}

Core Materials List:
{{step_2}}

Let's create a guide on material collection and preparation:

Material Collection & Preparation Guide:
{{step_3}}

Having prepared our materials guide, let's detail any safety considerations when using these materials. This could encompass the use of scissors, glue, or small parts representing choking hazards.

->>>>

With our project, materials, and preparation guide:

Craft Project Description:
{{step_1}}

Material Collection & Preparation Guide:
{{step_3}}

We need to present the safety considerations for using these materials:

Safety Considerations:
{{step_4}}

Next, let's include a section on 'Materials Care & Maintenance'. This might incorporate how to clean and safely store the materials post-craft activity, plus tips to ensure their longevity.

->>>>

Following our extensive safety considerations:

Safety Considerations:
{{step_4}}

Our 'Materials Care & Maintenance' guide will look like this:

Materials Care & Maintenance Guide:
{{step_5}}

Now, let's suggest recommendations for variations and adaptations of the craft project. Propose alternative materials, themes or designs, explaining how these adjustments will refresh and invigorate the craft project each time.

->>>>

After covering care and maintenance:

Materials Care & Maintenance Guide:
{{step_5}}

We will layout suggestions for future variations of the craft project in our:

Project Variations Guide:
{{step_6}}

Lastly, recap your materials list by restating the name of the craft project. Ensure you remind craft authors about the essence of making the craft engaging, fun, and safe for children.


```

