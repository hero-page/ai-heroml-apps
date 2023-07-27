# Child Art Supplies Ad Creator

Unleash creativity with Child Art Supplies Ad Creator, equipped with AI technology. This savvy app empowers users to generate custom, high-quality ads for children's art supplies. Tailor each ad with specific variables for persuasive, attention-holding content. Highlight features, benefits, unique selling points and value for money, while reassuring parents about safety and quality. Engage your audience through a call to action and emphasis on the product's educational value and potential sustainability. Particularly, it addresses parental concerns, reflecting a nuanced view of the target audience's needs and desires.

To run this app online: [Child Art Supplies Ad Creator Online](https://hero.page/app/child-art-supplies-ad-creator-ai-powered-kid-friendly-art-ads/rtxGzb1srrgZP2C7mceO)

[![Run Child Art Supplies Ad Creator Online](/assets/run.svg)](https://hero.page/app/child-art-supplies-ad-creator-ai-powered-kid-friendly-art-ads/rtxGzb1srrgZP2C7mceO)

To learn more about AI Apps for Product Marketer use-cases in the Children's Art Supplies industry, read [How to Master AI-Driven Marketing in Children's Art Supplies](https://hero.page/blog/ai/children's-art-supplies/how-to-master-ai-driven-marketing-in-children's-art-supplies/170776)

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
npx hero run ./child_art_supplies_ad_creator.heroml
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
hero run ./child_art_supplies_ad_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./child_art_supplies_ad_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./child_art_supplies_ad_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./child_art_supplies_ad_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Child Art Supplies Ad Creator
```
Let's create an "Ad Copy" for the "Children's Art Supplies" industry for a "Product Marketer".

Firstly, generate a captivating headline for the ad copy about the art supplies. This headline should intrigue the reader and spark curiosity for further reading.

Here's some more context about the Ad Copy:
Headline: {{headline}}
Product Range Overview: {{product_range_overview}}
Product Features: {{product_features}}
Unique Selling Proposition: {{unique_selling_proposition}}
Call To Action: {{call_to_action}}
Reassuring Statement: {{reassuring_statement}}

->>>>

We have a compelling headline for our ad copy:

Headline:
{{step_1}}

Next, let's write a brief introduction that overviews the product range targeting children. This should outline the general attributes of the product(s) without delving into specifics.

->>>>

Now, we have both a compelling headline and a concise introduction for our ad copy:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Continuing, let's write a detailed product description to highlight the main features and benefits of the products. Ensure this description showcases the benefits from the perspective of children and their parents.

->>>>

So far for our ad copy, we have a headline, an introduction and now a detailed description of the product:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Product Description:
{{step_3}}

Let's now write a unique selling proposition. This should include the qualities that set these art supplies apart from competing products. The proposition should trigger desire and convince potential buyers about the value of the product for their children.

->>>>

In our ad copy, we have a headline, an overview, a detailed product description, and a unique selling proposition:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Product Description:
{{step_3}}

Unique Selling Proposition:
{{step_4}}

Next, let's include a call-to-action for the reader. This may be an invitation to purchase the product, subscribe to your newsletter or visit your website for further information.

->>>>

For our ad copy, we have an introduction, detailed product description, a unique selling proposition, and a call-to-action:

Introduction:
{{step_2}}

Product Description:
{{step_3}}

Unique Selling Proposition:
{{step_4}}

Call to Action:
{{step_5}}

To finalize, let's write a reassuring statement or guarantee. This should essentially confirm the product's quality, safety, or educational value, helping to alleviate any concerns that parents might have.


```

