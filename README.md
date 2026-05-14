# fukui-kanko

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A community project for creating simple, interactive tourism web apps for Fukui, Japan.

This repository provides the tools and a platform for anyone to easily build and share small, visual-novel-style web applications. Tell a story, create a quiz, or guide users through your favorite spots in Fukui!

## Community Showcase

Discover a gallery of apps created by the community. Feel free to try them out, leave feedback, or get inspired!

➡️ **[View Community Apps in Issues](https://github.com/code4fukui/fukui-kanko/issues)**

## Getting Started: Create Your Own App

Follow these steps to build and publish your own Fukui tourism app.

### Step 1: Write Your App's Story

Create a new file named `index.html` and paste the code below. This example is a simple interactive quiz. You can test and modify your code live using the [ES-Jam](https://code4fukui.github.io/htmlprac/) web tool.

For an introduction to the language, see [Introduction to JavaScript](https://github.com/code4fukui/slide/blob/main/%E3%81%AF%E3%81%98%E3%82%81%E3%81%A6%E3%81%AEJavaScript.pdf).

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>My Fukui App</title>
</head>
<body>

<script type="module">
import { bg, show } from "https://js.sabae.cc/egadv.js";

// Set a background image (ID from https://find47.jp/)
await bg(3972); // Tojinbo Cliffs

// Show a message
await show("Hello from Fukui!");

// Ask a question with choices
let answer = await show("Where am I?", ["Fukui", "Ishikawa", "Toyama"]);

// Check the answer and show a result
if (answer == "Fukui") {
  await show("Correct!");
} else {
  await show("Nope, this is in Fukui!");
}

await show("Let's continue exploring!");

// Redirect to the main project page
location.href = "https://github.com/code4fukui/fukui-kanko/";
</script>

</body>
</html>
```

### Step 2: Publish with GitHub Pages

1.  Create a new repository on your GitHub account. (If you're new to GitHub, follow this [First Step on GitHub](https://github.com/code4fukui/slide/blob/main/GitHub%E3%81%AF%E3%81%98%E3%82%81%E3%81%AE%E3%81%84%E3%81%A3%E3%81%BD.pdf) guide).
2.  Add the `index.html` file you created to the new repository.
3.  In your repository's **Settings**, navigate to the **Pages** tab.
4.  Under "Build and deployment," select the source branch (e.g., `main`) and click **Save**.
5.  GitHub will publish your site and provide you with a URL (e.g., `~~https://your-username.github.io/your-repo-name/`~~ *(unavailable)*). It may take a minute to become active.

### Step 3: Share Your Creation

Once your app is live, share it with the community!

- **[Create a new Issue](https://github.com/code4fukui/fukui-kanko/issues/new)** in this repository.
- Include the title of your app and the URL provided by GitHub Pages.

## Examples & Tools

Explore these helpful applications for finding images and location data for your own project.

-   **[Keyword Photo Search](https://code4fukui.github.io/find47/search.html)** - Find photos of locations across Japan by keyword.
-   **[Map Photo Explorer](https://code4fukui.github.io/find47/map.html)** - Discover photos by browsing a map.

## License

MIT License