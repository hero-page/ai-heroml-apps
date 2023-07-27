# Craft Class Announcement Creator

Craft Class Announcement Creator is an AI-Powered app specifically designed for crafting engaging kids' class announcements. Convey key details with a captivating title, an expressive intro, unique class aspects, and practical info. Tailor-made for children's craft classes, the generated content adopts a vibrant, appealing tone, skillfully drawing kids and parents while underscoring the benefits of joining the class. This comprehensive tool ensures your announcements are well-structured, personalized, and effective.

To run this app online: [Craft Class Announcement Creator Online](https://hero.page/app/craft-class-announcement-creator-ai-powered-kids'-class-announcements/zGqteLYB3RfmsnLH4sTV)

[![Run Craft Class Announcement Creator Online](/assets/run.svg)](https://hero.page/app/craft-class-announcement-creator-ai-powered-kids'-class-announcements/zGqteLYB3RfmsnLH4sTV)

To learn more about AI Apps for Hobby Instructor use-cases in the Children's Crafts & Hobbies industry, read [How to Elevate Children's Craft Lessons with AI Tools](https://hero.page/blog/ai/children's-crafts-and-hobbies/how-to-elevate-children's-craft-lessons-with-ai-tools/170781)

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
npx hero run ./craft_class_announcement_creator.heroml
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
hero run ./craft_class_announcement_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./craft_class_announcement_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./craft_class_announcement_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./craft_class_announcement_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Craft Class Announcement Creator
```
Your task is to write a "Class Announcement" for the "Children's Crafts & Hobbies" industry, specifically for a "Hobby Instructor". 

First, let's generate a captivating header that mentions the hobby class title: {{hobby_class_title}}. This will be our first way of engaging potential attendees.

Here's some more context about the Class Announcement:
Hobby Class Title: {{hobby_class_title}}
Purpose Of Hobby Class: {{purpose_of_hobby_class}}
Structure Of Class: {{structure_of_class}}
Unique Aspects Of Class: {{unique_aspects_of_class}}
Details: {{details}}
Registration Info: {{registration_info}}
Benefits Of Joining: {{benefits_of_joining}}

->>>>

With this class announcement on our hands, we have a captivating header:

Header:
{{step_1}}

Now, compose an engaging introduction that outlines the purpose of the class, focusing on the outcomes potential attendees could achieve or create: {{purpose_of_hobby_class}}.

->>>>

In our "Class Announcement", we now have an engaging header and introduction:

Header:
{{step_1}}

Introduction:
{{step_2}}

Next, detail the structure of the class, mention sequence of activities and the method of instruction. Also, highlight the key craft or hobby skills attendees will gain: {{structure_of_class}}.

->>>>

Our class announcement has a header, an introduction, and the structure of the class:

Header:
{{step_1}}

Introduction:
{{step_2}}

Structure of class:
{{step_3}}

Now, integrate what makes your class unique: talk about your teaching method, your experience in the field, or any fun aspects of the class: {{unique_aspects_of_class}}.

->>>>

So far, we have a header, introduction, class structure, and unique selling points for our class announcement:

Header:
{{step_1}}

Introduction:
{{step_2}}

Structure of Class:
{{step_3}}

Unique Aspects of Class:
{{step_4}}

Next, present practical information such as the class location, timing, targeted age group, and skill level required, if any: {{details}}.

->>>>

Our "Class Announcement" presently has a header, introduction, class structure, unique selling points and practical information:

Header:
{{step_1}}

Introduction:
{{step_2}}

Structure of Class:
{{step_3}}

Unique Aspects of Class:
{{step_4}}

Details:
{{step_5}}

Onward, provide instructions for registration and payment processes, and don't forget to include the cut-off date: {{registration_info}}.

->>>>

Now, our "Class Announcement" has a header, introduction, class structure, unique selling points, practical information, and registration information:

Header:
{{step_1}}

Introduction:
{{step_2}}

Structure of Class:
{{step_3}}

Unique Aspects of Class:
{{step_4}}

Details:
{{step_5}}

Registration Info:
{{step_6}}

Finally, convey your enthusiasm for the class and summarize the benefits of joining: {{benefits_of_joining}}. End on a motivating note to encourage sign-ups.


```

