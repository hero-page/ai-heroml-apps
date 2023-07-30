# SEO News Headline Creator

Boost your SEO strategy with SEO News Headline Creator - an AI-driven app designed for media and news organizations! Specify variables for your news article and let the AI do the magic! It creates customized, eye-catching, accurate, and SEO-optimized headlines. It incorporates industry-specific terminology and keywords, that potential readers might use in searches. The app demonstrates a deep understanding of SEO practices, making your headlines not only captivating but relevant and searchable!

To run this app online: [SEO News Headline Creator Online](https://hero.page/app/seo-news-headline-creator-ai-driven-seo-news-headline-generator/79z2NytlD9FKdrwkKnT7)

[![Run SEO News Headline Creator Online](/assets/run.svg)](https://hero.page/app/seo-news-headline-creator-ai-driven-seo-news-headline-generator/79z2NytlD9FKdrwkKnT7)

To learn more about AI Apps for Editor use-cases in the Media & News Organizations industry, read [How to Elevate Editorial Work with AI-driven Guidelines, Reviews, and Headlines](https://hero.page/blog/ai/media-and-news-organizations/how-to-elevate-editorial-work-with-ai-driven-guidelines-reviews-and-headlines/171024)

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
npx hero run ./seo_news_headline_creator.heroml
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
hero run ./seo_news_headline_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./seo_news_headline_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./seo_news_headline_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./seo_news_headline_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

