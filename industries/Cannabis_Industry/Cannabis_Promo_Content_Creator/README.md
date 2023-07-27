# Cannabis Promo Content Creator

Cannabis Promo Content Creator is your AI-driven cannabis campaign creator tool. Fully customizable, this high-tech app can generate a promotional campaign for your cannabis dispensary. Feed in specific variables to highlight your unique products, special promotions, history, mission, or the benefits of your offerings. The AI will craft a comprehensive output promoting responsible use while abiding by cannabis laws, and ensuring your contact details are clear. This strategic content marketing tool aims to attract potential consumers, carrying a focussed theme around your unique product or special offering.

To run this app online: [Cannabis Promo Content Creator Online](https://hero.page/app/cannabis-promo-content-creator-ai-driven-cannabis-campaign-creator/SMnEGynko6jSJG6dho36)

[![Run Cannabis Promo Content Creator Online](/assets/run.svg)](https://hero.page/app/cannabis-promo-content-creator-ai-driven-cannabis-campaign-creator/SMnEGynko6jSJG6dho36)

To learn more about AI Apps for Dispensary Manager use-cases in the Cannabis Industry industry, read [How to Amplify Cannabis Marketing with AI Tools](https://hero.page/blog/ai/cannabis-industry/how-to-amplify-cannabis-marketing-with-ai-tools/170770)

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
npx hero run ./cannabis_promo_content_creator.heroml
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
hero run ./cannabis_promo_content_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./cannabis_promo_content_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./cannabis_promo_content_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./cannabis_promo_content_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Cannabis Promo Content Creator
```
Your task is to write a promotional content for the Cannabis Industry, specifically for a Dispensary Manager.

Let's start by creating an engaging introduction that focuses on the promotional theme, {{promotional_theme}}. This might highlight a unique product, new arrivals, discounts, special promotions or a company event.

Here's some more context about the Promotional Content:
Promotional Theme: {{promotional_theme}}
Dispensary Background: {{dispensary_background}}
Product Information: {{product_information}}
Special Offers: {{special_offers}}
Legal Information: {{legal_information}}

->>>>

Now, we have generated an engaging introduction to our promotional content for a Dispensary Manager:

Introduction:
{{step_1}}

Next, we need to provide information about the background or history of your dispensary, its mission, and what sets it apart from competitors. This is where we'll provide our {{dispensary_background}} to show what distinguishes your business from others.

->>>>

At this stage, we have the introduction and background of our dispensary:

Introduction:
{{step_1}}

Dispensary Background:
{{step_2}}

Next, let's dive into the specifics of the product or service being promoted. Here we'll detail our {{product_information}}, discussing the advantages of your cannabis products, their unique features, and potential benefits to consumers.

->>>>

Now, we have the introduction, dispensary background and product information for our promotional content:

Introduction:
{{step_1}}

Dispensary Background:
{{step_2}}

Product Information:
{{step_3}}

To keep the content engaging, let's include some strategic mentions of special deals or offers that you have ongoing or upcoming. We will describe our {{special_offers}} to instill a sense of urgency and possible action from the reader.

->>>>

So far our promotional content has an introduction, background, product information and details about special offers:

Introduction:
{{step_1}}

Dispensary Background:
{{step_2}}

Product Information:
{{step_3}}

Special Offers:
{{step_4}}

Next, we must add a section that aims to educate the customer on the legalities related to cannabis use in your geographic area. With {{legal_information}}, we are promoting responsible use, but also positioning your dispensary as a knowledgeable authority.


```

