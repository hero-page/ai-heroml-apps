# Mexican Spices Expert Guide Creator

Explore the vibrant world of Mexican spices with Mexican Spices Expert Guide Creator. Create personalized guides with AI tech, detailing essence, uses, historical significance, health benefits, and storage tips of spices. Dive into cooking techniques like roasting, smoking, and griddling. Explore unique flavors like adobos, moles, and salsas to enhance your dishes. Discover lesser-known Mexican spices, expanding your culinary skills. A comprehensive and detailed insight into Mexican cuisine.

To run this app online: [Mexican Spices Expert Guide Creator Online](https://hero.page/app/mexican-spices-expert-guide-creator-crafting-unique-mexican-spice-combinations/HW1vt8eIMXou3uPPlqJS)

[![Run Mexican Spices Expert Guide Creator Online](/assets/run.svg)](https://hero.page/app/mexican-spices-expert-guide-creator-crafting-unique-mexican-spice-combinations/HW1vt8eIMXou3uPPlqJS)

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
npx hero run ./mexican_spices_expert_guide_creator.heroml
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
hero run ./mexican_spices_expert_guide_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./mexican_spices_expert_guide_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./mexican_spices_expert_guide_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./mexican_spices_expert_guide_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

