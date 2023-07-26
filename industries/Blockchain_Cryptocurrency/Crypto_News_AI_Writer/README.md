# Crypto News AI Writer

Delve into blockchain with Crypto News AI Writer, your go-to source for AI-generated cryptocurrency journalism. Specify variables to create custom tailored news pieces covering cryptocurrency and blockchain nuances. Equipped with intelligent AI, the app generates high-quality content, incorporating expert views, industry jargon, and future trends for a distinct crypto journalism experience. It responsibly cites information, ensuring you're always well-informed.

To run this app online: [Crypto News AI Writer Online](https://hero.page/app/crypto-news-ai-writer-ai-generated-cryptocurrency-journalism/E3TJdApnzPk3xz3SXUQJ)

[![Run Crypto News AI Writer Online](/assets/run.svg)](https://hero.page/app/crypto-news-ai-writer-ai-generated-cryptocurrency-journalism/E3TJdApnzPk3xz3SXUQJ)

To learn more about AI Apps for Crypto Journalist use-cases in the Blockchain & Cryptocurrency industry, read [How to Generate Stellar Crypto Articles, Interviews and Analysis with AI](https://hero.page/blog/ai/blockchain-and-cryptocurrency/how-to-generate-stellar-crypto-articles-interviews-and-analysis-with-ai/170753)

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
npx hero run ./crypto_news_ai_writer.heroml
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
hero run ./crypto_news_ai_writer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./crypto_news_ai_writer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./crypto_news_ai_writer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./crypto_news_ai_writer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Crypto News AI Writer
```
Start by writing a headline for the "News Article" that captures the main theme of the article and invokes curiosity in the reader.

Here's some more context about the News Article:
Headline: {{headline}}
Intro Overview: {{intro_overview}}
Article Topic: {{article_topic}}
Expert Views: {{expert_views}}
Article Conclusion: {{article_conclusion}}

->>>>

We have a headline for our news article:

Headline:
{{step_1}}

Next, write an introduction that gives an overview of the topic and its relevance in the blockchain and cryptocurrency industry. Mention recent events, trends or statistics.

->>>>

We have the headline and introduction for our news article:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Moving on, let's write the body of the article. Divide it into different subheadings for better readability. It should delve into the details of the {{article_topic}}, and might include aspects such as its impact on the cryptocurrency market, its implications for traders or investors, any regulatory considerations, and how it compares with other similar developments.

->>>>

We have the headline, introduction, and body of our news article:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Body:
{{step_3}}

Now incorporate key industry-specific jargon and concepts such as block mining, hash rate, smart contracts, ICOs, digital wallets, or any other terms relevant to the {{article_topic}} within the body of the article.

->>>>

Our news article now includes relevant key industry-specific terms:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Body with key industry-specific jargon:
{{step_4}}

Next, let's incorporate expert opinions and quotes to substantiate the points in your article. Interview industry leaders, analysts or blockchain developers and use their thoughts to provide an authoritative voice to your article.

->>>>

Our news article now includes expert opinions:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Body with key industry-specific jargon and expert opinions:
{{step_5}}

Now it's time to conclude the article. Summarise the major points of the article, and offer a speculation or prediction of what these developments mean for the future of the industry.


```

