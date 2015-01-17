# SS-Ghost

A starting point for Ghost theme development.

## Usage: Setting Up

- create local Ghost install
- in the themes directory: `git clone https://github.com/Pixel-and-Kraft/ss-ghost.git`
- `cd ss-ghost`
- `npm install`

## Usage: Developing a Theme

In 2 terminals, 2 commands:  

1. `gulp`
2. `gulp ghost-start`

**Command 1:**  
First, cleans destination (build) theme.
Then, runs front-end-asset development watch tasks.  
- .sass/.scss to .css
- script lenting via jshint
- single browserified js build via watchify

**Command 2:**  
A convenience task for running the necessary Ghost start command from the development theme's directory (`npm start`).

**With both commands running (each in their own terminal),** make something awesome :)

*Note: running 'gulp watch' is the same as simply running 'gulp' except that it skips the initial cleaning task (not recommended, but useful if you're sure of no orphans)*

## ABB (Always Be Building)

A goal of ss-ghost is to introduce no more mental load than necessary. Accordingly, the `gulp watch` command (which is started via the `default` task, ie: the one that runs by calling `gulp` in the console) simultaneously watches and builds two theme versions: 

1. A development version
2. A deployment version

In **the development version,** scripts and styles include source maps for sane debugging.

In **the deployment version,** scripts and styles are minified. No source maps are included. 

## Note

- A work in progress. 
- Use at your own risk! 
- Feel free to request insight/help and such in the issues.
- Insight/feedback/PRs welcomed.

---

**For the Curious:**  
The repo's "ss" is short for "Solid Start."