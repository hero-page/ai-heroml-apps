# Chinese New Year Culinary Culture Guide

Dive into the rich culinary culture of the Chinese New Year! This app takes you on a guided culinary journey, providing detailed recipes and highlighting cultural symbolism behind each dish. Relying on AI, it creates customized, informative content that not just teaches cooking, but elaborates on rituals, taboos, and unique anecdotes surrounding each dish. Emphasizing the role of the Cultural Cooking Instructor, this app gives you an educational exploration, comparing traditions with other cultural celebrations, truly a comprehensive cultural-culinary guide.

To run this app online: [Chinese New Year Culinary Culture Guide Online](https://hero.page/app/chinese-new-year-culinary-culture-guide-cultural-culinary-journey:-chinese-new-year/v77avc0IkvV5guOwKVgm)

[![Run Chinese New Year Culinary Culture Guide Online](/assets/run.svg)](https://hero.page/app/chinese-new-year-culinary-culture-guide-cultural-culinary-journey:-chinese-new-year/v77avc0IkvV5guOwKVgm)

To learn more about AI Apps for Cultural Cooking Instructor use-cases in the Food and Culture industry, read [How to Enrich Cultural Cooking Classes with AI-Powered Guide](https://hero.page/blog/ai/food-and-culture/how-to-enrich-cultural-cooking-classes-with-ai-powered-guide/170890)

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
npx hero run ./chinese_new_year_culinary_culture_guide.heroml
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
hero run ./chinese_new_year_culinary_culture_guide.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./chinese_new_year_culinary_culture_guide.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./chinese_new_year_culinary_culture_guide.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./chinese_new_year_culinary_culture_guide.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

