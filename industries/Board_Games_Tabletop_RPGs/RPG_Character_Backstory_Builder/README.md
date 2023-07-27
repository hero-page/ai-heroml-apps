# RPG Character Backstory Builder

RPG Character Backstory Builder, a comprehensive RPG character backstory generator, lets you specify variables to create a full-fledged role-playing persona. Leveraging AI, it generates high-quality, tailored content, including name, race, class, origin, family history, and key life events. It crafts a detailed narrative of the character's journey and aspirations, incorporating their personality, strengths, and flaws. From details of their professional life to a pre-game story summary, the app creates an immersive RPG experience, offering unique in-depth character backstories.

To run this app online: [RPG Character Backstory Builder Online](https://hero.page/app/rpg-character-backstory-builder-comprehensive-rpg-character-backstory-generator/0ma2SLeJAQdYsmzHTY1t)

[![Run RPG Character Backstory Builder Online](/assets/run.svg)](https://hero.page/app/rpg-character-backstory-builder-comprehensive-rpg-character-backstory-generator/0ma2SLeJAQdYsmzHTY1t)

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
npx hero run ./rpg_character_backstory_builder.heroml
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
hero run ./rpg_character_backstory_builder.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./rpg_character_backstory_builder.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./rpg_character_backstory_builder.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./rpg_character_backstory_builder.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for RPG Character Backstory Builder
```
Your task is to write a "Character Backstory" for the "Board Games & Tabletop RPGs" industry, specifically for a "Dungeon Master". 

Let's begin by establishing the basic information about the character: {{character_name}}, {{character_race}}, {{character_class}}, {{character_alignment}} and {{character_level}}. This forms the foundational information that would define who the character is within the game world.

Here's some more context about the Character Backstory:
Character Name: {{character_name}}
Character Race: {{character_race}}
Character Class: {{character_class}}
Character Alignment: {{character_alignment}}
Character Level: {{character_level}}
Character Origin Location: {{character_origin_location}}
Character Family And Early Life: {{character_family_and_early_life}}
Character Catalyst: {{character_catalyst}}
Character Goals: {{character_goals}}
Character Traits: {{character_traits}}
Character Profession: {{character_profession}}

->>>>

We now have the basic details of the character:

Character Name:
{{step_1}}

Next, set the character's geographical origin within the game world. This should denote where their journey begins, their hometown or perhaps a significant location from their early life that would shape their personality and views. This location: {{character_origin_location}}, should align with the settings and world-building elements of the campaign.

->>>>

With a name for the character and their origin location, we have:

Character Name:
{{step_1}}

Origin Location:
{{step_2}}

Now, detail the character's family and early life which shapes much of his/her worldview. It should include information relating to the character's upbringing, key members of their family, socio-economic status, and important early life events. This information forms {{character_family_and_early_life}}.

->>>>

Our character, with their name, origin, and their family & early life details, are as follows:

Character Name:
{{step_1}}

Origin Location:
{{step_2}}

Family & Early Life:
{{step_3}}

Let's move on to describe the key event(s) or catalyst(s) that turned the character onto the path of adventure. This could be anything from a personal tragedy to the urge to seek out glory or even being chosen by a divine entity. These event(s) make up the {{{character_catalyst}}} and can be significant plot points in the character's development arc.

->>>>

For our character, these are the details we have so far:

Character Name:
{{step_1}}

Family & Early Life:
{{step_3}}

Character Catalyst:
{{step_4}}

Next, let's explore the character's personal aspirations, goals, and motivations. These drives form the basis of {{character_goals}} and are vital to shaping the character's actions, decisions, and growth throughout the campaign.

->>>>

The details we've gathered about the character so far include their name, the key event that marks the start of their journey, and their motivations. They are as follows:

Character Name:
{{step_1}}

Character Catalyst:
{{step_4}}

Character Goals:
{{step_5}}

Moving on, delve into the character's personality traits, strengths, and flaws. This could be determined using the personality aspects of the Dungeons and Dragons Character sheet or custom-created by the Dungeon Master to align with the character's backstory. Include these traits in {{character_traits}}.

->>>>

For our character, here's what we have:

Character Goals:
{{step_5}}

Character Traits:
{{step_6}}

Following this, provide a detailed account of the Character's Professional life, detailing the knowledge, skills, and experiences gained in their chosen field or occupation, example being a rogue's time as a thief or a wizard's years spent studying arcane texts. This professional background will make up {{character_profession}}.


```

