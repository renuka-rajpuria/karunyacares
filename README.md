### Website for Karunya Cares - Mental Health Platform at Karunya University

### Project Overview:
- Technologies:
    React JS
    Tailwind CSS

- Concepts:
    - SPA (Single Page Application)
    - Modern UI/UX 
    - Fundamental CSS Flex-box properties.
    - Soft and pleasant animations and perfect gradients.
    - Perfectly placed media queries for satisfactory responsiveness on all devices.
    - Deploying it on hostinger.

### Steps:

#### 1. Setup

1.1 Type `npm create vite@latest my-project -- --template react` in the terminal, provided you have nodejs installed, if not run this command after installing it. More about Vite [here](https://vitejs.dev/)

1.2 Give the project name in the terminal and then in this case our framework is going to be react without ts (typescript).

1.3 Once done, cd into the code folder and run `npm install`, once all the dependencies are installed, proceed with `npm run dev` and click on the link to get the basic webpage up and running.

1.4 Once we do this to realise what vite has helped us with we can go to the `package.json` file only to see not many things are listed under dependencies.

1.5 Install Tailwind CSS using (from [here](https://tailwindcss.com/docs/guides/vite)):
```
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

1.6 Complete the `tailwind.config.cjs` file's code and then define the styles in `src/index.css`.

1.7 Next, go to `src/App.jsx` and delete everything present there already and type `rafce` to generate boilerplate code for react.

1.8 We will delete the `src/App.css` and `Assets` folder as we will be adding our custom files.

1.9 Then we will create a `constants` folder in the main project folder and inside it create a `index.js` file which will contain all the static text that is going to be displayed on the website.

#### 2. Structure and Layout

2.1 Note that if a react functional component simply returns jsx then we can remove the return statement and the curly braces to make the code look cleaner and also reduce another level of hierarchy.

2.2 Then the last file to write is `src/styles.js` that contains the styles that will help with the basic layout, it is a collection of class names that are tied to one single string.

2.3 This is what `App.jsx` should look like:
```
import styles from './style';

const App = () => (
    <div className="bg-primary w-full overflow-hidden">
      <div className={`${styles.paddingX} ${styles.flexCenter}`}>
        <div className = {` ${styles.boxWidth}`}>
          Navbar
        </div>
      </div>

      <div className = {`bg-primary ${styles.flexStart}`}>
        <div className={`${styles.boxWidth}`}>
          Hero
        </div>
      </div>

      <div className = {`bg-primary ${styles.paddingX} ${styles.flexStart}`}>
        <div className={`${styles.boxWidth}`}>
          Stats
          Business
          Billing
          CardDeal
          Testimonials
          Clients
          CTA
          Footer
        </div>
      </div>
    </div>
  );


export default App
```
2.4 Create a `src/components` folder with the following .jsx files and use `rafce` in all of them to structure your files:
Business.jsx
Button.jsx
CTA.jsx
CardDeal.jsx	
Clients.jsx
FeedbackCard.jsx
Footer.jsx
GetStarted.jsx
Hero.jsx
Navbar.jsx
Stats.jsx
Testimonials.jsx

2.5 When we have multiple components, instead of importing them all in separate lines in App.jsx we can instead create a `index.js` file in the components folder that will export all the components, it will look like this:
```
import Navbar from "./Navbar";
import Billing from "./Billing";
import CardDeal from "./CardDeal";
import Business from "./Business";
import Clients from "./Clients";
import CTA from "./CTA";
import Stats from "./Stats";
import Footer from "./Footer";
import Testimonials from "./Testimonials";
import Hero from "./Hero";

export {
  Navbar,
  Billing,
  CardDeal,
  Business,
  Clients,
  CTA,
  Stats,
  Footer,
  Testimonials,
  Hero,
};
```

2.5 VSCode Trick to quickly complete all the text elements into components:
Double click on the text elements and press alt while double clicking on all the others, then press control key and left arrow and then add `<` and then press control key and right arrow and close the tags.

2.6 `Ctrl + W` to close the applications in VS Code

#### 3. Navbar



#### 4. Hero Section

#### 5. Stats

#### 6. Business Section

#### 7. Billing Section

#### 8. Card Deals

#### 9. Testimonials

#### 10. CTA Section

#### Footer



