# RPG World Builder: Interactive Guide AI

RPG World Builder: Interactive Guide AI is a dynamic game-creation tool. With users' input, AI assists in creating a customized, high-quality RPG world. Prioritize variables, such as geography, climate, species, magic systems and more. The AI then generates a detailed and immersive guide that impacts the course of the gameplay. Beyond information, it illuminates on how these defined world elements influence potential scenarios or outcomes. The guide is malleable for storytellers and game masters, offering flexibility for modifications and opening doors for riveting stories and unique gaming experiences. A remarkable tool in the realm of tabletop RPGs.

To run this app online: [RPG World Builder: Interactive Guide AI Online](https://hero.page/app/rpg-world-builder:-interactive-guide-ai-ai-assisted-dynamic-rpg-world-building/l1IKUk0LCtey7QjUFrhC)

[![Run RPG World Builder: Interactive Guide AI Online](/assets/run.svg)](https://hero.page/app/rpg-world-builder:-interactive-guide-ai-ai-assisted-dynamic-rpg-world-building/l1IKUk0LCtey7QjUFrhC)

To learn more about AI Apps for Dungeon Master use-cases in the Board Games & Tabletop RPGs industry, read [How to Enhance RPG Campaigns with AI-Assisted World Building and Backstories](https://hero.page/blog/ai/board-games-and-tabletop-rpgs/how-to-enhance-rpg-campaigns-with-ai-assisted-world-building-and-backstories/170758)

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
npx hero run ./rpg_world_builder_interactive_guide_ai.heroml
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
hero run ./rpg_world_builder_interactive_guide_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./rpg_world_builder_interactive_guide_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./rpg_world_builder_interactive_guide_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./rpg_world_builder_interactive_guide_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for RPG World Builder: Interactive Guide AI
```
Your task is to write a "World Building Guide" for a "Dungeon Master" in the "Board Games & Tabletop RPGs" industry. 

Let's start with an introduction that summarizes the purpose of the guide and sketches out the basic parameters of the world to be built: {{world_concept}}.

Here's some more context about the World Building Guide:
World Concept: {{world_concept}}
Geography Climate: {{geography_climate}}
Races Species: {{races_species}}
World History: {{world_history}}
World Magic: {{world_magic}}
World Politics: {{world_politics}}
World Economy: {{world_economy}}

->>>>

We have an introduction and basic parameters for our "World Building Guide":

Introduction and Basic World Parameters:
{{step_1}}

Next, describe the geography & climate of the world in detail: {{geography_climate}}. This section should include descriptions of landscapes, continents, oceans, and how the climate shapes the world.

->>>>

After creating a basic world concept, we have the geography and climate for our world:

Geography and Climate:
{{step_2}}

Now, let's discuss the different races and species (if any) that inhabit your world: {{races_species}}. This might include their specific habitats, cultures, languages, relationships with each other, and any unique biological aspects.

->>>>

So far we have the geography and the races that live in our world:

Geography and Climate:
{{step_2}}

Races and Species:
{{step_3}}

Next, detail the history of this world: {{world_history}}. This should cover major historical events, cultural shifts, wars, and changes in power structure.

->>>>

In our "World Building Guide", we have details about the geography, climate, and the races, and now we have a clear world history:

World History:
{{step_4}}

For the next step, define the system of magic or supernatural phenomena, if any, present in the world: {{world_magic}}. Describe how it works, who can use it, and how it impacts the world and the people living there.

->>>>

So far in our guide, we have developed the history and magic system of our world:

World History:
{{step_4}}

Magic System:
{{step_5}}

Now, write about the political structure of the world: {{world_politics}}. Explain the different nations, factions, their relationships, and the balance (or imbalance) of power.

->>>>

For our guide, we have established a magic system and a political structure:

Magic System:
{{step_5}}

Political Structure:
{{step_6}}

Let's move onto the economy of the world: {{world_economy}}. This should include information about the common currencies, trade goods, significant industries, and any unique economic systems or practices.

->>>>

So far in our guide, we have described the political structure and the economy:

Political Structure:
{{step_6}}

Economy:
{{step_7}}

Finally, summarize the guide with an overview of adventuring in the world. Discuss potential plot hooks, dungeons, conflicts, and important NPCs. 

For each of these paragraphs, keep in mind how each element can impact the gameplay, storyline and choices players might make, and highlight elements that make the world unique to enhance its vividness and appeal.


```

