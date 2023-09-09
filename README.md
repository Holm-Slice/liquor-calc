# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

// for this app we are going to be making a simple costing calculator for prices that should be charged liquor (liquid) at diff cost %'s
// we are going to need to define several variable and classes to proivide a range of outputs (prices at various pours) and inputs(sizes and prices).
// These variable will include btl sizes in ml/ozs, cost per btl which we will use to create outputs of vary costs depending on the sizes/volumes of pours (ammounts used in ml/oz) at given price point %'s
// the scope of the size of btls will be 200ml - 1.7l or 6.8oz - 59.2 oz (type out later)
// the scope of volume or pour out puts will range from .25-3.0 ozs (.25, .5, .75, 1, 1.5, 2, 2.5, 3)
// the scope of the cost %'s will range from 15-25%
// ----> this will equate to the $ ammount that needs to be charged a x % to
// these values will need to be filled into forms with selector options (or potetntially different "pages") on which metric of measurement is going to be calculated btw ml/oz
// we will need to create two mathmatical functions
// the first should price out costs per pour at varying volumes and %'s
// ----> this intial fnct (f1()) will be determined as cost by volume (oz/ml) = cost per bottle / size per btl (oz/ml)
// --------> this function should render as a table (tbl1)
// the second funtion will nee to calculate the percentage that would need to be charged to @ varying %'s of cost
// ----> this second fnct (f2()) will be determined as charge price by % = cost per volume (oz/ml) \* the desired percent of cost (15% = .15, etc)
// outputs should render as a table based on the input btl size with a y axis of cost %'s low(top) - high(bottom) and the x axis should contain the pour volumes with the output being would be the cost of what you would charge for varying volumes of pours
// --------> should fnct should render as a table below tbl1

// Phase 2
// create a seperate form and possibly importing cost by volume previously calculated of various components
// components of this form should include cost per volume (used) and be sorted into columns of info such as... (cocktail name placeholder with values and keys for ingredients used ie: liquors, juices, bitters, etc.
// create fcnt that add up total cost of ingredients (sum of x+y+z etc.; tci) / price charged on menu (menuPrice) = net cost % (costP)
// ----> (fnct3()) = {tci / menuPrice = costP}
// -------> tci could be a sum variable / in itself

//Phase 3
// eventually make tabs/pages for beer by the keg/can/btl and wine by the gl/btl
