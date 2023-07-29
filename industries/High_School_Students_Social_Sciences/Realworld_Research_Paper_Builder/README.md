# Real-world Research Paper Builder

Real-world Research Paper Builder: Smart AI, Real-World Contextual Analysis is an innovative app that uses artificial intelligence to create customized high-quality research papers for high school students. Users are able to specify various parameters in their prompts, guiding the AI in generating a paper covering a specific research topic, a clear thesis statement, an organized body discussing key elements of the topic, data analysis, and a conclusion. The app also incorporates a bibliographical section and a discussion on societal or local issues related to the research topic for a broader understanding. This feature sets it apart, encouraging students to connect theory with real-world implications, deepening their understanding and awareness. Experience the revolution in academic writing!

To run this app online: [Real-world Research Paper Builder Online](https://hero.page/app/real-world-research-paper-builder-smart-ai-real-world-contextual-analysis/UPdMraNutiYIyqqbhKeL)

[![Run Real-world Research Paper Builder Online](/assets/run.svg)](https://hero.page/app/real-world-research-paper-builder-smart-ai-real-world-contextual-analysis/UPdMraNutiYIyqqbhKeL)

To learn more about AI Apps for Student use-cases in the High School Students - Social Sciences industry, read [How to Ace Research, History and Sociology Tasks with AI Tools](https://hero.page/blog/ai/high-school-students-social-sciences/how-to-ace-research-history-and-sociology-tasks-with-ai-tools/170967)

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
npx hero run ./real_world_research_paper_builder.heroml
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
hero run ./real_world_research_paper_builder.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./real_world_research_paper_builder.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./real_world_research_paper_builder.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./real_world_research_paper_builder.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

