# Custom Art Supply List Planner

Experience the pinnacle of personalized art planning with Custom Art Supply List Planner. This app uses AI to curate detailed & customized lists for children's art educators. Your unique input initiates an in-depth breakdown of supplies by type, quantity, and safety guidelines. Emphasizing eco-friendliness, the app also suggest green alternatives. Included is a comprehensive summary of required items alongside precautionary measures about possible allergies. With a focus on age group & artistic goals, each list is individually tailored ensuring teaching creativity is as effortless as it is safe and eco-conscious.

To run this app online: [Custom Art Supply List Planner Online](https://hero.page/app/custom-art-supply-list-planner-personalized-eco-friendly-art-planning/VdZdZLEXtaPAH7LEc7X2)

[![Run Custom Art Supply List Planner Online](/assets/run.svg)](https://hero.page/app/custom-art-supply-list-planner-personalized-eco-friendly-art-planning/VdZdZLEXtaPAH7LEc7X2)

To learn more about AI Apps for Art Educator use-cases in the Children's Art Supplies industry, read [How to Elevate Children's Art Lessons with AI Planning Tools](https://hero.page/blog/ai/children's-art-supplies/how-to-elevate-children's-art-lessons-with-ai-planning-tools/170774)

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
npx hero run ./custom_art_supply_list_planner.heroml
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
hero run ./custom_art_supply_list_planner.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./custom_art_supply_list_planner.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./custom_art_supply_list_planner.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./custom_art_supply_list_planner.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Custom Art Supply List Planner
```
Your task is to write a "Materials List" for the "Children's Art Supplies" industry, specifically for an "Art Educator". Let's start by creating an introduction that details the age group and artistic goals of the lesson plan: {{age_group_and_goal}}.

Here's some more context about the Materials List:
Age Group And Goal: {{age_group_and_goal}}
Art Supply Type: {{art_supply_type}}
Art Supply Item: {{art_supply_item}}
Eco Friendly Items: {{eco_friendly_items}}
Material Allergies Sensitivities: {{material_allergies_sensitivities}}

->>>>

We are partway through the "Materials List", with an introduction that details the age group and artistic goals of the lesson plan:

Introduction:
{{step_1}}

Next, let's segregate the list into different sections based on the type or class of art supply; for instance, drawing materials, painting supplies, crafting items, and specialty supplies.

->>>>

In the "Materials List", we have the introduction, and the sections based on the type or class of art supply:

Introduction:
{{step_1}}

Type/Class of Art Supply:
{{step_2}}

Now, within each section, we need to list individual items necessary for the project. Each entry on the list should include the item's name, the quantity needed, and a brief description of its use in the class.

->>>>

We have the introduction, the sections based on the type or class of art supply, and the individual items necessary for the project in our "Materials List":

Introduction:
{{step_1}}

Type/Class of Art Supply:
{{step_2}}

Individual Art Supply Items for Project:
{{step_3}}

We need to add a section dedicated to safety materials and equipment, especially for situations where the items on the list might require extra safety precautions.

->>>>

In our "Materials List", along with the introduction, sections based on the type or class of art supply, and the individual items, we have introduced a section dedicated to safety materials and equipment:

Introduction:
{{step_1}}

Type/Class of Art Supply:
{{step_2}}

Individual Art Supply Items for Project:
{{step_3}}

Safety Materials and Equipment:
{{step_4}}

Next, let's add an additional environment-friendly category that will provide information on eco-friendly alternatives to traditional supplies.

->>>>

Our "Materials List" has an introduction, sections based on the type or class of art supply, individual items, safety materials, and we have introduced an environment-friendly category:

Introduction:
{{step_1}}

Type/Class of Art Supply:
{{step_2}}

Individual Art Supply Items for Project:
{{step_3}}

Safety Materials and Equipment:
{{step_4}}

Environment-Friendly Category:
{{step_5}}

Now, we need to conclude the list with a summary of the total number of unique items required, re-emphasizing the age group and artistic goal of the lesson plan.


```

