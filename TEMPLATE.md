### Hi, I'm a developer from <img src="https://hatscripts.github.io/circle-flags/flags/no.svg" width="16" /> Norway

<!--<p>
  <img alt="Vue" src="https://img.shields.io/badge/-Vue-63B587?style=flat-square&logo=vue.js&logoColor=white" />
  <img alt="HTML" src="https://img.shields.io/badge/-HTML-E34F26?style=flat-square&logo=html5&logoColor=white" />
  <img alt="Pug" src="https://img.shields.io/badge/-Pug-9F6758?style=flat-square&logo=html5&logoColor=white" />
  <img alt="CSS" src="https://img.shields.io/badge/-CSS3-448AC0?style=flat-square&logo=css3&logoColor=white" />
  <img alt="Sass" src="https://img.shields.io/badge/-Sass-CC6699?style=flat-square&logo=sass&logoColor=white" />
  <img alt="javaScript" src="https://img.shields.io/badge/-JavaScript-DABD4D?style=flat-square&logo=html5&logoColor=white" />
  <img alt="Netlify" src="https://img.shields.io/badge/-Netlify-5EA7BA?style=flat-square&logo=netlify&logoColor=white" />
  <img alt="Node.js" src="https://img.shields.io/badge/-Nodejs-43853d?style=flat-square&logo=Node.js&logoColor=white" />
  <img alt="Python" src="https://img.shields.io/badge/-Python-4F7CAA?style=flat-square&logo=python&logoColor=white" />
  <img alt="Rust" src="https://img.shields.io/badge/-Rust-000000?style=flat-square&logo=rust&logoColor=white" />
  <img alt="Docker" src="https://img.shields.io/badge/-Docker-46a2f1?style=flat-square&logo=docker&logoColor=white" />
  <img alt="MongoDB" src="https://img.shields.io/badge/-MongoDB-13aa52?style=flat-square&logo=mongodb&logoColor=white" />
  <img alt="Flutter" src="https://img.shields.io/badge/-Flutter-3E89F5?style=flat-square&logo=flutter&logoColor=white" />
  <img alt="git" src="https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white" />
  <img alt="VSCode" src="https://img.shields.io/badge/-VSCode-3277B4?style=flat-square&logo=visual-studio-code&logoColor=white" />
  <img alt="Brave browser" src="https://img.shields.io/badge/-Brave_Browser-FB542B?style=flat-square&logo=brave&logoColor=white" />
  <img alt="User since 2015-03-04" src="https://img.shields.io/badge/Joined-2015--03--04-2eb872?style=flat-square&logo=github&logoColor=white&labelColor=2f3438" />
  <img src="https://gpvc.arturio.dev/probablykasper" />
</p>-->

```js
// {{ TEMPLATE: }}
module.exports = {
  CUSTOM_PINNED_REPOS: {
    type: 'specificRepos',
    repos: [
      'cpc',
      'ferrum',
      'date-picker-svelte',
      'kadium',
      'mr-tagger',
      'time-machine-inspector',
      'remind-me-again',
      'vidl',
      'taskler',
      'embler',
      'notifier',
      'thumbnail-grabber',
      'redlux',
      'readme-template-action',
      '2dcam',
      'to',
      'serve',
    ],
    modifyVariables: function(repo, moment, user) {
      // if (repo.REPO_LANGUAGE === 'JavaScript') repo.REPO_LANGUAGE = 'JS'
      let imgSrc = null
      if (repo.REPO_LANGUAGE === 'Rust') imgSrc = './rust.svg'
      // if (repo.REPO_LANGUAGE === 'Svelte') imgSrc = 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/svelte/svelte-original.svg'
      if (repo.REPO_LANGUAGE === 'Svelte') imgSrc = 'https://raw.githubusercontent.com/devicons/devicon/e9bd76ead0b7ea6dde1b108d902868bd90195aa9/icons/svelte/svelte-original.svg'
      if (repo.REPO_LANGUAGE === 'Python') imgSrc = 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg'
      if (repo.REPO_LANGUAGE === 'Stylus') imgSrc = 'https://stylus-lang.com/logo.svg'
      if (repo.REPO_LANGUAGE === 'JavaScript') imgSrc = 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg'
      if (repo.REPO_LANGUAGE === 'Dart') imgSrc = 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/dart/dart-original.svg'
      if (repo.REPO_LANGUAGE === 'TypeScript') imgSrc = 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg'
      if (repo.REPO_LANGUAGE === 'Shell') imgSrc = 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bash/bash-original.svg'
      if (repo.REPO_LANGUAGE === 'Go') imgSrc = 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/go/go-original-wordmark.svg'
      
      if (imgSrc !== null) repo.REPO_LANGUAGE = `<img src="${imgSrc}" width="14" height="14" />`
      return repo
    },
  },
}
// {{ :TEMPLATE }}
```

| ⭐️ | 📦 Repo       | 📚 Description |
| -- | ------------ | -------------- |
{{ loop CUSTOM_PINNED_REPOS }}
| {{ REPO_STARS }} | <a href="{{ REPO_URL }}"><b>{{ REPO_NAME }}</b> {{ REPO_LANGUAGE }}</a> | {{ REPO_DESCRIPTION }} |
{{ end CUSTOM_PINNED_REPOS }}
