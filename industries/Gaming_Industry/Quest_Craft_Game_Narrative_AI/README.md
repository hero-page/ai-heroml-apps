# Quest Craft: Game Narrative AI

Experience virtual world building like never before with the Quest Craft: Game Narrative AI app. Generate custom and high-quality game content with the intelligent AI that crafts detailed quest narratives based on your specific inputs. This app caters to multiple facets of a video game quest, including the title, context, objectives, challenges, rewards, and hints for future quests. Its trademark, the ability to uphold the game's universe and storyline, ensures your quests are both cohesive and engaging additions to your game's broader narrative.

To run this app online: [Quest Craft: Game Narrative AI Online](https://hero.page/app/quest-craft:-game-narrative-ai-ai-generated-immersive-gaming-quests/kYgklJSg0ICYRkPgThG6)

[![Run Quest Craft: Game Narrative AI Online](/assets/run.svg)](https://hero.page/app/quest-craft:-game-narrative-ai-ai-generated-immersive-gaming-quests/kYgklJSg0ICYRkPgThG6)

To learn more about AI Apps for Game Writer use-cases in the Gaming Industry industry, read [How to Enhance Game Writing with AI - Character Backstory, Quests, Dialogues](https://hero.page/blog/ai/gaming-industry/how-to-enhance-game-writing-with-ai-character-backstory-quests-dialogues/170898)

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
npx hero run ./quest_craft_game_narrative_ai.heroml
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
hero run ./quest_craft_game_narrative_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./quest_craft_game_narrative_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./quest_craft_game_narrative_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./quest_craft_game_narrative_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

