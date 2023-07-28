# Emotive Fashion Product Storyteller

Discover an innovative way to enhance your fashion product's appeal with Emotive Fashion Product Storyteller. Harness AI to craft detailed, personalized narratives that evoke powerful emotions, captivate potential buyers, and increase engagement. Narrate your product's unique origins, features, ideal customer profile, and how it's a perfect fit for your customer's lifestyle. Unlike traditional product descriptions or marketing content, our app creates deep, meaningful connections between your product and its potential buyers, stirring emotions that compel them to purchase and giving your brand a distinctive edge. Enjoy uniquely crafted, high-quality content that truly resonates.

To run this app online: [Emotive Fashion Product Storyteller Online](https://hero.page/app/emotive-fashion-product-storyteller-personalized-emotional-fashion-storytelling/obfcOIH8VrnrLywKH8nM)

[![Run Emotive Fashion Product Storyteller Online](/assets/run.svg)](https://hero.page/app/emotive-fashion-product-storyteller-personalized-emotional-fashion-storytelling/obfcOIH8VrnrLywKH8nM)

To learn more about AI Apps for Product Marketer use-cases in the Fashion & Apparel Marketing industry, read [How to Enhance Fashion Marketing with AI for Storytelling and Trend Analysis](https://hero.page/blog/ai/fashion-and-apparel-marketing/how-to-enhance-fashion-marketing-with-ai-for-storytelling-and-trend-analysis/170867)

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
npx hero run ./emotive_fashion_product_storyteller.heroml
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
hero run ./emotive_fashion_product_storyteller.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./emotive_fashion_product_storyteller.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./emotive_fashion_product_storyteller.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./emotive_fashion_product_storyteller.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

