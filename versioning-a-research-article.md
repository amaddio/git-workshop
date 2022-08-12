# Versioning a Research Article

## Docs like Code

You can take advantages of Git's versioning feature when you write a research article. A requirement is that you have to write your article in a non proprietary software (Microsoft Word etc.). That means that the file that you are writing in must be plain text / machine readable so that Git can version / diff the files properly. Otherwise you would only have binary changes which can not be individually merged.

I suggest you use Markdown or LaTeX. To help you get started I suggest you to use Overleaf which takes away all the hassle that comes along with writing LaTeX and setting-up a base envirnment. If you don't already have one, create an account at https://overleaf.com/.

__Note__: The principle to treat reasearch Articles (Documents) like software code is called: _Docs like Code_

# Overleaf

Connect to your Overleaf (Git) project.

- go to your project
  - initialize a Git repo if not already done: `git init`
- get the git clone url by looking at the overleaf project and opening the Overleaf menu
- add it as a submodule to your working directory, where you store your article
  - `git submodule add <your-clone-url->`

Whenever you change files in the Overleaf editor, it will create a commit. You can prevent cluttering up your vesrion history by writing locally instead of remotely in the Overleaf editor. Once you want to generate a new PDF (remotely), commit and push your changes and generate the PDF in overleaf.
