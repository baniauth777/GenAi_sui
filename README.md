// App.js import Home from "./pages/Home";

function App() { return <Home />; }

export default App;

// index.css @tailwind base; @tailwind components; @tailwind utilities;

// tailwind.config.js module.exports = { content: ["./src/**/*.{js,jsx,ts,tsx}"], theme: { extend: {}, }, plugins: [], };

// src/pages/Home.jsx import Navbar from "../components/Navbar"; import Hero from "../components/Hero"; import Footer from "../components/Footer";

const Home = () => { return ( <> <Navbar /> <Hero /> <Footer /> </> ); };

export default Home;

// src/components/Navbar.jsx const Navbar = () => { return ( <nav className="flex justify-between items-center p-6 bg-black text-white"> <h1 className="text-xl font-bold">Orimex</h1> <ul className="flex space-x-6"> <li className="hover:text-purple-400 cursor-pointer">Home</li> <li className="hover:text-purple-400 cursor-pointer">Staking</li> <li className="hover:text-purple-400 cursor-pointer">AI Agent</li> <li className="hover:text-purple-400 cursor-pointer">Whitepaper</li> </ul> </nav> ); };

export default Navbar;

// src/components/Hero.jsx const Hero = () => { return ( <section className="h-screen bg-gradient-to-br from-gray-900 to-black text-white flex flex-col justify-center items-center text-center px-4"> <h2 className="text-4xl md:text-6xl font-bold mb-6">AI Crypto Trading Agent</h2> <p className="text-lg max-w-xl mb-8"> Automated AI agents to trade crypto for you. Stake. Earn. Repeat. </p> <button className="bg-purple-600 hover:bg-purple-700 px-6 py-3 rounded-xl text-white font-semibold"> Launch App </button> </section> ); };

export default Hero;

// src/components/Footer.jsx const Footer = () => { return ( <footer className="bg-black text-white text-center py-6 mt-20"> <p>© 2025 Orimex. All rights reserved.</p> </footer> ); };

export default Footer;

