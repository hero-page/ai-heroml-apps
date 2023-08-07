# High School Humanities Interview Creator

Immerse in the experience of a high school humanities club member with the High School Humanities Interview Creator app. This unique application harnesses AI technology for generating customised, high-quality content. Users can specify variables, leading to engaging interviews that delve into the member's academic interests, community issues relevant to students, significant contributions, challenges, future plans and more. Experience deep insights from covering rarely discussed topics, opportunities to learn from their experiences, and gather advice for fellow students.

To run this app online: [High School Humanities Interview Creator Online](https://hero.page/app/high-school-humanities-interview-creator-customized-high-school-humanities-interviews/RDI9qTGW5E8KR6ejsB0T)

[![Run High School Humanities Interview Creator Online](/assets/run.svg)](https://hero.page/app/high-school-humanities-interview-creator-customized-high-school-humanities-interviews/RDI9qTGW5E8KR6ejsB0T)

To learn more about AI Apps for Newspaper Club Member use-cases in the High School Students - Humanities industry, read [How to Fuel High School Journalism With AI-Enhanced Writing](https://hero.page/blog/ai/high-school-students-humanities/how-to-fuel-high-school-journalism-with-ai-enhanced-writing/170956)

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
npx hero run ./high_school_humanities_interview_creator.heroml
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
hero run ./high_school_humanities_interview_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./high_school_humanities_interview_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./high_school_humanities_interview_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./high_school_humanities_interview_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```
