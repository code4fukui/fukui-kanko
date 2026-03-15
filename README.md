# Fukui Tourism App

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A community-created tourism app for Fukui.

## Demo
Check out the apps created by the community in the [Issues](https://github.com/code4fukui/fukui-kanko/issues) (feedback and comments are welcome!).

## Features
- Create your own tourism app using the provided program
- Discover useful tourism apps like "Find great photos by keyword" and "Find photos on a map"

## Usage
1. Open the [ES-Jam](https://code4fukui.github.io/htmlprac/) site
2. Use the following program as a reference (see also [Introduction to JavaScript](https://github.com/code4fukui/slide/blob/main/%E3%81%AF%E3%81%98%E3%82%81%E3%81%A6%E3%81%AEJavaScript.pdf)):
```
<script type="module">
import { bg, show } from "https://js.sabae.cc/egadv.js";

await bg();
await show("Hello");
await bg(3972);
let a = await show("Where am I?", ["Fukui", "Ishikawa", "Toyama"]);
if (a == "Fukui") {
  await show("Correct!");
}
await show("Please continue to build the app!");
location = "https://github.com/code4fukui/fukui-kanko/";
</script>
```
3. Create a new repository on your GitHub account (if you don't have one, see [First Step on GitHub](https://github.com/code4fukui/slide/blob/main/GitHub%E3%81%AF%E3%81%98%E3%82%81%E3%81%AE%E3%81%84%E3%81%A3%E3%81%BD.pdf))
4. Add a new file, name it "index.html"
5. Paste the program you created
6. Scroll down and click the green "Commit new file" button
7. Go to "Settings" (if hidden, click the "..." button) -> "Pages" on the left menu
8. Change the "source" from "none" to "main", then click "Save"
9. The displayed URL is the URL of your app (it may take about a minute to become active)
10. Please introduce your app in the [Issues](https://github.com/code4fukui/fukui-kanko/issues) of this repository!

## Useful Apps
- [Find great photos by keyword](https://code4fukui.github.io/find47/search.html)
- [Find photos on a map](https://code4fukui.github.io/find47/map.html)

## Related Event
2022-07-16 Saturday [Fukui Prefecture presents Everybody's Tourism Hackathon | Peatix](https://ideathon-hackathon-fukui.peatix.com/)

## License
MIT License