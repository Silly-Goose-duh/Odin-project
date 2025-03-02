# Introduction
This lesson will explain the importance of good commit messages, how to write them, when to commit, and why having a history of good commits is so important!

# Lesson Overview
This section contains a general overview of topics that you will learn in this lesson:

- How to write a meaningful commit message.
- Why meaningful commit messages are important.
- When to commit.

# Are Commit Messages So Important They Deserve Their Own Lesson?
Yes! Let me give you a quick list of reasons why:

- When you are applying for jobs, employers will look through your projects on GitHub and they will look through your commit history. Having good commits as a novice developer will help you stand out.
- Having a good commit message history will allow you (or other developers working on your code) to quickly see what changes were made and why. This is useful if a bug is found in the code that needs to be fixed!
- Having a good commit message history will also be helpful if you come back to a project you were working on after stepping away from it for a while. You likely won’t remember your thought process and changes made when initially writing out the code.

# Bad vs. Good Commits
When it comes to writing commits, it is crucial to know how to write them effectively. Here’s an example of a bad commit message:

**Bad commit message:**
```
fix a bug
```
Even though it describes what you did, the message is too vague, which leaves the other developers on your team confused. A good commit message will explain the why behind your changes. In other words, a commit message describes what problem your changes solve and how it solves them.

Effective commits consist of two separate parts: a subject, and a body:

### Subject
A brief summary of the change you made to the project.
```
This is the change I made to the codebase
```
GitHub has a 72-character limit, so we recommend keeping your commits’ subjects within this amount.

### Body
A concise yet clear description of what you did.
- Describe the problem your commit solves and how.

Now that we learned the secret to creating a good commit message, let’s try and fix the commit message from earlier:

**Good commit message:**
```
Add missing link and alt text to the company's logo

Screen readers won't read the images to users with disabilities without this information.
```

Now, developers can gain a better understanding of this commit message because it does the following:

- Provides a subject that specifies your code’s action.
- Contains a body that provides a concise yet clear description of why the commit needed to be made.
- Separates the subject from the body with a new/blank line.

# How to Commit with a Subject and Body in the Message
Up until now, you’ve been told to commit with:
```
git commit -m "<message>"
```
To make a commit with a subject and body, the simplest way is to type:
```
git commit
```
Doing so will open a new Visual Studio Code tab if you had set Visual Studio Code as the Git editor. You can remove any comments and enter your multi-line messages. When you save and close the tab, your commit will be created.

# When to Commit
A good way to view a commit is like a “snapshot” of your code at the moment that it was made. That version of your code up to that point will be saved for you to revert back to or look back at.

### When should you commit?
- Every time you have a meaningful change in the code.
- When you fix a typo or a bug.
- When a piece of code starts functioning correctly.

This will create a timeline of your progress and show that your finished code didn’t appear out of nowhere.

There will come a time when you are working on a project and you FINALLY get something just right (this would be a good time to commit), and then maybe 30 seconds to a few days later it breaks. You have no idea what you changed, everything looks to be the same and you don’t remember editing that line, but alas, it isn’t working how you want it anymore. You’d be able to go back through your commit history and either revert your code back to the last commit you made when you first got that part working or go back and see what your code looked like at that point in time.

# Assignment
This article, [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/), covers all the main bases on how to write good commit messages. The whole article is great and informative, but the key section is **“The seven rules of a great commit message.”**

# Tips and Things to Remember
- Using VSCode as your text editor (you should have set this up in the Git Basics section) will allow you to easily make multi-line commit messages, see the character length of each line, and use spell check extensions to ensure correct spelling.
- Use an active voice: **“Fix card generator”**.
- Avoid using vague commit messages such as **“saved”** or **“updated”**.
- **Commit early and often!**

# Knowledge Check
The following questions are an opportunity to reflect on key topics in this lesson. If you can’t answer a question, click on it to review the material, but keep in mind you are not expected to memorize or master this knowledge.

1. What are two benefits of having well-written commit messages and a good commit history?
2. How many characters should the subject line of your commit message be?

# Additional Resources
This section contains helpful links to related content. It isn’t required, so consider it supplemental.

- One way to formulate high-information commit messages is to follow a template. **[Conventional commits](https://www.conventionalcommits.org/)** is one of many commit message templates that you can explore.
- Explore this amazing tutorial video on Conventional Commits ➔ **[Full Video Link](https://www.youtube.com/watch?v=FJ0F6ts1xTI)**. The video showcases the Conventional Commits template from the resource above. It also mentions creating releases and shows using something called “Yarn.” These two parts are out of scope for this part of the course, so don’t worry about them and instead focus on the commit template.

