# dokku-resume
Publish your resume displayed in a stylish, responsive, and easily customizable Bootstrap layout using Dokku

![example](./example.png)

<!-- TABLE OF CONTENTS -->
## Table Of Contents
- [About The Project](#about-the-project)
- [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
- [Usage](#usage)
   - [Updating your resume](#updating-your-resume)
- [Roadmap](#roadmap)
- [Conrtibuting](#contributing)

#

<!-- ABOUT THE PROJECT -->
## About The Project
This project is intended to provide a way to quickly and easily publish your resume using Dokku. It combines [dokku-static-site](https://github.com/glogiotatidis/dokku-static-site) with [startbootstrap-resume](https://github.com/StartBootstrap/startbootstrap-resume). 


### Built With

* [Dokku](https://dokku.com/)
* [Digital Ocean](https://marketplace.digitalocean.com/apps/dokku/)
* [dokku-static-site](https://github.com/glogiotatidis/dokku-static-site)
* [startbootstrap-resume](https://github.com/StartBootstrap/startbootstrap-resume)


<!-- GETTING STARTED -->
## Getting Started

Follow the steps below to set up the project locally.

### Prerequisites

* A hosting platform 
* A running Dokku installation

### Installation

1. Fork this repo

2. Clone the repo specifying your project name and navigate to the directory
   ```sh
   git clone https://github.com/{your-github-username}/dokku-resume.git
   cd dokku-resume
   ```

   Alternatively, you can specify your own project name by appending it to the `git clone` command. Then just substitute it in the following commands:
   ```sh
   git clone https://github.com/{your-github-username}/dokku-resume.git my-project-name
   cd my-project-name
   ```

   
3. Update the [resume template](docs/index.html) with your resume details and commit the change:
   ```sh
    git add .
    git commit -m "<Commit message>"
   ```

### Configuration

1. Create the app
```
# on the Dokku host
dokku apps:create dokku-resume
```

2. Add the dokku host as a git remote

```
git remote add dokku dokku@{my-host.com}:dokku-resume
```

3. Push to dokku

```
git push dokku master
```

<!-- USAGE EXAMPLES -->
## Usage
### Updating your resume
As you update your resume, push to your main branch and then deploy to your Dokku host via the steps above.


<!-- ROADMAP -->
## Roadmap
* Include multiple templates
* Extract content into Markdown files
* ...

<!-- CONTRIBUTING -->
## Contributing
TBD

1. Clone the repo
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
