# Jitsi_Developer_Notes


Embedding Jitsi in a web app through iFrame:
https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-iframe

Feature layout

When adding a new feature, this would be the usual layout.

react/features/sample/<br />
├ actionTypes.js<br />
├ actions.js<br />
├ components<br />
├── AnotherComponent.js<br />
├── OneComponent.js<br />
└── index.js<br />
├ middleware.js<br />
└ reducer.js<br />

The middleware must be imported in react/features/app/ specifically in middlewares.any, middlewares.native.js or middlewares.web.js where appropriate. Likewise for the reducer.

An index.js file must not be provided for exporting actions, action types and component. Features / files requiring those must import them explicitly.

This has not always been the case and the entire codebase hasn't been migrated to this model but new features should follow this new layout.

When working on an old feature, adding the necessary changes to migrate to the new model is encouraged.

https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-contributing#feature-layout
https://github.com/jitsi/jitsi-meet/blob/master/doc/examples/api.html

REST API |  jitsi-meet/resources/cloud-api.swagger 
https://app.swaggerhub.com/apis/smachaje/SwaggerVideo/1.0.0

Self-Hosting Guide - Docker
https://jitsi.github.io/handbook/docs/devops-guide/devops-guide-docker

Jitsi on Amazon AWS with cluster optimization:
https://aws.amazon.com/blogs/opensource/getting-started-with-jitsi-an-open-source-web-conferencing-solution/

Jitsi Architecture diagram:
https://jitsi.github.io/handbook/docs/devops-guide/devops-guide-manual#network-description

Jitsi React code:
https://github.com/jitsi/jitsi-meet/tree/master/react

Changing the basics: logo/title
https://technologyrss.com/how-to-customize-jitsi-meet-video-conference-server/

Youtube video, into to Jitsi architecture:
https://www.youtube.com/watch?v=7vFUVClsNh0&feature=youtu.be

Embedding video session in an external app:
https://www.youtube.com/watch?v=d67z7FrP-Hs

Electron apps:
https://www.youtube.com/watch?v=3yqDxhR2XxE

Developer forum:
https://community.jitsi.org/c/dev/6

Jitsi Meet React Component
An unofficial React component which wraps the standard Jitsi Meet JS API. It is written in Typescript to help you configure the library with ease, and get your super important meetings up and going, in a blink of an eye.
https://www.npmjs.com/package/react-jitsi

React tutorial:
https://dev.to/metamodal/add-jitsi-meet-to-your-react-app-33j9

Sandbox:
https://codesandbox.io/s/react-jitsi-demo-qjoei?module=%2Fsrc%2FVideoConference.jsx

