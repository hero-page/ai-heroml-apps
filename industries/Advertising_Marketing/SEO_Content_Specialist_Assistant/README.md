# SEO Content Specialist Assistant

SEO Content Specialist Assistant, an AI-Driven SEO Content Optimizer, allows users to define their needs in detailed prompts. The app then creates sophisticated, SEO-rich articles, custom-designed from user input. These articles are not only top-quality, based on well-researched data and valuable information on SEO practices, but are also structurally optimized for SEO. Exceptional feature of this app is its holistic SEO-focus, extending from content creation to backend technicalities such as strategic keyword density, placement, meta details, and URL structures.

To run this app online: [SEO Content Specialist Assistant Online](https://hero.page/app/seo-content-specialist-assistant-ai-driven-seo-content-optimizer/fCEjG7z9nWojc6DuG73D)

To learn more about AI Apps for SEO Specialist use-cases in the Advertising & Marketing industry, read [How to Generate SEO Keyword Reports and Optimized Articles with AI](https://hero.page/blog/ai/advertising-and-marketing/how-to-generate-seo-keyword-reports-and-optimized-articles-with-ai/170717)

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
npx hero run ./seo_content_specialist_assistant.heroml
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
hero run ./seo_content_specialist_assistant.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./seo_content_specialist_assistant.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./seo_content_specialist_assistant.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./seo_content_specialist_assistant.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for SEO Content Specialist Assistant
```

In order to write an SEO-optimized article for the Advertising & Marketing industry, specifically for a SEO specialist, follow the sequence of steps provided.

Start with an engaging title for the article. It should include the primary keyword: {{primary_keyword}}.

Here's some more context about the SEO-optimized Article:
Primary Keyword: {{primary_keyword}}
Theme: {{theme}}
Secondary Keywords: {{secondary_keywords}}

->>>>

The title of our SEO-optimized article for the SEO Specialist in the Advertising & Marketing industry includes the primary keyword is:

Title:
{{step_1}}

Next, craft an introduction, providing an overview of the theme: {{theme}} of the article. Include the primary keyword from the title in the introduction, to ignite curiosity and engage the reader.

->>>>

The title and introduction of our article are:

Title:
{{step_1}}

Introduction:
{{step_2}}

In the body of the article, craft headers and subheaders. These should contain secondary keywords: {{secondary_keywords}} aligning them with the main topic.

->>>>

The title, introduction, and headers for our SEO optimised article are:

Title:
{{step_1}}

Introduction:
{{step_2}}

Headers and Subheaders:
{{step_3}}

Let's provide comprehensive and well-researched information related to the theme: {{theme}}. This part may discuss data or current trends in the SEO industry, positioning the SEO specialist as an expert in their field.

->>>>

In our SEO optimised article, we have:

Title:
{{step_1}}

Introduction:
{{step_2}}

Headers and Subheaders:
{{step_3}}

Article Body:
{{step_4}}

Incorporate SEO best practices in the article, such as keyword positioning and density. The primary keyword: {{primary_keyword}} should appear in the first 100 words, and both primary and secondary keywords: {{secondary_keywords}} should be naturally incorporated throughout the article.

->>>>

Our SEO optimised article now includes SEO best practices:

Title:
{{step_1}}

Introduction:
{{step_2}}

Headers and Subheaders:
{{step_3}}

Article Body with SEO practices:
{{step_5}}

Next, elaborate on the practical benefits of the subject matter, with a special emphasis on its relevance to the SEO industry. This part should answer "How does this information help a SEO specialist improve their practice?"

->>>>

Our SEO optimised article with the application and benefits of the subject matter is:

Title:
{{step_1}}

Introduction:
{{step_2}}

Headers and Subheaders:
{{step_3}}

Article Body with SEO practices:
{{step_5}}

Benefits and Applications:
{{step_6}}

Winding up, summarize the article by recapitulating key points related to {{theme}} and {{primary_keyword}} and conclude with a call-to-action, encouraging reader engagement or further exploration of the topic.


```

