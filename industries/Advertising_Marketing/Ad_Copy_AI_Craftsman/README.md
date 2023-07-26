# Ad Copy AI Craftsman

Ad Copy AI Craftsman is a powerful, AI-powered tool that lets users craft perfect, personalized ad copies. Highlight your ad writing prowess by setting specific variables and watch as the mastery of artificial intelligence delivers compelling, high-quality content. Stand out with captivating headlines, apt descriptions of client challenges, showcasing your unique skills and advantages. Amplify your credibility with expertly woven testimonials and invoke action with effective call-to-actions, backed by solid assurances. Whether it's converting leads into clients or simply piquing interest in your offerings, our AI-driven approach tailors your ad to fit your needs and the complex structure of the modern ad landscape.

To run this app online: [Ad Copy AI Craftsman Online](https://hero.page/app/ad-copy-ai-craftsman-ai-driven-ad-creation-mastery/zt4Bcuxgv9VhkFeIP46F)

[![Run Ad Copy AI Craftsman Online](/assets/run.svg)](https://hero.page/app/ad-copy-ai-craftsman-ai-driven-ad-creation-mastery/zt4Bcuxgv9VhkFeIP46F)

To learn more about AI Apps for Copywriter use-cases in the Advertising & Marketing industry, read [How to Supercharge Ad Creation, Email Campaigns, and Blog Posts with AI](https://hero.page/blog/ai/advertising-and-marketing/how-to-supercharge-ad-creation-email-campaigns-and-blog-posts-with-ai/170716)

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
npx hero run ./ad_copy_ai_craftsman.heroml
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
hero run ./ad_copy_ai_craftsman.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ad_copy_ai_craftsman.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ad_copy_ai_craftsman.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ad_copy_ai_craftsman.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Ad Copy AI Craftsman
```
Your task is to write an "Ad Copy" for the "Advertising & Marketing" industry, specifically for a "Copywriter". Let's begin with creating a compelling headline to hook in readers.

Here's some more context about the Ad Copy:
Hook Headline: {{hook_headline}}
Problem Description: {{problem_description}}
Product Features: {{product_features}}
Testimonial Reviews: {{testimonial_reviews}}
Call To Action: {{call_to_action}}
Assurance Point: {{assurance_point}}

->>>>

We've started our "Ad Copy" with a compelling headline:

Headline:
{{step_1}}

Next, let's draft a description that expands on the concept of our headline, demonstrating the issue your product or service solves.

->>>>

Our "Ad Copy" now has a compelling headline and a problem description:

Headline:
{{step_1}}

Problem Description:
{{step_2}}

Now, let's introduce your product or service, focusing on its unique selling points, benefits, and features that make it the best solution to the problem.

->>>>

Our "Ad Copy" so far includes a captivating headline, a description of the problem, and an introduction to your product or service:

Headline:
{{step_1}}

Problem Description:
{{step_2}}

Product Introduction:
{{step_3}}

Next, if available, include testimonials or client reviews highlighting beneficial results to foster trust with the audience.

->>>>

Now our "Ad Copy" has a strong structure that includes an enticing headline, a problem description, an introduction to your product or service, and supportive testimonials and reviews:

Headline:
{{step_1}}

Problem Description:
{{step_2}}

Product Introduction:
{{step_3}}

Testimonials and Reviews:
{{step_4}}

Our next task is to create a clear and powerful call-to-action, guiding readers on what they should do next.

->>>>

Our "Ad Copy" now includes an inviting headline, a problem description, a product introduction, testimonials, and a persuasive call-to-action:

Headline:
{{step_1}} 

Problem Description:
{{step_2}}

Product Introduction:
{{step_3}}

Testimonials and Reviews:
{{step_4}}

Call to Action:
{{step_5}}

To conclude our "Ad Copy", let's provide some sort of assurance, like a money-back guarantee or a free trial, to the reader to instill a sense of security in their decision.


```

