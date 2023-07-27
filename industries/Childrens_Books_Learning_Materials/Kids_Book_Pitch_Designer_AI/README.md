# Kids' Book Pitch Designer AI

Kids' Book Pitch Designer AI, a Persuasive AI for Children's Education, is an app designed to create distinct and compelling pitches for children's books. Users can specify variables to generate custom content with AI technology. Its unique quality is the ability to emphasize children's educational benefits, crafting persuasive pitches that highlight the product's educational value, target demographic, and potential for future expansion.

To run this app online: [Kids' Book Pitch Designer AI Online](https://hero.page/app/kids'-book-pitch-designer-ai-persuasive-ai-for-children's-education/nCWfRc7yatRZgP6ivDuJ)

[![Run Kids' Book Pitch Designer AI Online](/assets/run.svg)](https://hero.page/app/kids'-book-pitch-designer-ai-persuasive-ai-for-children's-education/nCWfRc7yatRZgP6ivDuJ)

To learn more about AI Apps for Product Designer use-cases in the Children's Books & Learning Materials industry, read [How to Streamline Children's Learning Material Design with AI](https://hero.page/blog/ai/children's-books-and-learning-materials/how-to-streamline-children's-learning-material-design-with-ai/170778)

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
npx hero run ./kids_book_pitch_designer_ai.heroml
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
hero run ./kids_book_pitch_designer_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./kids_book_pitch_designer_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./kids_book_pitch_designer_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./kids_book_pitch_designer_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Kids' Book Pitch Designer AI
```
Your task is to write a "Product Pitch" for the "Children's Books & Learning Materials" industry, specifically for a "Product Designer". 

Let's start by introducing the type of children's book and learning material. Convey the details about {{product_type}} focusing on the genre, theme, and content.

Here's some more context about the Product Pitch:
Product Type: {{product_type}}
Unique Selling Point: {{unique_selling_point}}
Design Principles: {{design_principles}}
Educational Objectives: {{educational_objectives}}
Target Demographics: {{target_demographics}}
Additional Features: {{additional_features}}
Product Value: {{product_value}}
Expansion Potential: {{expansion_potential}}

->>>>

For your product pitch, we have initiated with an introduction of our product:

Product Type:
{{step_1}}

Next, we need to highlight the unique selling point of {{product_type}}. Explain how this product stands out from the competition or how it fills a gap in the current market: {{unique_selling_point}}.

->>>>

For our pitch, we have detailed:

Product Type:
{{step_1}}

Unique Selling Point:
{{step_2}}

Now, let's elaborate on the design aesthetics and principles that were used in creating the product. Discuss the look, feel, and usability of the product from a Product Designer's perspective.

->>>>

In our product pitch, we have:

Product Type:
{{step_1}}

Unique Selling Point:
{{step_2}}

Design Aesthetics and Principles:
{{step_3}}

Moving forward, we need to present how the product benefits children. Discuss the specific educational objectives and learning outcomes to be achieved with this product.

->>>>

For our product, we have described:

Unique Selling Point:
{{step_2}}

Design Aesthetics and Principles:
{{step_3}}

Educational Objectives:
{{step_4}}

Next, delve into the target demographics for the product. Describe the ideal age group and how the product caters to their specific learning styles or needs.

->>>>

So far, we have:

Design Aesthetics and Principles:
{{step_3}}

Educational Objectives:
{{step_4}}

Target Demographics:
{{step_5}}

Now, let's describe any additional features of the product. This could include interactive elements, robustness for young children's handling, or ease of storing and transporting.

->>>>

In our product pitch, we have:

Educational Objectives:
{{step_4}}

Target Demographics:
{{step_5}}

Additional Features:
{{step_6}}

Next, articulate how the product would be a valuable addition to bookshops, schools or homes. Utilize its unique features, design aspects and educational benefits in crafting this argument.

->>>>

The current status of our pitch includes:

Target Demographics:
{{step_5}}

Additional Features:
{{step_6}}

Product Value:
{{step_7}}

Finally, discuss the product's potential for expansion. This could include possibilities for extending the product line like sequels, series, or variations based on a theme.


```

