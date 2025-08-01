###### **REACT SMART CONTRACT LOTTERY SETUP**



npm install wagmi viem @rainbow-me/rainbowkit

yarn add @tanstack/react-query

yarn add @tanstack/react-query





**HOSTING YOUR WEBSITE IN MANUAL WAY**

---

**to view your IPFS deployed file-** https://ipfs.io/ipfs/<your CID>



yarn build **after updating vite.config.js**

**'''**
import { defineConfig } from 'vite'

import react from '@vitejs/plugin-react'



export default defineConfig({

&nbsp; plugins: \[react()],

&nbsp; base: './', // Use relative paths for IPFS

&nbsp; build: {

&nbsp;   outDir: 'dist',

&nbsp;   assetsDir: 'assets',

&nbsp;   sourcemap: false, // Optional: disable for smaller builds

&nbsp; }

})

'''

**if also using react router you need to do this too**

**'''**
import { HashRouter as Router, Routes, Route } from 'react-router-dom'



function App() {

&nbsp; return (

&nbsp;   <Router>

&nbsp;     <Routes>

&nbsp;       <Route path="/" element={<Home />} />

&nbsp;       <Route path="/about" element={<About />} />

&nbsp;       {/\* other routes \*/}

&nbsp;     </Routes>

&nbsp;   </Router>

&nbsp; )

}

'''

