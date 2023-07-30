# Mexican Cuisine History Dissector

Explore and dissect the rich heritage of authentic Mexican cuisine like never-before with Mexican Cuisine History Dissector. This app uses advanced AI technology to generate unique content on the complex history, varied cultural significance, and distinctive culinary traditions of Mexican food. Set your variables and watch as the app delivers a detailed analysis, tracing the origins from ancient Mesoamerican cultures through to its global spread. Gain insights on the role of cuisine in Mexican festivals, its recognition by UNESCO, and misconceptions, specially around Tex-Mex and authentic Mexican cuisine. Learn about staple ingredients, dish preparations, and how geography and climate influence its diversity. This app uniquely emphasizes on clearing misunderstandings, elevating understanding of Mexican food heritage, separating it from generic discussions.

To run this app online: [Mexican Cuisine History Dissector Online](https://hero.page/app/mexican-cuisine-history-dissector-dissecting-authentic-mexican-cuisine-history/zzU49lk8A5CCsp51vueO)

[![Run Mexican Cuisine History Dissector Online](/assets/run.svg)](https://hero.page/app/mexican-cuisine-history-dissector-dissecting-authentic-mexican-cuisine-history/zzU49lk8A5CCsp51vueO)

To learn more about AI Apps for Mexican Cuisine Expert use-cases in the International Cuisine industry, read [How to Master Authentic Taco Recipes and Mexican Spices with AI](https://hero.page/blog/ai/international-cuisine/how-to-master-authentic-taco-recipes-and-mexican-spices-with-ai/171008)

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
npx hero run ./mexican_cuisine_history_dissector.heroml
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
hero run ./mexican_cuisine_history_dissector.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./mexican_cuisine_history_dissector.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./mexican_cuisine_history_dissector.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./mexican_cuisine_history_dissector.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

