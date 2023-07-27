# Children's Book Press Release Maker

The Children's Book Press Release Maker uses cutting-edge AI technology to produce comprehensive, custom press releases. Users can input prompts, like title, author, and plot synopsis, to orchestrate a robust overview of their storybook. The app expands on basics, highlighting unique selling points, early reviews, and purchasing details, creating a 360-degree picture of the book. It further sets itself apart by focusing exclusively on children's books, improving the overall output quality.

To run this app online: [Children's Book Press Release Maker Online](https://hero.page/app/children's-book-press-release-maker-comprehensive-ai-storybook-press-release/aYQ5jHDZOBRTKGF9FHZx)

[![Run Children's Book Press Release Maker Online](/assets/run.svg)](https://hero.page/app/children's-book-press-release-maker-comprehensive-ai-storybook-press-release/aYQ5jHDZOBRTKGF9FHZx)

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
npx hero run ./childrens_book_press_release_maker.heroml
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
hero run ./childrens_book_press_release_maker.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./childrens_book_press_release_maker.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./childrens_book_press_release_maker.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./childrens_book_press_release_maker.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

