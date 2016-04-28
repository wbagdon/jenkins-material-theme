# jenkins-material-theme
Beautify your Jenkins with the Material Design theme!

Forked from: http://jenkins-contrib-themes.github.io/jenkins-material-theme

So you love **Jenkins** but hate its ugly user interface and icons... Me too!  Introducing **Jenkins Material Theme**.
You can turn your favorite frog CI tool into a handsome prince in few steps!

## Features
* Just one small css file (35K)
* Embed minified SVG images
* Update logo with simple replacement
---
## Installation
1. Copy the files from /dist into %JENKINS_HOME%/userContent
1. Install [Jenkins Simple Theme Plugin][simple]
1. Click `Manage Jenkins`
1. Click `Configure System` and scroll down to `Theme`
1. Specify the URL for `https://$JENKINS_URL:8080/userContent/material-light.css`
1. Click `Save`

## Development
CSS file are minified and compressed with Grunt. To prepare the environment:

```
npm install
grunt

```

This will generate the following file:
- dist/material-light.css
- dist/logo.png

To get the latest icons and features:

```
git pull
npm update
grunt
```

## Compatibility
- Simple Theme plugin 0.3
- Jenkins 1.636
- Firefox 3.5+
- Chrome 4+
- Safari 4+
- Opera 15+
- Microsoft IE11 and Edge

If you are experiencing issues please let me know! Also, feel free to contribute!

## License
http://afonsof.mit-license.org/

## Thanks to
- [@alfonsof][alfonsof] for the base theme
- [Simple Theme Plugin][simple] for the Simple Theme plugin
- [Google][google] for the the material design inspiration and the icons
- [Material Design Icons][material-design-icons] for some extra icons
- [Stylish][stylish] for making the test of new versions easy
- [canon-jenkins][canon-jenkins] for the base theme
- [@Heldroe][heldroe] for Firefox and Microsoft support
- [@bootstraponline][bootstraponline] for Jenkins native plugin

[alfonsof]: http://afonsof.com/
[simple]: https://wiki.jenkins-ci.org/display/JENKINS/Simple+Theme+Plugin
[google]: https://www.google.com/design/spec/material-design/introduction.html
[material-design-icons]: https://materialdesignicons.com/
[stylish]: https://chrome.google.com/webstore/detail/stylish/fjnbnpbmkenffdnngjfgmeleoegfcffe
[canon-jenkins]: https://github.com/rackerlabs/canon-jenkins
[heldroe]: https://github.com/Heldroe
[generator]: http://jenkins-contrib-themes.github.io/jenkins-material-theme
[bootstraponline]: https://github.com/bootstraponline
