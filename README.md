# INK-Ascii-Diagrams

Community repository for sharing ASCII diagrams. Edit and view them as vector graphics with the INK notebook tool: https://a.co/d/0dEQ2VVP

## About

Each diagram in this repository is a plain-text `.txt` file. Paste it into the INK notebook tool and it is rendered as an SVG vector graphic that you can download and edit.

The tool is **fully client-side. There is no server.** 

**Pull requests are very welcome.** If you can draw it in ASCII, please add it: physics, math, electronics, chemistry, flowcharts, anything that reads well as text.

## How to use a diagram

1. Open a `.txt` file from this repository, for example `physics/free-body-diagram.txt`.
2. Copy its full contents.
3. Paste it into the ASCII source box of the INK notebook tool.
4. Copy or download the SVG, and edit it further in an SVG editor if you like.

## Example

A diagram is just text:

```
              N
              ^
              |
        +-----+-----+
        |           |
 f <----+           +----> F
        |     m     |
        |           |
        +-----+-----+
              |
              |
              v
              mg
```

![Free-body diagram](images/free-body-diagram.svg)

## How to submit a pull request

1. **Fork** this repository with the *Fork* button at the top right of the GitHub page.
2. **Clone** your fork and move into it:

   ```bash
   git clone https://github.com/sevetech/INK-Ascii-Diagrams.git
   cd INK-Ascii-Diagrams
   ```

3. **Create a branch** for your change:

   ```bash
   git checkout -b add-my-diagram
   ```

4. **Add your diagram** as a `.txt` file inside a topic folder, using a short lowercase name with hyphens, for example `physics/simple-pendulum.txt`. Create a new folder if the topic does not exist yet (`math/`, `electronics/`, ...).
5. **Check what you are about to commit**, so that only your diagram is included:

   ```bash
   git status
   ```

6. **Commit and push:**

   ```bash
   git add physics/simple-pendulum.txt
   git commit -m "Add simple pendulum diagram"
   git push origin add-my-diagram
   ```

7. **Open the pull request.** On your fork's GitHub page, click *Compare & pull request*, write a one-line description of the diagram, and submit it.

Small fixes are welcome too: better alignment, clearer labels, or corrected physics.

## Guidelines

- The file should contain only the diagram, with no title line and no license header.
- Use plain ASCII characters and spaces (no tabs), so the alignment stays intact.
- Keep labels short.
- Check the diagram in the tool before opening the pull request.

## License

This work is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to share and adapt the diagrams for any purpose, including commercially, as long as you give appropriate credit to **SeveTech** and the contributors, link to the license, and indicate if changes were made.

By opening a pull request you agree that your contribution is released under the same license.

