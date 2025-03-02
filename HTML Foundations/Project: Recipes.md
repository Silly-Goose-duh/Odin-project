# Introduction

It’s time to practice all of the HTML knowledge you have acquired. In this project, you are going to build a basic recipe website.

The website will consist of a main index page which will have links to a few recipes. The website won’t look very pretty by the time you’ve finished but it’s important to keep in mind that this project is just to build your HTML chops; we will revisit this project in the future to style it up with CSS.

## Setting up your project’s GitHub repository

As mentioned in the **Introduction to Git** lesson, you’ll want to organize all your projects like a portfolio and link them to GitHub so it can be seen by others.

### Be careful about creating files on GitHub

GitHub allows us to make changes directly on its site. If you do this after you have cloned the repository to your machine, it will cause your local code to be a version behind the remote, creating extra challenges when you push your work. Most of the time, you should be creating files locally.

As you progress in the course, you’ll learn how to handle these situations, but for now, it’s important to follow the instructions carefully to stay on the simple path.

If you do not know how to set up a repository, follow instruction steps 1 and 2 found in **Git Basics** to learn how, before carrying on with these steps:

1. Create a new repo for this project on GitHub.com and call it `odin-recipes` and choose the public option instead of the default private.
2. Clone that repository onto your local machine, inside the `repos` folder that you previously created in the **Git Basics** lesson. The command should look like:
   ```bash
   git clone git@github.com:username/odin-recipes.git
   ```
   (use SSH).
3. Now `cd` into the `odin-recipes` project directory that is now on your local machine.
4. Set up your `README.md` file and write a brief introduction describing what the current project is and what skills you will have demonstrated once you have completed it.

### If you are having trouble:

- All Git commands need to be run from inside your project’s folder (**Did you forget to `cd` into the `odin-recipes` folder?**).
- Ensure you followed the steps on how to create an SSH key to clone from GitHub with SSH.
- Refer to the workflow in the **Git Basics** lesson.

## Tips on when to commit

Don’t forget everything we went over in the **Commit Messages** lesson!

When you’re building your project, you will probably end up doing several `git add` + `git commit` cycles before being ready to push it up to GitHub with:

```bash
git push origin main
```

When writing code, it’s considered **best practice to commit early and often**. Commit every time you have a meaningful change in the code. This will create a timeline of your progress and show that your finished code didn’t appear out of nowhere.

After you have entered `git push origin main`, switch over to your browser and open your repository on GitHub. You should now see all the files you just pushed.

Okay, that’s enough Git for the moment – time to actually build stuff!

---

# Assignment

## Iteration 1: Initial Structure

1. Within the `odin-recipes` directory, create an `index.html` file.
2. Fill it out with the usual boilerplate HTML and add an `<h1>` heading `Odin Recipes` to the body.

## Iteration 2: Recipe Page

1. Create a new directory within the `odin-recipes` directory and name it `recipes`.
2. Create a new HTML file within the `recipes` directory and name it after the recipe it will contain (e.g., `lasagna.html`).
3. Be sure to include the usual boilerplate HTML.
4. Add an `<h1>` heading with the recipe’s name as its content.
5. Back in `index.html`, add a link to the recipe page you just created:
   ```html
   <a href="recipes/recipename.html">Recipe Title</a>
   ```
6. Add a link back to the index page on your recipe page for easier navigation:
   ```html
   <a href="../index.html">Home</a>
   ```

## Iteration 3: Recipe Page Content

Your new recipe page should have the following content:

1. An **image** of the finished dish under the `<h1>` heading.
2. A **Description** section with a paragraph or two describing the recipe.
3. An **Ingredients** section with an unordered list of the ingredients.
4. A **Steps** section with an ordered list of the steps needed to make the dish.

## Iteration 4: Add More Recipes

1. Add two more recipes with identical page structures to the first recipe page.
2. Update the `index.html` to include links to all recipes. Consider putting them inside an unordered list:
   ```html
   <ul>
       <li><a href="recipes/yourrecipe.html">Recipe Title 1</a></li>
       <li><a href="recipes/yourrecipe.html">Recipe Title 2</a></li>
       <li><a href="recipes/yourrecipe.html">Recipe Title 3</a></li>
   </ul>
   ```

---

# Viewing Your Project on the Web

To show your work to others, publish your site using GitHub Pages:

1. Ensure the main HTML file is named `index.html`.
2. Go to your GitHub repo and click **Settings**.
3. Click **Pages** in the left sidebar.
4. Change the **Branch** from `none` to `main` and click **Save**.
5. It may take a few minutes for your project to be accessible at:
   ```
   your-github-username.github.io/your-github-repo-name
   ```
6. If it does not publish after 1 hour, check:
   - Your `index.html` file is in the root of the repository.
   - GitHub Pages settings are correctly set.
   - Go to **Actions** in GitHub, and if there are no entries, reset the branch selection in **Pages** settings.

---

### A Final Note

When looking at other project submissions, remember:

- Many were created by experienced programmers or past students.
- Your project does **not** need to look like theirs.
- Focus on completing the requirements.
- Improve it later with CSS and JavaScript!

For more insights, read **“Learning Code”** from **“Becoming a TOP Success Story”**.
