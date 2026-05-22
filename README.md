# Zero to VS Hero

This is the main event: getting VS Code installed, set up, and running your notebooks, either fresh on your own machine or pulled down from the cloud and sent back when you are done.

## Before you read the steps

A few things to know going in.

**The instructions work exactly like the previous guide.** Each step uses the same format:

- **Type:** what to type or paste
- **Press:** what key to press
- **You should see:** what to expect after

And where the steps differ by operating system, they are split into **Windows**, **macOS**, and **Linux** sections. Read only the one that matches your computer and ignore the other two.

**You already have what you need to start.** From the previous setup guide, you already have Python and Anaconda installed, including the `upitt` environment. This guide does not change any of that. It only adds VS Code on top of what you already have, and then points VS Code at the `upitt` environment you already made. So there is nothing to install on the Python or Anaconda side here. You are just adding a new place to do your work.

**Do not be afraid of making a mistake.** VS Code is about the most forgiving tool you will ever use, because underneath it is really just a bundle of small add-on pieces called extensions, and almost anything you do can be undone, closed, or reinstalled. Nothing here can break your computer.

So if at any point you feel like you have messed something up, do this: take your hand off the mouse, take a breath, and start the step over. That is genuinely all it takes most of the time. You are cool. The potted plant to your left is cool. That bird outside that will not stop singing? Not cool. But you? Cool. Keep going.

---

## Step 1: Download and install VS Code

VS Code is free, made by Microsoft, and the same on every operating system once it is open.

### Windows

1. Open a web browser and go to **https://code.visualstudio.com**
2. Click the big blue **Download for Windows** button.
3. When the download finishes, double-click the downloaded file (it will be named something like `VSCodeUserSetup-x64.exe`).
4. Walk through the installer:
   - Accept the agreement, click **Next**.
   - Leave the install location at its default, click **Next**.
   - On the "Select Additional Tasks" screen, the defaults are fine. The box "Add to PATH" is helpful to leave checked. Click **Next**.
   - Click **Install**, then **Finish**.

**You should see:** VS Code opens, showing a Welcome tab.

### macOS

1. Open a web browser and go to **https://code.visualstudio.com**
2. Click the big blue **Download for macOS** button.
3. When the download finishes, find the downloaded `.zip` file (usually in your Downloads folder) and double-click it. This produces a file called **Visual Studio Code**.
4. Drag that **Visual Studio Code** file into your **Applications** folder.
5. Open your Applications folder and double-click **Visual Studio Code** to launch it.
   - The first time, macOS may warn that it was downloaded from the internet. Click **Open** to confirm.

**You should see:** VS Code opens, showing a Welcome tab.

### Linux

1. Open a web browser and go to **https://code.visualstudio.com**
2. Click the **Download for Linux** button and choose the package that matches your system. For Ubuntu, Debian, and most beginner-friendly distributions, choose the **.deb** option.
3. When the download finishes, open your file manager, find the downloaded `.deb` file, and double-click it. Your system's software installer should open and offer an **Install** button. Click it.
   - If double-clicking does not open an installer, your distribution may handle this differently. Search your applications menu for "Software" and install from there, or consult your distribution's documentation.
4. After installing, search your applications menu for "Visual Studio Code" and open it.

**You should see:** VS Code opens, showing a Welcome tab.

---

## Step 2: What an extension is, and the four you need

VS Code on its own is just a text editor. It does not yet know how to run Python or how to open notebooks. You teach it those skills by adding small pieces called **extensions**. An extension is an add-on you install once from inside VS Code, the same way you install an app on a phone. You will install four of them. You do this one time, and you will not have to do it again.

You will install each extension the same way: open the extensions panel, search for the extension by its name, and click its Install button. You are about to do that four times. Going through this by hand, rather than hoping VS Code adds pieces for you, does two things: it makes sure you actually have all four extensions, and it teaches you how to add any extension you might need later in the program. That same search-and-install motion is how you will add tools for other courses, so it is worth learning now.

**First, open the extensions panel:**

1. Look at the narrow vertical strip of icons running down the far left edge of the VS Code window. This strip is called the Activity Bar.
2. On that Activity Bar, find the icon that looks like four small squares, with one of the four squares lifting away from the other three. Click that four-squares icon.
   - **You should see:** a panel open along the left side with a search box at the top. The search box contains gray placeholder text reading "Search Extensions in Marketplace."

**Now install the four extensions, one at a time.**

**Extension 1 of 4: Python**

1. Click inside the search box at the top of the extensions panel.
2. **Type:** `Python`
3. A list of results appears below the search box. Find the result whose name is exactly **Python** and whose publisher, shown in smaller text, is **Microsoft**. This Python extension has a blue verified checkmark and a download count in the millions, which helps you confirm you have the right one and not a lookalike.
4. Click that **Python** result to open the Python extension's page.
5. A larger page for the Python extension opens to the right. On that page, click the blue **Install** button.
   - **You should see:** the Install button change to show the Python extension is now installed (the button may now read "Uninstall" or show a gear icon instead).

**Extension 2 of 4: Jupyter**

1. Clear whatever text is in the search box (select the text and delete it), then click inside the search box again.
2. **Type:** `Jupyter`
3. In the results list, find the result whose name is exactly **Jupyter** and whose publisher is **Microsoft**.
4. Click that **Jupyter** result to open the Jupyter extension's page.
5. On the page that opens for the Jupyter extension, click the blue **Install** button.

**Extension 3 of 4: Jupyter Keymap**

1. Clear the search box, then click inside the search box again.
2. **Type:** `Jupyter Keymap`
3. In the results list, find the result named **Jupyter Keymap**, published by **Microsoft**.
4. Click that **Jupyter Keymap** result to open its page, then click the blue **Install** button on the Jupyter Keymap page.

**Extension 4 of 4: Jupyter Cell Tags**

1. Clear the search box, then click inside the search box again.
2. **Type:** `Jupyter Cell Tags`
3. In the results list, find the result named **Jupyter Cell Tags**, published by **Microsoft**.
4. Click that **Jupyter Cell Tags** result to open its page, then click the blue **Install** button on the Jupyter Cell Tags page.

**You should see:** all four extensions now showing as installed. One note so nothing surprises you: VS Code sometimes installs a few extra Jupyter-related helper pieces on its own, with names like "Jupyter Notebook Renderers" or "Jupyter Slide Show." If you see one or two extra Jupyter-named items in your installed list that you did not add yourself, seeing those extra items is normal and correct. Leave the extra items alone. They do no harm, and you do not need to remove them.

That is all the setup VS Code itself needs. You will not have to install these extensions again.

---

## Step 3: Make your PittMDS folder

You want one consistent home for all your coursework, in the same place everyone else in the cohort keeps theirs. That way, when you need help, you and the person helping you are looking at the same structure, and "put it in your PittMDS folder" means the same thing to everyone.

You will create a folder named exactly **PittMDS** (no spaces, capital P, capital MDS) inside your user folder.

### Windows

1. Open **File Explorer** (the folder icon on your taskbar).
2. In the address bar at the top, **Type:** `C:\Users\` followed by your username, then **Press:** Enter. (If you are unsure of your username, clicking "This PC" then your `C:` drive then "Users" will show you the folders; yours is the one that is not "Public" or "Default.")
3. Right-click in an empty area, choose **New**, then **Folder**.
4. Name it `PittMDS` and **Press:** Enter.

Your folder now lives at `C:\Users\<your-username>\PittMDS`.

### macOS

1. Open **Finder**.
2. In the menu bar at the top, click **Go**, then **Home**. This opens your user folder.
3. Click **File** in the menu bar, then **New Folder** (or right-click in an empty area and choose **New Folder**).
4. Name it `PittMDS` and **Press:** Return.

Your folder now lives at `/Users/<your-username>/PittMDS`.

### Linux

1. Open your **Files** application (the file manager).
2. Navigate to your **Home** folder (it is usually the first item in the sidebar).
3. Right-click in an empty area and choose **New Folder** (or use the menu).
4. Name it `PittMDS` and **Press:** Enter.

Your folder now lives at `/home/<your-username>/PittMDS`.

### Open the folder in VS Code

Now tell VS Code to use that folder as its home base.

1. In VS Code, click **File** in the top menu, then **Open Folder**.
2. Navigate to the **PittMDS** folder you just made and select it. Click **Open** (or **Select Folder**).
   - VS Code may ask "Do you trust the authors of the files in this folder?" Click **Yes, I trust the authors**. This is your own folder, so it is safe.

**You should see:** the PittMDS folder name appears in the panel on the left side of VS Code. Anything you put in this folder will now show up there, ready to open with a single click.

---

## Step 4: Get a notebook open

Here the path splits depending on what you are doing. Read the one that fits your situation.

- **Path A:** You are starting a brand new notebook from scratch on your own machine.
- **Path B:** You have a homework notebook on Coursera that you want to pull down, work on locally, and send back.

Most of the time, for actual homework, you want **Path B**.

### Path A: Start a new notebook from scratch

1. In the left panel showing your PittMDS folder, hover over the folder name. A small row of icons appears.
2. Click the **New File** icon (a page with a small plus).
3. Name the file ending in `.ipynb`, for example `practice.ipynb`, and **Press:** Enter.

**You should see:** the file opens as a notebook, with a place to type your first cell. Skip ahead to **Step 5: Pick your kernel**.

### Path B: Pull a notebook down from Coursera, work on it, send it back

This is the round trip: down, work, back up. Take it in order.

**Download the notebook from Coursera:**

1. Open your assignment's lab on Coursera in your browser, the same way you normally would.
2. In the lab's file list, find your notebook (for example `HW2.ipynb`). Either use a **Download** button if the lab offers one, or check the box next to the file and use the download option that appears.
3. When it downloads, move the downloaded notebook file into your **PittMDS** folder so VS Code can see it. (Putting it in a sub-folder for that assignment, like `PittMDS/Homework2`, keeps things tidy, but that is optional.)

**One rule, and it is absolute: never rename the file.** Whatever it downloaded as, `HW2.ipynb`, that is its name forever. Do not change it, not even slightly. Coursera's automatic grader is looking for that exact name. If you rename it, your finished work becomes invisible to the grader even though it is sitting right there, and you can get a zero on work you actually did. So leave the name alone.

**Open it in VS Code:**

1. In the left panel, click the notebook file you just moved into PittMDS.

**You should see:** the notebook opens, showing the assignment's cells. Now go to **Step 5: Pick your kernel** to make it runnable.

You will send the finished version back up to Coursera in **Step 6**.

---

## Step 5: Pick your kernel

A "kernel" is just the Python engine that actually runs your code. You need to tell the notebook to use the `upitt` environment you made with Anaconda.

1. Look at the **top-right corner** of the open notebook. There is a button there for selecting the kernel. It may say "Select Kernel" or show some other Python name.
2. Click it.
   - **You should see:** a menu drops down from the top of the window with kernel options. VS Code may offer choices like "Python Environments" first; if so, click that.
3. Look through the list for the one that mentions **upitt**. It will look something like `upitt (Python 3.10.20)`.
4. Click it.

**You should see:** the top-right corner now shows `upitt` as the selected kernel. Your notebook is now wired to the right Python.

If you do not see `upitt` in the list, close VS Code completely and reopen it, then try again. VS Code sometimes needs a restart to notice Anaconda environments the first time.

---

## Step 6: Run it, and (for Path B) send it back

### Run a cell to confirm everything works

1. Click into the first code cell so your cursor is inside it.
2. **Press:** Shift and Enter together.

**You should see:** a number in brackets appear to the left of the cell, like `[1]`, and any output appear just below it. That number is proof the kernel ran your code. Congratulations, you are running notebooks locally.

A few ways to run cells, now that you are here:

- **Shift+Enter:** run this cell and move to the next one.
- **Ctrl+Enter** (Cmd+Enter on Mac): run this cell and stay on it.

### When you are finished, run the whole thing top to bottom

Before you send anything back to Coursera, you must run the entire notebook fresh, in order, from the top. Here is why this matters: as you work, it is easy to run cells out of order, or to delete a cell you were relying on, and the notebook can look finished while secretly being held together by leftover scraps in memory. A clean run from the top is the only thing that proves it actually works. It is also exactly what Coursera's grader does to it.

1. At the top of the notebook, find the **Restart** button (a circular arrow) and click it to restart the kernel. Confirm if it asks.
2. Then use **Run All** (a "Run All" button sits along the top of the notebook).

**You should see:** every cell run in order, each getting its own bracket number, no red error messages. If a cell errors, fix it and run all again. Do not send back a notebook that errors on a clean run.

### Send it back to Coursera (Path B only)

1. Go back to your assignment's lab on Coursera in your browser.
2. Use the lab's **Upload** button.
3. Choose your finished notebook from your PittMDS folder.

**Expect a warning, and expect it to feel wrong.** Because your file has the same name as the blank one already in the lab, the lab will ask something like **"are you sure you want to overwrite this file?"** Every instinct you have about computers says overwriting a file is dangerous and you should stop. In this one case, ignore that instinct. The file you are replacing is the blank original; the file you are uploading is your finished work. You *want* yours to take its place. Confirm the overwrite.

**DON'T PANIC if you open the notebook and your work is not there.** This is normal and your file is safe. Here is what is happening: the lab loaded the old, blank notebook into your session when you first opened it, and it keeps showing you that loaded copy. It does not automatically notice that the file underneath has been replaced by your upload. The fix is simple:

> **Close the notebook tab or window completely, then open the notebook again.** This forces the lab to load the fresh version, the one you just uploaded. Your work will be there.

Once you can see your work in the lab and have confirmed it runs, you are ready to turn it in.

**How you turn it in varies by assignment.** Some assignments have a Submit button. Some advance with a Next button. Some have a checkbox confirming you are done. Some grade automatically with no button at all. There is no single answer, so: **submit your assignment as directed** by that specific assignment's instructions. Whatever the method, only do it after you have run the notebook and confirmed it works.

That is the full round trip: down from the cloud, worked on locally with all of VS Code's help, and back up to be graded. From here on, every assignment follows the same path.

---

# Your First Jupyter Notebook

You now have VS Code installed, the four extensions added, and you know how to open a notebook and point it at the `upitt` kernel. This section is where you actually use it. You are going to write and run three small pieces of code, building from the simplest possible thing up to a tiny program. The goal is not to learn programming in one sitting. The goal is to prove to yourself, with your own eyes, that the whole setup works, and to get comfortable with the one habit that trips up almost everyone at the start: running cells.

If you have not already, open a notebook to work in. Use **Path A** from Step 4 to make a fresh practice notebook (name the practice notebook something like `firstnotebook.ipynb`), and make sure the top-right corner of the notebook shows `upitt` as the kernel, exactly as you set up in Step 5. Everything below happens inside that practice notebook.

## What a cell is, and how to make one

A notebook is built out of **cells**. A cell is a single box that holds a chunk of code. You type code into a cell, you run that cell, and the notebook shows you the result of that cell directly underneath it. A notebook is just a stack of these cells, top to bottom.

When you open a fresh notebook, you should see at least one empty cell already waiting for you: a rectangular box, usually with a slightly different background than the rest of the page, often with the word "Python" or a small "+ Code" label near it. That box is where your code goes.

To make sure you are starting clean, here is how to add a new code cell whenever you need one:

1. Move your mouse near the top-left of the notebook, or hover just above or below an existing cell.
2. A small button labeled **+ Code** appears. Click the **+ Code** button.

**You should see:** a new empty code cell appear, ready for you to type into. Each time these instructions say "make a new cell," you click that **+ Code** button.

## Piece 1: Arithmetic (proving the kernel runs)

Start with the simplest thing a computer can do: basic math. This first piece proves that your kernel is alive and actually running your code.

1. Click inside your first empty code cell so that your typing cursor is blinking inside that cell.
2. Into that cell, **Type:** the following exactly as written:

```python
2 + 2
```

3. Now run that cell. To run the cell, **Press:** the **Shift** key and the **Enter** key at the same time.

**You should see** two things happen. First, a number in square brackets appears just to the left of the cell, reading `[1]`. That bracket number is the notebook telling you "I ran this cell, and this was the first cell I ran." Second, directly underneath the cell, a result appears reading `4`.

Notice something important: you did not have to tell the notebook to show you the answer. You just typed `2 + 2`, and the notebook displayed `4` on its own. A Jupyter notebook automatically displays the result of the last line in a cell. This is a convenience the notebook gives you, and it is worth knowing now so the behavior does not confuse you later.

Let us do one more arithmetic cell so you can see the bracket number change.

1. Make a new cell by clicking the **+ Code** button.
2. Into that new cell, **Type:**

```python
10 * 5
```

3. Run that cell by pressing **Shift** and **Enter** together.

**You should see** the bracket to the left of this cell now read `[2]`, because this is the second cell you have run, and the result `50` appear underneath the cell. The asterisk (`*`) is how you tell Python to multiply.

That is arithmetic. The kernel runs, and you can read the answers. If you got `4` and `50` with bracket numbers next to them, everything is working.

## Piece 2: Variables (proving the notebook remembers)

Math is fine, but the real power comes from storing values and reusing them. A **variable** is a name you give to a value so you can use that value again later. This piece proves that the notebook remembers things from one cell to the next.

1. Make a new cell by clicking the **+ Code** button.
2. Into that new cell, **Type** the following two lines exactly. To get the second line, press **Enter** at the end of the first line to move down inside the same cell, then type the second line:

```python
first_name = "John"
last_name = "Doe"
```

3. Run this cell by pressing **Shift** and **Enter** together.

**You should see** a new bracket number appear to the left of this cell, but no result printed underneath the cell. That absence of output is correct and expected. You did not ask the notebook to show you anything; you only asked the notebook to store two values. The value `"John"` is now stored under the name `first_name`, and the value `"Doe"` is now stored under the name `last_name`. The quotation marks around `John` and `Doe` are how you tell Python that those values are words (text), not numbers.

Now prove that the notebook actually remembered those two values, by using the two values in a different, later cell.

1. Make a new cell by clicking the **+ Code** button.
2. Into that new cell, **Type:**

```python
print(first_name + " " + last_name)
```

3. Run this cell by pressing **Shift** and **Enter** together.

**You should see** the result `John Doe` appear underneath the cell.

Look at what just happened, because it is the whole point of this piece. You stored the two values in one cell, and then used those two stored values in a completely different cell, and the notebook still knew what `first_name` and `last_name` meant. The notebook remembers what you have run, across all the cells, for as long as the kernel keeps running. That shared memory is what lets you build something step by step, one cell at a time.

A few small things from that last cell, so nothing is a mystery:

The word `print` is an instruction that tells Python to display whatever you put inside the print parentheses. Earlier, with `2 + 2`, the notebook displayed the answer on its own. But that automatic display only happens for the very last line of a cell, and only for a value. When you want to be sure something is shown, `print` is how you ask for the value to be shown on purpose.

The plus signs (`+`) between the names join the pieces of text together into one. The `" "` in the middle is a single space inside quotation marks, which puts the space between `John` and `Doe` so that the result reads `John Doe` and not `JohnDoe`.

## Piece 3: A loop (proving it can actually program)

The last piece is a **loop**. A loop is how you tell the computer to repeat an action several times without you writing the action out over and over. This is the moment the notebook stops being a fancy calculator and starts being a tool that does work for you.

You are going to make the notebook count from 1 to 5, printing each number on its own line, all from a few short lines of code.

1. Make a new cell by clicking the **+ Code** button.
2. Into that new cell, **Type** the following two lines exactly. After typing the first line, press **Enter** to move to the next line inside the same cell. The spaces at the start of the second line matter, so type them: press the **Tab** key once at the start of the second line to create that indent.

```python
for number in range(1, 6):
    print(number)
```

3. Run this cell by pressing **Shift** and **Enter** together.

**You should see** five lines of output appear underneath the cell, each on its own line:

```
1
2
3
4
5
```

Here is what each part of that loop does, so the loop is not a magic spell:

The word `for` begins the loop. It tells Python "do the following action repeatedly."

`range(1, 6)` produces the sequence of numbers to count through. One quirk to know up front, because it surprises every beginner: the count starts at the first number, `1`, but stops just before the second number, `6`. So `range(1, 6)` gives you 1, 2, 3, 4, 5, and not 6. This is simply how Python's `range` works, and now you know.

`number` is a variable that holds one value from that sequence at a time. The first time through the loop, `number` holds `1`. The next time, `number` holds `2`, and so on, up through `5`.

The second line, `print(number)`, is the action that gets repeated. The indent at the start of that line (the spaces you made with the Tab key) is how Python knows that this line belongs to the loop. Everything indented under the `for` line is the work the loop repeats. The colon (`:`) at the end of the `for` line is required punctuation that tells Python "the repeated work starts on the next line."

So in plain words: for each number in the sequence 1 through 5, print that number. Five numbers in, five lines of output out. You just wrote a program.

## The one habit that prevents most beginner headaches

You have now run several cells in a tidy order, top to bottom. In real work, you will not always be that tidy. You will run a cell, change it, run a cell lower down, go back up and fix something, and run cells out of order. This is where the single most confusing beginner problem comes from, so it is worth seeing on purpose, once, while nothing is at stake.

Remember from Piece 2 that the notebook remembers values across cells. That memory does not care about the top-to-bottom order the cells are arranged in. It only remembers the order in which you actually *ran* the cells. That means a notebook can look correct on the page while secretly holding an old value in its memory from a cell you changed but did not re-run.

You do not need to manufacture an example of this going wrong. You just need to know the fix, because the fix is reliable and you will use it constantly. Before you trust any notebook, especially before you submit one for a grade, you do this:

1. At the top of the notebook, find the **Restart** button. The Restart button is a circular-arrow icon, usually labeled "Restart." Click the Restart button. If the notebook asks you to confirm, confirm.
2. Then find and click **Run All**. The Run All button sits along the top of the notebook.

What this does: restarting wipes the notebook's memory completely clean, throwing away every stored value. Then Run All runs every cell again, in order, from the very top. After a Restart and Run All, what you see on the screen is the honest truth of what your code actually produces, with no leftover memory hiding a problem. The bracket numbers will renumber themselves from `[1]` straight down the notebook, which is your visual proof that every cell ran fresh and in order.

Get in the habit of doing a Restart and Run All before you believe your own notebook. It is the same thing the automatic grader does to your work, so if your notebook survives a clean Restart and Run All on your machine, you can trust it will behave the same way when it is graded.

That is your first notebook. You ran arithmetic, you stored and reused values in variables, you wrote a loop that did real repeated work, and you learned the one habit that keeps notebooks honest. Everything else in the program is built from these same pieces.
