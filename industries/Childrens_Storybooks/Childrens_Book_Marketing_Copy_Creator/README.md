# Children's Book Marketing Copy Creator

Optimize your children's book promotion with AI! Our app, Children's Book Marketing Copy Creator, smartly uses AI to generate high-quality, tailored content for your storybook. Providing a catchy headline, overview, character outline, theme review, and preview. It uniquely infuses educational value and a compelling call-to-action. It crafts engaging copies that captivate both children and parents, boosting their desire to buy. With a blend of creativity and marketing savvy, this tool enhances your book's appeal.

To run this app online: [Children's Book Marketing Copy Creator Online](https://hero.page/app/children's-book-marketing-copy-creator-ai-powered-children's-book-promotion/QiSqr7IaMBsWZA40uy4h)

[![Run Children's Book Marketing Copy Creator Online](/assets/run.svg)](https://hero.page/app/children's-book-marketing-copy-creator-ai-powered-children's-book-promotion/QiSqr7IaMBsWZA40uy4h)

To learn more about AI Apps for Publisher use-cases in the Children's Storybooks industry, read [How to Amplify Children's Book Marketing with AI Strategies](https://hero.page/blog/ai/children's-storybooks/how-to-amplify-children's-book-marketing-with-ai-strategies/170791)

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
npx hero run ./childrens_book_marketing_copy_creator.heroml
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
hero run ./childrens_book_marketing_copy_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./childrens_book_marketing_copy_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./childrens_book_marketing_copy_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./childrens_book_marketing_copy_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

