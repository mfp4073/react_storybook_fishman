# Take Home Assignement

### Running the project.
The serve, client and storybook are dockerized and the client will support hot loading so you can work on the front end without having to restart it. Cloen the repo, create a .env file in the root and add the following to it. After that, docker-compose up with start the projct

```sh
STORIES_PORT=6006
CLIENT_PORT=3000
SERVER_PORT=5000
```

### In browser
The client will run on http://localhost:3000
The storybook will run on http://localhost:6006

### About the project

I chose to make a small example of a self contained small node rest server, React app and Storybook that run from the same project. I wanted to challenge myself by doing something new so I chose to get into Docker as it is something I've wanted to use but haven't had the opportunity yet.  I used a d3 wrapper library called Brightcharts to make the ineractive donut chart. The Storybook is set up so I can show using buttons and a header inside the actual application as well as the Storybook. The power of Storybook is that a product owner can explore 'controls' on the components being built - they are the same ones being used within the actual  application but served in isolation. This allows a team to work on a UI without having to navigate an application for demos, QA or development. It's also an easier way to maintain control of and track variants and edge-cases of UI components - e.g. a button state or button variant set by a user state or prop. This makes creating and maintaining a component library for a company or team simple, clean and scalable. Any code changes to the components in the client will be reflected in the component library.

### Challenges and going forward

I had challenges getting Storybook to work Dockerized unlike the Node server and React app. Having it self contained would be the end goal but there is little documentation on Dockerizing Storbybook as opposed Node and React. Regardless, Docker was a fun challenge.

Adding more controls in for the components would probably be the first thing I would add for the stories. Allowing a stakeholder to be able to interact with the components more would help design the UX come to life faster and with less iteration. Going forward it would be great to move beyond the component heirarchy up to pages to expand the components into a sandboxed but more connected environment. Another step would be to possibly implement styled components and making use of React's compound components pattern. This would make the library less tightly coupled with the order of a components children and use component-level styles).




