# Kids Learning Material Design AI

Kids Learning Material Design AI utilizes sophisticated artificial intelligence to generate a comprehensive design guide for children's learning materials. With user-specified variables, it produces highly-customized content, outlining the material's purpose, target audience, physical features, safety considerations, and more. Compliance with educational guidelines and unique approaches are also highlighted. What sets it apart is its emphasis on producing designs tailor-made for children's learning, ensuring safety and practicality while promoting innovation and sustainability.

To run this app online: [Kids Learning Material Design AI Online](https://hero.page/app/kids-learning-material-design-ai-ai-driven-children's-learning-material-design/dXR3VbIDMe07uO2eMJHx)

[![Run Kids Learning Material Design AI Online](/assets/run.svg)](https://hero.page/app/kids-learning-material-design-ai-ai-driven-children's-learning-material-design/dXR3VbIDMe07uO2eMJHx)

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
npx hero run ./kids_learning_material_design_ai.heroml
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
hero run ./kids_learning_material_design_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./kids_learning_material_design_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./kids_learning_material_design_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./kids_learning_material_design_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Kids Learning Material Design AI
```
Your task is to write a "Design Specification" for the "Children's Books & Learning Materials" industry, specifically for a "Product Designer". Start by creating an introduction that clearly defines the product's purpose in aiding the learning process: {{product_purpose}}.

Here's some more context about the Design Specification:
Product Purpose: {{product_purpose}}
Target Audience: {{target_audience}}
Product Features: {{product_features}}
Development Process: {{development_process}}
Safety Considerations: {{safety_considerations}}

->>>>

With the product's purpose established: 

Product Purpose:
{{step_1}}

Next, describe the intended target audience, detailing the age range of children and their possible educational level: {{target_audience}}.

->>>>

So far, we have defined a purpose for our product and identified the target audience: 

Product Purpose:
{{step_1}}

Target Audience:
{{step_2}}

Our next task is to describe the product features. This section should entail detailed descriptions of the visual and functional features of the product that make it appealing and engaging to the target user: {{product_features}}.

->>>>

We have identified the product purpose, our target audience, and outlined the product's features:

Product Purpose:
{{step_1}}

Target Audience:
{{step_2}}

Product Features:
{{step_3}}

Then, present the proposed development process which should detail specific steps for the product's creation and assembly: {{development_process}}.

->>>>

In our Design Specification, we have the product's purpose, target audience, features, and a detailed development process:

Product Purpose:
{{step_1}}

Target Audience:
{{step_2}}

Product Features:
{{step_3}}

Development Process:
{{step_4}}

Now, discuss the safety considerations specific to the age group of the target audience. This should include choices of materials, paint, manufacturing processes, assembly, and packaging: {{safety_considerations}}.

->>>>

In our Design Specification, this is what we have thus far:

Product Purpose:
{{step_1}}

Target Audience:
{{step_2}}

Product Features:
{{step_3}}

Development Process:
{{step_4}}

Safety Considerations:
{{step_5}}

Finally, we need to conclude the Design Specification with a summary that reinforces the product's purpose and includes a list of deliverables expected from the Product Designer.


```

