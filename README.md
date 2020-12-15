## Setup Notes


PROBLEM: The local coffee shop seeks to increase customers using a website to promote sales. The coffee shop seeks to enhance their brand with a simple, mobile-first, website that showcases their coffee. This is a single landing page layout with different sections and a variety of functionalities such as a load/hide sidebar, responsive buttons and google map embedded frame. This coffee landing page is just an example of what could be achieved for a customer in relatively small time as an initial prototype. The landing page consists of: Home, About, Work, and Contact.

ACTION: To prototype the website, HTML, CSS, and JavaScript was used to quickly create the layout of the website. The website follows a responsible design approach and can be easily shown on a smart phone, a tablet and a regular Desktop computer.


1. All components ready to go (including imports)
2. Use main.css - less imports
3. Limit amount of components - better overview
4. React Icons

[react icons] :https://react-icons.github.io/react-icons/

```javascript
import { FaHome } from "react-icons/fa"
const Component = () => {
  return <FaHome className="icon"></FaHome>
}
```

5. Use constants to avoid repetition.
6. In order to follow along with the video use my backend (url below)

   [strapi backend]:https://github.com/john-smilga/strapi-gatsby-porfolio-2020-api

7. Make sure such content-types exist in your Strapi application. Or replace/delete them in gatsby-config.js

```javascript
{
      resolve: `gatsby-source-strapi`,
      options: {
        apiURL: `http://localhost:1337`,
        queryLimit: 1000, // Default to 100
        // contentTypes: [`jobs`, `projects`, `blogs`, ],
        //singleTypes:[`about` ]
        contentTypes: [`jobs`, `projects`, `blogs`],
        singleTypes: [`about`],
      },
    },
```
