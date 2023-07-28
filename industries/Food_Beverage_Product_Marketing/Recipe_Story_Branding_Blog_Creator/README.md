# Recipe Story & Branding Blog Creator

Craft sumptuous food narratives with Recipe Story & Branding Blog Creator. Use the AI-driven app to weave seamless, engaging tales around your recipes. Tailor prompts to get a detailed, narrative-styled blog post featuring captivating introductions, exhaustive ingredient lists with potential substitutions, easy-to-follow cooking instructions, handy tips, brand mentions, and a well-placed call-to-action. The app infuses each recipe with an emotional depth, referencing cultural backgrounds or personal anecdotes, ultimately serving a satisfying blend of culinary art and subtle brand promotion.

To run this app online: [Recipe Story & Branding Blog Creator Online](https://hero.page/app/recipe-story-and-branding-blog-creator-culinary-storytelling-and-branding-wizard/2hW9ic5UAa3zbBhpK7I9)

[![Run Recipe Story & Branding Blog Creator Online](/assets/run.svg)](https://hero.page/app/recipe-story-and-branding-blog-creator-culinary-storytelling-and-branding-wizard/2hW9ic5UAa3zbBhpK7I9)

To learn more about AI Apps for Content Creator use-cases in the Food & Beverage Product Marketing industry, read [How to Elevate Food Marketing with AI-Driven Recipe Blogs, Social Ads, and Reviews](https://hero.page/blog/ai/food-and-beverage-product-marketing/how-to-elevate-food-marketing-with-ai-driven-recipe-blogs-social-ads-and-reviews/170883)

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
npx hero run ./recipe_story_and_branding_blog_creator.heroml
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
hero run ./recipe_story_and_branding_blog_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./recipe_story_and_branding_blog_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./recipe_story_and_branding_blog_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./recipe_story_and_branding_blog_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

