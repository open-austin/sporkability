# forkability

Best practices for making projects easy to fork. The most important things you can do are: simplify your projects as much as possible, and

Have anything to add? Fork this repo and open a pull request.

There's more to making a project forkable/adoptable/redeployable than just the code and technology. What data would someone need to have to implement this project. What other skills besides installing the software on a server are needed. For example implementing a 211 system would require good skills organizing and leadership.

# Documentation

## README.md

See the [README-template.md]().

- [ ] Brief description of what the project does and why it exists. Explain why would someone else care.
- [ ] Include screenshots of the project so people can see the project in action without figuring out how to use it.
- [ ] Include a link to the project.
- [ ] Specify a maintainer.
- [ ] Installation instructions.
- [ ] Mistakes.

## INSTALL.md

By default, include installation instructions in the README. Consider moving the instructions to a INSTALL.md if the instructions are very long and distract from the rest of the README.

- [ ] Use your languages package management tools. Avoid asking people to install them by hand. Be sure to use very specific version numbers (`6.6.6` is much better than just `6`).
    - Python: requirements.txt
    - JavaScript: package.json
    - Ruby: Gemfile
    - Go: :troll: (Check in your dependencies, I guess)
- [ ] List dependencies that have to be manually installed. Link to useful guides on setting them up. Examples include Postgres, ...
- [ ] Test your installation and deployment instructions on a clean machine.
- [ ] CHANGELOG.md
    "It is a good idea to keep a changelog. http://keepachangelog.com (is a project on GitHub). "
    - See https://github.com/cfpb/qu and https://github.com/cfpb/hmda-explorer
    - Some Inspiration: http://keepachangelog.com/

## Data

- [ ] Its important to answer this question: What is the minimum amount of data do I need to get this project running?
- [ ] List where all the data the app uses, where it comes from, and from how it is used. Its important to answer this question: What is the minimum amount of data do I need to get this project running?

# Licenses and Copyright

- [ ] Choose a license and add it to your repo
    - ChooseALicense.com
    - Ideally just dedicate your work to the the Public Domain. The Unlicense is a good one for this.
    - Why public domain? MIT, GPL, and the rest don't answer the question of copyright.
- Don't put copyright 2015 John, Jane, Bob, etc. on every page (or even anywhere in the app).
    - As somebody forking the repo, I don't want to put your name on every page. Will you be offended that I'm removing yourname?
- Contributing - you’re inputs will go to the public domain!

# Be easy to contact

- Answer/use GitHub issues
- Add an email to the README, or add emails to your GitHub profile
- Specify a maintainer, and make sure the maintainer has an easy to find email
- If your brigade or project has a Slack channel, add a link to it.

# Simplify your app as much as possible

- Deploy buttons
- Reduce the number of dependencies
    - Do you really need mongo and memcached?
    - Do you even need a server? Can it just be static HTML + JS files hosted on GitHub Pages?
- Use simple easy to deploy technology
    - Tools like Travis CI make deployment public. Anybody can look at the build history and figure out how things are built.

# Admit your mistakes

- Are you unhappy with the architecture or the code of your app? Say so in the README or an issue (and explain why). People trying to fork your app may encounter some of these same problems and have solutions. Or they may just give up.
- Keep your city specific configuration in one file
    - For example, if your app has a map with some initial coordinates, store those initial coordinates in a config file instead of making them difficult to find.

# Style

- Format code consistently and follow a popular styleguide
    - [rdio/jsfmt](https://github.com/rdio/jsfmt)
    - [JS Standard Style](https://github.com/feross/standard)
    - [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)

# Apps that have been easy to fork

- Boston GreenMap
- CutePets Bot - Adoptable pets!

- How to tie hackpads and the repo?
- How do you use Github Issues?

- Deploy work on Github Pages!
  - Deployed projects to Github issues
  - Can’t maintain projects on Github Issues?
  - So many orgs can’t even get Wordpress up!
  - Best documentation: - FusionTables - Derrik Edder in Chicago
