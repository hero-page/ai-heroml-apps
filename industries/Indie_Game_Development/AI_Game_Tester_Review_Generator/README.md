# AI Game Tester Review Generator

AI Game Tester Review Generator is a specialized app for crafting in-depth game reviews. You can specify distinct variables which AI utilizes to generate detailed content. Using encompassing game analysis from game tester’s perspective, the AI constructs comprehensive evaluation inclusive of gameplay mechanics, plot, characters, game difficulty, uniqueness and any potential issues. With its unique trait of demonstrating a game tester's perspective, it ensures in-depth gameplay analysis, enlightening potential players about the game's quality features. The final rating further helps users comprehend the game's overall worth, making their choice easier.

To run this app online: [AI Game Tester Review Generator Online](https://hero.page/app/ai-game-tester-review-generator-expert-imbued-game-reviews/BawN9zPwCsi7ibOt3l8E)

[![Run AI Game Tester Review Generator Online](/assets/run.svg)](https://hero.page/app/ai-game-tester-review-generator-expert-imbued-game-reviews/BawN9zPwCsi7ibOt3l8E)

To learn more about AI Apps for Game Tester use-cases in the Indie Game Development industry, read [How to Enhance Game Testing with AI Guide and Review Tools](https://hero.page/blog/ai/indie-game-development/how-to-enhance-game-testing-with-ai-guide-and-review-tools/170995)

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
npx hero run ./ai_game_tester_review_generator.heroml
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
hero run ./ai_game_tester_review_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ai_game_tester_review_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ai_game_tester_review_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ai_game_tester_review_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

