# The WebLatex

![WebLatex](images/image.png)

> A complete alternative for Overleaf with VSCode + Web + Git Integration + Live Collaboration Support

- [The WebLatex](#the-weblatex)
  - [Screenshot](#screenshot)
  - [Why](#why)
    - [Just use overleaf](#just-use-overleaf)
  - [Installation Instructions](#installation-instructions)
  - [Where is my PDF?](#where-is-my-pdf)
  - [Editor Instructions](#editor-instructions)
  - [To use with LuaLatex or any other Tex program](#to-use-with-lualatex-or-any-other-tex-program)
  - [Live Collaboration](#live-collaboration)
  - [Configuration](#configuration)
  - [More Features and Configuration](#more-features-and-configurations)
  - [Contribution](#contribution)
  - [What's Next](#whats-next)
  - [Contact](#contact)

## Screenshot

![Screenshot](images/screenshot.png)

## Why

Do you use latex as your Resume builder / Research Project / Documentation / Article or any Documentation? Then you probably sometime wondered in your life if you could use the advantages of git. You could just commit your changes and roll back to older versions anytime you like. When writing a journal, you suddenly remembered you need the section that you deleted earlier. What will you do?

Haven't it occured to you that if only you could use your favorite editor VSCode to write your documents? With all the settings you configured, themes you liked and the extensions you probably prefer over your toxic girlfriend?

Think of a moment, your thesis supervisor and co-supervisor wanted to make some changes to your document. What you will do? Email them your document and tell him to reply the updated version? This is no 80's.

Or, you are in your car, away from your Laptop / Desktop. Suddenly remember you forgot to change the title of your document from "Loren Ipsum" to your actual document title. Won't it be great to modify your document On the Go with your phone? Or in a nerdy way, Apple Watch?

**Yes! You can do all of these things now with Git, GitHub, Full VSCode Integration, Live Collaboration and Web Support - The WebLatex.**

### Just use overleaf

Yes, but

- In overleaf, you have to pay 40$ to get the git feature which isn't even have the best or full git experience.
- Pay 40$ to collaborate with more than 1 person
- No VSCode

## Installation Instructions

> You can either fork this repository or just Use as a template. But you will not get latest updates if you use this as a template.

1. Login or Sign Up to [GitHub](https://github.com/login)
2. Fork this repository or just click [Here](https://github.com/sanjib-sen/weblatex/fork). Or, If you want to use as a template just Click on `Use this template` and `Create a new Repository`
3. Give it a name and select **Create Fork**
4. Select **<> Code** > **CodeSpaces** > **Create Codespace on Main**
    ![tutorial](images/tutorial.gif)
5. It will start installing. **You Have to wait for 2 mins in the first time**. After that it will take 2/3 seconds to open up

## Where is my PDF?

Generated PDFs will be saved to **`/PDF`** directory

## Editor Instructions

1. Pressing `Ctrl+S` will save the document and generate PDF in the **PDF** folder
2. To check the generated PDF click on the PDF file. However **It will take 20/30 seconds to open the preview for the first time. So, do not panic**. After that, it will generate and preview the pdf instantly.
3. Your code will be automatically saved and the PDF will generate automatically each time you edit something
4. You can see all the error logs in the **Terminal > Output > Latex Compiler** as well as in the Latex Workshop sidebar
5. If it shows **Error showing PDF** or in case of any inconvenience, just reload the browser or press `Ctrl+R`
6. **Just use it as you use Visual Studio Code**
7. Do not delete the `devcontainer.json` file.

## To use with LuaLatex or any other Tex program

Add this line to your main .tex file

```tex
%!TEX program = <tex_program>
```

For example, to use **`LuaLatex`**:

```tex
%!TEX program = lualatex
```

## Live Collaboration

Just Click on the **Live Share** Sidebar button and you are good to go
  ![Collaboration](images/collaborate.png)

## Configuration

- To change the output directory change the following properties in `./.devcontainer/devcontainer.json`

    ```json
    "latex-workshop.latex.outDir": "<YourDirectoryName>",
    ...
    "latex-workshop.latex.magic.args": ["-output-directory=<YourDirectoryName>",..],
    ```

- If you do not need the Live Collaboration at all, you can just **remove** the `"ms-vsliveshare.vsliveshare"` extension from the extension list in `./.devcontainer/devcontainer.json`

    ```json
    "extensions": [..,"ms-vsliveshare.vsliveshare"]
    ```

- Other configuration (e.g. PDF Generation Delay, Auto Saving etc.) can be modified in `./.devcontainer/devcontainer.json`. Check 

## More Features and Configurations

There are a lot of features like

- [Intellisense (Citation, References)](https://github.com/James-Yu/LaTeX-Workshop/wiki/Intellisense)
- [Snippet and SHortcuts](https://github.com/James-Yu/LaTeX-Workshop/wiki/Snippets)
- [Linting](https://github.com/James-Yu/LaTeX-Workshop/wiki/Linters)
- [Formating](https://github.com/James-Yu/LaTeX-Workshop/wiki/Format)
- [Code Folding](https://github.com/James-Yu/LaTeX-Workshop/wiki/ExtraFeatures#code-folding)

And a lot [more](https://github.com/James-Yu/LaTeX-Workshop/wiki/ExtraFeatures).

All of the features and configurations can be found [here](https://github.com/James-Yu/LaTeX-Workshop/wiki).

## Contribution

I am open to and actually request you to contribute in this project. You can just Create a new issue to let me know about your concern / requests or just send a pull request with your desired changes.

## What's Next

1. Will optimize the backend to decrease installation time and PDF showing time for the first time
2. Documentation
3. Release: Export PDF as a release version
4. You tell me

## Contact

1. Send an email to `sksenonline@gmail.com`
2. [Facebook](https://www.facebook.com/sanjib.kumarsen.963/), [LinkedIn](https://www.linkedin.com/in/sanjibsen/)
