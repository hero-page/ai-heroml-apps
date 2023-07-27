# DIY Craft Review & Inspiration Generator

Experience the power of AI in crafting with the DIY Craft Review & Inspiration Generator. Specify your variables and let the app create comprehensive, customizable content, including detailed analyses of DIY products. Packed with engaging intros, product specs, performance evaluations, possible crafting uses, and sizzling conclusions, this app inspires creativity while providing in-depth product reviews. The app's unique feature? It exemplifies how a product could be woven into your personal craft projects, offering you a deeper insight into its potential and versatility, enhancing your creative prowess.

To run this app online: [DIY Craft Review & Inspiration Generator Online](https://hero.page/app/diy-craft-review-and-inspiration-generator-inspiring-diy-craft-product-analysis/qUdR941eHHX3RjkyQ41k)

[![Run DIY Craft Review & Inspiration Generator Online](/assets/run.svg)](https://hero.page/app/diy-craft-review-and-inspiration-generator-inspiring-diy-craft-product-analysis/qUdR941eHHX3RjkyQ41k)

To learn more about AI Apps for Content Creator use-cases in the Craft Supplies & DIY Product Marketing industry, read [How to Enhance DIY Content with AI-Crafted Blog and Review Tools](https://hero.page/blog/ai/craft-supplies-and-diy-product-marketing/how-to-enhance-diy-content-with-ai-crafted-blog-and-review-tools/170828)

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
npx hero run ./diy_craft_review_and_inspiration_generator.heroml
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
hero run ./diy_craft_review_and_inspiration_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./diy_craft_review_and_inspiration_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./diy_craft_review_and_inspiration_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./diy_craft_review_and_inspiration_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

