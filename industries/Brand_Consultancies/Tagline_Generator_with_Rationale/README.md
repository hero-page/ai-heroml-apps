# Tagline Generator with Rationale

Tagline Generator with Rationale, an AI-powered, rationalized tagline creation tool, allows users to input specific variables, generating custom, high-quality content. Each creation strategically embodies the brand's message, engages the target audience and outlines the unique selling proposition. The app's exclusivity lies in its ability to provide a concise rationale for the taglines created, offering clear explanation on how it meets its outlined objectives, a feature not typically found in similar apps. This empowers users with a rational understanding of the strategic design behind their brand's taglines.

To run this app online: [Tagline Generator with Rationale Online](https://hero.page/app/tagline-generator-with-rationale-ai-powered-rationalized-tagline-creation/XgWA0uB67Wu9Hw3n02mw)

[![Run Tagline Generator with Rationale Online](/assets/run.svg)](https://hero.page/app/tagline-generator-with-rationale-ai-powered-rationalized-tagline-creation/XgWA0uB67Wu9Hw3n02mw)

To learn more about AI Apps for Copywriter use-cases in the Brand Consultancies industry, read [How to Harness AI for Dynamic Brand Storytelling, Engaging Taglines, and Persuasive Product Descriptions](https://hero.page/blog/ai/brand-consultancies/how-to-harness-ai-for-dynamic-brand-storytelling-engaging-taglines-and-persuasive-product-descriptions/170764)

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
npx hero run ./tagline_generator_with_rationale.heroml
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
hero run ./tagline_generator_with_rationale.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./tagline_generator_with_rationale.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./tagline_generator_with_rationale.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./tagline_generator_with_rationale.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Tagline Generator with Rationale
```
Write a "Tagline Creation" for the "Brand Consultancies" industry, specifically for a "Copywriter". 
Let's begin by writing a creative brief for a "Copywriter". The brief should include: The key message to be conveyed through the tagline ({{key_message}}), a description of the target audience ({{target_audience}}), and the unique selling proposition (USP) of the product or service ({{unique_selling_proposition}}).

Here's some more context about the Tagline Creation:
Key Message: {{key_message}}
Target Audience: {{target_audience}}
Unique Selling Proposition: {{unique_selling_proposition}}

->>>>

At this stage, we have a creative brief for the "Copywriter":

Creative Brief:
{{step_1}}

Next, focus on the emotional response you want to elicit from your {{target_audience}} and how to encapsulate the {{unique_selling_proposition}} effectively, to develop a list of potential taglines that resonate with the brand's key message.

->>>>

We have a creative brief and a list of potential taglines for the "Copywriter":

Creative Brief:
{{step_1}}

Potential Taglines:
{{step_2}}

Next, for each potential tagline, evaluate whether it aligns with the characteristics of a good tagline: It should be memorable, concise, give a strong message. Make sure it reflects the brand’s personality, keeping your {{target_audience}} and {{unique_selling_proposition}} in mind during this time.

->>>>

We have a set of evaluated taglines for the brand consultancies industry:

Creative Brief:
{{step_1}}

Evaluated Taglines:
{{step_3}}

Now, select the top choices from your list and test them against the business values and the brand promise. This will ensure your tagline communicates the brand ethos and your {{unique_selling_proposition}} in a way that would appeal to the {{target_audience}}.

->>>>

For the brand consultancies industry, we have a shortlist of selected taglines:

Creative Brief:
{{step_1}}

Selected Taglines:
{{step_4}}

Let's revise and polish the selected tagline for a "Copywriter". The final tagline should reflect the brand's tone and style. It should seamlessly incorporate the {{key_message}}, resonate with the {{target_audience}}, and reinforce the {{unique_selling_proposition}}.

->>>>

For the brand consultancies industry, we have a polished tagline:

Polished Tagline:
{{step_5}}

Let's finish the tagline creation process by conducting an external review. This could be focus groups, surveys, or one-on-one interviews. Strive for feedback from a variety of people from your {{target_audience}} to gauge if the crafted tagline aligns with the {{key_message}} and the {{unique_selling_proposition}}.


```

