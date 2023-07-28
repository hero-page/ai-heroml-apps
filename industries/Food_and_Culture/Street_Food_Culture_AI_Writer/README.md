# Street Food Culture AI Writer

Discover the richness of global street food culture with the Street Food Culture AI Writer app. Powered by advanced AI, this tool creates personalized, comprehensive guides to city's street food scenes. Tailor your prompts to generate high-quality content that dives deep into local culinary landscapes. Includes overviews, detailed descriptions, mapped food spots, dietary advise, safety tips, local anecdotes, and more. Stand out with engaging, respectful, even humorous content, perfect for food lovers and travel bloggers.

To run this app online: [Street Food Culture AI Writer Online](https://hero.page/app/street-food-culture-ai-writer-ai-powered-deep-dive-street-food-guide/8WtSBgBPcNzyVDh2uJqI)

[![Run Street Food Culture AI Writer Online](/assets/run.svg)](https://hero.page/app/street-food-culture-ai-writer-ai-powered-deep-dive-street-food-guide/8WtSBgBPcNzyVDh2uJqI)

To learn more about AI Apps for Food Travel Blogger use-cases in the Food and Culture industry, read [How to Craft Ultimate Food Guides using AI in Travel Blogging](https://hero.page/blog/ai/food-and-culture/how-to-craft-ultimate-food-guides-using-ai-in-travel-blogging/170889)

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
npx hero run ./street_food_culture_ai_writer.heroml
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
hero run ./street_food_culture_ai_writer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./street_food_culture_ai_writer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./street_food_culture_ai_writer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./street_food_culture_ai_writer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

