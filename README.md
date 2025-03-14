# Digital Skills Slides
This repository holds the slide decks for lessons in the digital skills curriculum of the Netherlands eScience Center. It is built using the [NEBULA framework](https://github.com/esciencecenter-digital-skills/NEBULA).

For elaborate setup instructions and other documentation, see the [NEBULA documentation](https://github.com/esciencecenter-digital-skills/NEBULA-docs)


## Quick local setup

More detailed information about local setup can be found in the [NEBULA local rendering docs](https://github.com/esciencecenter-digital-skills/NEBULA-docs/blob/main/local-rendering.md)

### Content directory/repository

To use NEBULA to build the content in this repository locally, you will need to clone this repository and the NEBULA repository:

```bash
git clone git@github.com:esciencecenter-digital-skills/digital-skills-slides.git
git clone git@github.com:esciencecenter-digital-skills/NEBULA.git
```

### Link to the content repository

To make sure that NEBULA knows where to find the content, we create the following environment variable:

```bash
export CONTENT_PATH="path/to/your/content/repository"
```

NOTE: You cannot use a ~ in your path, you have to provide the absolute path as returned with `pwd`.

### Install dependencies
First move into the NEBULA folder (so not the content folder):
```bash
cd NEBULA
```

Install the dependencies using the [node package manager](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm):

```bash
# node package manager
npm install
```

### Local development build

Start the development server on `http://localhost:3000`:

```bash
# node package manager
npm run dev
```

Now you can open a browser and navigate to `http://localhost:3000/digital-skills-slides`
