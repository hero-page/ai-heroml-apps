# Children's Learning Content Ad Generator

This robust app, Children's Learning Content Ad Generator, leverages AI to create personalized, high-quality adverts for children's education materials. Users specify variables in prompts, and the app intelligently crafts content emphasizing product features, benefits, unique selling aspects, and an appropriate age range. What sets it apart is the integration of credibility-enhancing details about the product's creator and testimonials from satisfied users or experts. It creates visually appealing, interest-piquing scenarios and concludes with a compelling call to action for a complete advertising experience.

To run this app online: [Children's Learning Content Ad Generator Online](https://hero.page/app/children's-learning-content-ad-generator-ai-powered-child-education-ad-creator/5eW7rOxpxcnaWb4imbeg)

[![Run Children's Learning Content Ad Generator Online](/assets/run.svg)](https://hero.page/app/children's-learning-content-ad-generator-ai-powered-child-education-ad-creator/5eW7rOxpxcnaWb4imbeg)

To learn more about AI Apps for Product Marketer use-cases in the Children's Books & Learning Materials industry, read [How to Supercharge Children's Learning Material Marketing with AI](https://hero.page/blog/ai/children's-books-and-learning-materials/how-to-supercharge-children's-learning-material-marketing-with-ai/170779)

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
npx hero run ./childrens_learning_content_ad_generator.heroml
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
hero run ./childrens_learning_content_ad_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./childrens_learning_content_ad_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./childrens_learning_content_ad_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./childrens_learning_content_ad_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Children's Learning Content Ad Generator
```
Your task is to write a "Ad Copy" for the "Children's Books & Learning Materials" industry, specifically for a "Product Marketer". Let's begin by coming up with an engaging headline that sparks interest and focuses on the product's main selling point: {{product_main_selling_point}}.

Here's some more context about the Ad Copy:
Product Main Selling Point: {{product_main_selling_point}}
Product Description: {{product_description}}
Product Key Features: {{product_key_features}}
Educational Benefits: {{educational_benefits}}
Unique Selling Proposition: {{unique_selling_proposition}}
Age Range: {{age_range}}
Creator Information: {{creator_information}}
Use Case Scenario: {{use_case_scenario}}
Testimonials: {{testimonials}}
Call To Action: {{call_to_action}}

->>>>

The following is the headline for our "Ad Copy":

Headline:
{{step_1}}

Next, create an introduction that briefly explains the product: {{product_description}} and its key features: {{product_key_features}}.

->>>>

For our "Ad Copy", we now have a headline and an introduction:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Now, it's time to describe the benefits of using the product. Portray the educational value it can offer children, such as enhancing learning, making education fun, developing skills, and augmenting knowledge: {{educational_benefits}}.

->>>>

The "Ad Copy" for our product so far includes the headline, introduction, and the educational benefits:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Educational Benefits:
{{step_3}}

Next, elaborate on the unique selling proposition, stating what differentiates our product from competitors: {{unique_selling_proposition}}.

->>>>

The "Ad Copy" for our product advances with the addition of the unique selling proposition alongside the headline, introduction, and educational benefits:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Educational Benefits:
{{step_3}}

Unique Selling Proposition:
{{step_4}}

Now, let's clearly define the age range suitable for the product: {{age_range}}, keeping in mind its importance in the choice of children's books and learning materials.

->>>>

Here's what our "Ad Copy" looks like so far, with the addition of a defined age range:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Educational Benefits:
{{step_3}}

Unique Selling Proposition:
{{step_4}}

Suitable Age Range:
{{step_5}}

Following that, provide information about the author, illustrator, or manufacturer: {{creator_information}}, to augment product's credibility.

->>>>

So far, our "Ad Copy" includes the following:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Educational Benefits:
{{step_3}}

Unique Selling Proposition:
{{step_4}}

Suitable Age Range:
{{step_5}}

Creator Information:
{{step_6}}

Now, create a compelling story or scenario reflecting the beneficial usage of the product: {{use_case_scenario}}.

->>>>

Our product's "Ad Copy" continues to take shape:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Educational Benefits:
{{step_3}}

Unique Selling Proposition:
{{step_4}}

Suitable Age Range:
{{step_5}}

Creator Information:
{{step_6}}

Use Case Scenario:
{{step_7}}

We're almost there. Incorporate testimonials, if available, from satisfied customers, educators, or experts to validate the product's effectiveness: {{testimonials}}.


```

