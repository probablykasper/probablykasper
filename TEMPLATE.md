### Hi, I'm a developer from <img src="https://image.flaticon.com/icons/svg/197/197579.svg" width="16" /> Norway

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
      'v6.kasper.space',
      'vidl',
      'embler',
      'notifier',
      'taskler',
      'mr-tagger',
      'redlux',
      'thumbnail-grabber',
      'yt-email-notifier',
      'readme-template-action',
      '2dcam',
      'to',
      'serve',
    ],
    modifyVariables: function(repo, moment, user) {
      // if (repo.REPO_LANGUAGE === 'JavaScript') repo.REPO_LANGUAGE = 'JS'
      return repo
    },
  },
}
// {{ :TEMPLATE }}
```

| ⭐️ | 📦 Repo       | 🧰 | 📚 Description |
| -- | ------------ | -- | -------------- |
{{ loop CUSTOM_PINNED_REPOS }}
| {{ REPO_STARS }} | <b>[{{ REPO_NAME }}]({{ REPO_URL }})</b> | {{ REPO_LANGUAGE }} | {{ REPO_DESCRIPTION }} |
{{ end CUSTOM_PINNED_REPOS }}
