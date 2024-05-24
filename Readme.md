# Instructions for FG GeoI

## Dealing with R Solutions

After really overengineering this in FS22, we are more pragmatic and elegant in FS23. The solutions are in a *private* github repo, which is included into this repo as a submodule. When cloning this project for the first time, you need to explicitly activate this submodule so that the content is pulled:

```
git submodule update --init --recursive
```

## Publishing

I have always found that version controlling the output files is [not a good idea](https://stackoverflow.com/q/67664158/4139249). One way to avoid this is by adding `docs/` to `.gitignore` and using ~the tool [`ghp-import`](https://pypi.org/project/ghp-import/)~ the `quarto publish` functionality. 

We used to have the html-output in its own repo (`computationalmovementanalysis.github.io`), but switched it up in FS23: The html output is now in the `gh-pages` branch, and computationalmovementanalysis.github.io forwards to computationalmovementanalysis.github.io/FS23.

To publish the html files to the `gh-pages` branch, run the following line:

```
quarto publish --no-prompt gh-pages
```




# Todos in FS25

In Ex. 5, when we try and find a meet pattern between rosa and sabi, the order of the exercises is aligned with how you would solve this task if you had foresight. It would be easyer to undestand the exercise, if we first split the animals into two df's, rosa and sabi. plot them. Did they meet? how do we find out? Try to join: cant. So need to create datetimeround... etc


