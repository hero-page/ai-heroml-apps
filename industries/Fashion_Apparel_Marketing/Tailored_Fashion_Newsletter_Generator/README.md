# Tailored Fashion Newsletter Generator

The Tailored Fashion Newsletter Generator app creates engaging, customized newsletters for product marketers in the Fashion & Apparel sector. Using advanced AI, it generates content tailored to each brand, covering key product benefits, current trends, and more. The generated content features an introduction, product highlights, usage tips, a preview of upcoming launches, and a strong call-to-action. Ensuring a friendly tone in line with the brand helps build a stronger reader connection. This targeted, personalized content boosts reader engagement, fostering a powerful brand-consumer relationship.

To run this app online: [Tailored Fashion Newsletter Generator Online](https://hero.page/app/tailored-fashion-newsletter-generator-customized-fashion-marketing-content/HEBviwXaIicZIUY3NsP9)

[![Run Tailored Fashion Newsletter Generator Online](/assets/run.svg)](https://hero.page/app/tailored-fashion-newsletter-generator-customized-fashion-marketing-content/HEBviwXaIicZIUY3NsP9)

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
npx hero run ./tailored_fashion_newsletter_generator.heroml
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
hero run ./tailored_fashion_newsletter_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./tailored_fashion_newsletter_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./tailored_fashion_newsletter_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./tailored_fashion_newsletter_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

