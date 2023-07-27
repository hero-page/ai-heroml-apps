# Children's Book Cover Feedback AI

Children's Book Cover Feedback AI is a specialized app for custom AI analysis of kids' book covers. Users can input specific variables to get detailed, high-quality content about their book cover's design. The AI will provide feedback about initial impact, key elements such as title and author name, color scheme, style, and specific design flaws. Additionally, the AI summarizes the strong points and areas that require improvement and suggests practical enhancements. The app provides a deep critique that goes beyond basic impressions, focusing on specific elements like impact, title presentation, and color scheme. The unique attribute of this app is its ability to provide feedback specialized for children's and young adult books.

To run this app online: [Children's Book Cover Feedback AI Online](https://hero.page/app/children's-book-cover-feedback-ai-custom-ai-analysis-for-kids'-covers/A4S3xfysIo59bdx1q8o2)

[![Run Children's Book Cover Feedback AI Online](/assets/run.svg)](https://hero.page/app/children's-book-cover-feedback-ai-custom-ai-analysis-for-kids'-covers/A4S3xfysIo59bdx1q8o2)

To learn more about AI Apps for Editor use-cases in the Children's Storybooks - Young Adult Novels industry, read [How to Improve Children's Book Publishing with AI Editing and Marketing](https://hero.page/blog/ai/children's-storybooks-young-adult-novels/how-to-improve-children's-book-publishing-with-ai-editing-and-marketing/170806)

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
npx hero run ./childrens_book_cover_feedback_ai.heroml
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
hero run ./childrens_book_cover_feedback_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./childrens_book_cover_feedback_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./childrens_book_cover_feedback_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./childrens_book_cover_feedback_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

