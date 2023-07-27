# DIY Product Use-cases Writer

DIY Product Use-cases Writer is a state-of-art app that leverages AI to generate intricate, tailored product descriptions steeped in DIY terminology. By specifying variables, users receive lucid yet compelling content illustrating product features, real-world applications, and problem-solving prowess. It also provides instructions for product usage, outlines unique benefits, and highlights its positive impacts on user's hobbies or lifestyles. The end product is a compelling combination of the product's distinct value, a comparative analysis from rivals, and an engaging call-to-action embedded in crafting-focused language. This robust, targeted communication approach is designed not just to inform but also to captivate and convert its intended audience.

To run this app online: [DIY Product Use-cases Writer Online](https://hero.page/app/diy-product-use-cases-writer-crafting-terminology-driven-product-descriptions/k6I223Tg6R699F2m6M6S)

[![Run DIY Product Use-cases Writer Online](/assets/run.svg)](https://hero.page/app/diy-product-use-cases-writer-crafting-terminology-driven-product-descriptions/k6I223Tg6R699F2m6M6S)

To learn more about AI Apps for Product Marketer use-cases in the Craft Supplies & DIY Product Marketing industry, read [How to Elevate Craft Marketing with AI-Generated Use-cases & Newsletters](https://hero.page/blog/ai/craft-supplies-and-diy-product-marketing/how-to-elevate-craft-marketing-with-ai-generated-use-cases-and-newsletters/170827)

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
npx hero run ./diy_product_use_cases_writer.heroml
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
hero run ./diy_product_use_cases_writer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./diy_product_use_cases_writer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./diy_product_use_cases_writer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./diy_product_use_cases_writer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

