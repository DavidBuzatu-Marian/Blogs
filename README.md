# Table of contents
- [Blogs](#blogs)
  * [Background](#background)

# Blogs
Repository to hold blogs in markdown type. Blogs are written in a specific format in order to keep the automated usage of them practical.

## Background

To use these blogs in my [portfolio](https://github.com/DavidBuzatu-Marian/DavidBuzatu_Portfolio_V2) website, I had to come up with a way in which blogs contained the following information without using a database:
1. Publication date
2. Title
3. Splash image
4. Tags


In order to solve these issues, each blog starts with its publication date. During the fetching process on my portfolio website, I pre-process each blog, taking the publication date out and sorting the blogs in decreasing order of it.

Then, the title is processed in a similar way, knowing it is the element starting with `#`.

Then, the splash image is found by searching for the first `<img>` tags.

Then, the tags are found by keeping them in an array-like format. This is due to the array being processed by a `JSON.parse()` to convert it to a JavaScript array.

Finally, the rest of the content is kept and rendered on screen.
