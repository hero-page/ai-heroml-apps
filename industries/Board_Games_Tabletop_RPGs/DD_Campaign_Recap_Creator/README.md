# D&D Campaign Recap Creator

D&D Campaign Recap Creator makes the game master's job easier by generating detailed session recaps, customized via AI. Specify variables and the app will outline crucial events, character interactions and the impact of player decisions. Your recap will include unresolved mysteries and exciting teasers for next games, making each session a continuation of the unique story you're crafting. Catering to D&D and similar RPGs, it serves as the perfect dungeon master's assistant.

To run this app online: [D&D Campaign Recap Creator Online](https://hero.page/app/dandd-campaign-recap-creator-personalized-recap-for-dandd-campaigns/LiBRavcYU6yQkpsI7tZy)

[![Run D&D Campaign Recap Creator Online](/assets/run.svg)](https://hero.page/app/dandd-campaign-recap-creator-personalized-recap-for-dandd-campaigns/LiBRavcYU6yQkpsI7tZy)

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
npx hero run ./dandd_campaign_recap_creator.heroml
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
hero run ./dandd_campaign_recap_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./dandd_campaign_recap_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./dandd_campaign_recap_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./dandd_campaign_recap_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for D&D Campaign Recap Creator
```
Your task is to write a "Campaign Recap" for the "Board Games & Tabletop RPGs" industry, specifically for a "Dungeon Master". 
Start by writing an introduction to set the recap scene. This introduction should highlight the key location and theme of the last session: {{campaign_location}} and {{campaign_theme}}.

Here's some more context about the Campaign Recap:
Campaign Location: {{campaign_location}}
Campaign Theme: {{campaign_theme}}
Key Events: {{key_events}}

->>>>

Now that we have an introduction for our "Campaign Recap":

Introduction:
{{step_1}}

Let's move on to enumerating the key events of the campaign. Compile the prioritized events that occurred in chronological order using the key event details: {{key_events}}.

->>>>

With our key events listed in chronological order:

Key Events List:
{{step_2}}

Proceed to expand on these events, creating a logical sequence that describes the consequences and game world impacts of these actions. Use the established list of {{key_events}} for reference.

->>>>

Having detailed the key event sequence:

Key Event Sequence and Impact:
{{step_3}}

Next, delve into characters' actions and decisions. Explain how the players' actions impacted the unfolding of the {{key_events}}.

->>>>

We've covered how the players' actions shaped the campaign:

Player Actions and Their Impact:
{{step_4}}

Let's now dedicate a section to the non-player characters and significant entity interactions. Describe how these characters influenced the campaign's trajectory and added complexity to the {{campaign_theme}}.

->>>>

After addressing the non-player characters and their influence on the campaign:

Non-Player Characters Influence:
{{step_5}}

Focus on the summary of key item discoveries, spells used or learned, and essential battles. Emphasize specific creatures defeated or tactics a player used that were instrumental in impacting the {{key_events}}.

->>>>

Having highlighted key item discoveries, spells and battles:

Key Items, Spells and Battles:
{{step_6}}

Now, discuss any important plot revelations uncovered by the players or through storyline progression in the context of the {{campaign_theme}}.

->>>>

We've discussed important plot revelations relevant to the {{campaign_theme}}:

Plot Revelations:
{{step_7}}

Highlight any unresolved events or cliffhangers that could play an essential role in the next campaign session.

->>>>

We now have a comprehensive list of unresolved events and cliffhangers:

Unresolved Events or Cliffhangers:
{{step_8}}

Summarize the recap by outlining possible future implications under the {{campaign_theme}}, setting a tone for the forthcoming session.


```

