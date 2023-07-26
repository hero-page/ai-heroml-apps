# AI Dataset Description Compendium

AI Dataset Description Compendium uses AI to offer custom dataset analytics and insights. You can specify variables in your prompts. Get comprehensive summaries of AI & Machine Learning datasets, complete with details on origins, methodology, preprocessing, size, structure, key patterns, and prominent features. Understand dataset limitations or biases. The output is ideal for Data Scientists needing in-depth knowledge. Plus, access download information for immediate use. The high-quality content is uniquely thorough and practical.

To run this app online: [AI Dataset Description Compendium Online](https://hero.page/app/ai-dataset-description-compendium-ai-dataset-analytics-and-insights/n2VSxCBFKLycEzY0o1vi)

[![Run AI Dataset Description Compendium Online](/assets/run.svg)](https://hero.page/app/ai-dataset-description-compendium-ai-dataset-analytics-and-insights/n2VSxCBFKLycEzY0o1vi)

To learn more about AI Apps for Data Scientist use-cases in the Artificial Intelligence & Machine Learning industry, read [How to Streamline AI Dataset Reporting, Data Analysis, and Tutorial Creation](https://hero.page/blog/ai/artificial-intelligence-and-machine-learning/how-to-streamline-ai-dataset-reporting-data-analysis-and-tutorial-creation/170732)

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
npx hero run ./ai_dataset_description_compendium.heroml
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
hero run ./ai_dataset_description_compendium.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ai_dataset_description_compendium.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ai_dataset_description_compendium.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ai_dataset_description_compendium.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for AI Dataset Description Compendium
```
Your task is to write a "Dataset Description" for the "Artificial Intelligence & Machine Learning" industry, specifically for a "Data Scientist". 

Start with a clear introduction that explains what the dataset contains: {{dataset_content}}. Avoid diving into too much detail at this point.

Here's some more context about the Dataset Description:
Dataset Content: {{dataset_content}}
Data Sources: {{data_sources}}
Dataset Size And Structure: {{dataset_size_and_structure}}
Dataset Features: {{dataset_features}}
Dataset Limitations: {{dataset_limitations}}

->>>>

We've now written a clear introduction, which explains what the dataset contains:

Introduction:
{{step_1}}

Following the introduction, please provide an in-depth description of the data source(s): {{data_sources}}. This might include the original source of the data, how it was collected or generated, and any transformations or preprocessing steps that were applied to it.

->>>>

With our introduction in place, we've also described the data source(s) in depth:

Introduction:
{{step_1}}

Data Sources:
{{step_2}}

Create a section dedicated to explaining the size and structure of the dataset: {{dataset_size_and_structure}}. This should address the number and types of data points included in the dataset, the way in which the data is organized or structured, and any key patterns or characteristics that emerge from this structure.

->>>>

We have our introduction, a description of the data source, and now a detailed view of our dataset's size and structure:

Introduction:
{{step_1}}

Data Sources:
{{step_2}}

Dataset Size and Structure:
{{step_3}}

Next, describe the interesting or unique attributes or features of the dataset: {{dataset_features}}. Outline prominent variables in the data, how they are encoded, and their relevance in the context of AI & Machine Learning. Emphasize those aspects that would have particular interest to a Data Scientist.

->>>>

We have detailed the dataset's size and structure, now let's look at the description of the attributes and features:

Dataset Size and Structure:
{{step_3}}

Dataset Features:
{{step_4}}

Now, dedicate a section to explain any limitations or potential biases in the dataset: {{dataset_limitations}}. Include any missing data, imbalances, or potential biases in the dataset that could impact the result of data analysis or model training.

->>>>

We detailed the attributes and features of the dataset and provided an explanation of any limitations or potential biases:

Dataset Features:
{{step_4}}

Dataset Limitations:
{{step_5}}

Next, create a summary that recaps the key points about the dataset: {{dataset_content}}, {{data_sources}}, {{dataset_size_and_structure}}, {{dataset_features}}, and {{dataset_limitations}}. This should reemphasize why this dataset is important and how it could be used in the context of AI & Machine Learning.


```

