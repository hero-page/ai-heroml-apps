# Child Sport Ad Copy Creator

Child Sport Ad Copy Creator is a powerful app that uses AI to produce customized content for children's sports and outdoor products. It provides engaging, child-friendly ad copy, highlighting key product features, safety measures, benefits, and purchasing details. The app creates a sense of urgency with calls to action surrounding limited stock or promotions, ensuring high-quality and effective advertising. Tailor your advert for maximum relatability and appeal, with the Child Sport Ad Copy Creator.

To run this app online: [Child Sport Ad Copy Creator Online](https://hero.page/app/child-sport-ad-copy-creator-tailored-ad-copy-for-kid's-sports/CcwtrEPgn6eEAsz5qYaC)

[![Run Child Sport Ad Copy Creator Online](/assets/run.svg)](https://hero.page/app/child-sport-ad-copy-creator-tailored-ad-copy-for-kid's-sports/CcwtrEPgn6eEAsz5qYaC)

To learn more about AI Apps for Product Marketer use-cases in the Children's Sports & Outdoor Activities industry, read [How to Amplify Children's Sports Marketing with AI Tools](https://hero.page/blog/ai/children's-sports-and-outdoor-activities/how-to-amplify-children's-sports-marketing-with-ai-tools/170788)

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
npx hero run ./child_sport_ad_copy_creator.heroml
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
hero run ./child_sport_ad_copy_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./child_sport_ad_copy_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./child_sport_ad_copy_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./child_sport_ad_copy_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

