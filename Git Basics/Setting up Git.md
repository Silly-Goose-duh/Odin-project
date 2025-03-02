# Introduction
Git is a very popular version control system. You’ll become very familiar with this piece of software throughout TOP, so don’t worry too much about understanding it at this point. There are many lessons focused on Git later in the curriculum.

GitHub is a service that allows you to upload, host, and manage your code using Git with a nice web interface.

Even though GitHub and Git sound similar, they are not the same or even created by the same company.

## Step 1: Install Git
Click the Operating System you have chosen below:
- Linux
- MacOS
- ChromeOS

## Step 2: Configure Git and GitHub

### Step 2.1: Create a GitHub account
Go to [GitHub.com](https://github.com/) and create an account! During the account setup, it will ask you for an email address. This needs to be a real email, and it will be used by default to identify your contributions. If you are privacy-conscious or just don’t want your email address to be publicly available, make sure you tick the following two boxes on the Email Settings page after you have signed in:

- **Keep my email addresses private**
- **Block command line pushes that expose my email**

Having these two options enabled will prevent accidentally exposing your personal email address when working with Git and GitHub.

You may also notice an email address under the **Keep my email addresses private** option. This is your private GitHub email address. If you plan to use this, make note of it now as you will need it when setting up Git in the next step.

### Step 2.2: Setup Git
For Git to work properly, we need to let it know who we are so that it can link a local Git user (you) to GitHub. The commands below will configure Git. Be sure to enter your own information inside the quotes (but include the quotation marks!). If you chose to keep your email private on GitHub, use your special private GitHub email from step 2.1.

```sh
git config --global user.name "Your Name"
git config --global user.email "yourname@example.com"
```

For example, if you set your email as private on GitHub, the second command will look something like this:

```sh
git config --global user.email "123456789+odin@users.noreply.github.com"
```

GitHub recently changed the default branch on new repositories from `master` to `main`. Change the default branch for Git using this command:

```sh
git config --global init.defaultBranch main
```

You’ll also likely want to set your default branch reconciliation behavior to merging. Run the below command:

```sh
git config --global pull.rebase false
```

To verify that things are working properly, enter these commands:

```sh
git config --get user.name
git config --get user.email
```

### For macOS Users
Run these two commands to tell Git to ignore `.DS_Store` files:

```sh
echo .DS_Store >> ~/.gitignore_global
git config --global core.excludesfile ~/.gitignore_global
```

### Step 2.3: Create an SSH key
If you have already set up an SSH key pair with GitHub on a different machine, you can follow these instructions again to set up another key pair and register it with GitHub.

First, check if you already have an Ed25519 algorithm SSH key installed:

```sh
ls ~/.ssh/id_ed25519.pub
```

If a message appears in the console containing the text “No such file or directory”, then you do not yet have an SSH key, and you will need to create one. To create a new SSH key, run the following command inside your terminal:

```sh
ssh-keygen -t ed25519
```

When it prompts you for a location to save the generated key, just press **Enter**.

Next, it will ask you for a password. You can enter one if you wish, but it’s not required. If you choose not to use a password, just hit **Enter** without typing anything.

### Step 2.4: Link your SSH key with GitHub
Log into GitHub, go to **Settings** > **SSH and GPG keys**, and click **New SSH Key**.

Now, copy your public SSH key:

```sh
cat ~/.ssh/id_ed25519.pub
```

Highlight and copy the entire output. Then, paste the key into GitHub's key field, keep the key type as **Authentication Key**, and click **Add SSH key**.

### Step 2.5: Testing your key
Test your SSH connection with GitHub:

```sh
ssh -T git@github.com
```

If successful, you will see:

```
Hi username! You’ve successfully authenticated, but GitHub does not provide shell access.
```

## Step 3: Let us know how it went!
You’ve completed the basic installation section, good job! As you progress through the Paths, there will be other tools to install, so keep an eye out!

You probably felt like you were way in over your head, and you probably didn’t understand much of what you were doing. That’s 100% normal. Hang in there. You can do this! And we’ve got your back.

## Additional Resources
This section contains helpful links to related content. It isn’t required, so consider it supplemental.

- [Understanding SSH Key Pairs](https://www.ssh.com/academy/ssh/keygen) - A secure network protocol that uses public-key cryptography.
- [Asymmetric Encryption - Simply Explained](https://www.youtube.com/watch?v=AQDCe585Lnc) - A short video explaining Asymmetric Encryption.

