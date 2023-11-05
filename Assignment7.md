1- various wasys to add image to our app
2- what will happen if we do console.log(useState())?
ans-it returns a array onto the console in browser.
-----------------------------------------------------------------
3- How useEffect behaves if we dont add a dependecy array ?
ans- useEffect has two parameters , first is a callback fucntion and other is dependency array.
dependency array declaration is not important. but we have to give a call back function to useEffect hook.
useEffect is called everytime the component renders. if we dont put a dependency array in here then, it will render everytime the component renders(it is the default behaviour), but if we have a dependecny array then , useEffect will be rendered only when there is a change in the state variables present in the array. and if we have a empty dependency array . useEffect will be called only in the initial render. the component loads the useEffect is called and that's all.
useEffect (()=>{}, [])
-----------------------------------------------------------------------
4- What is SPA?
ans-stands for single page Application. even when we route or go to another page even then, we dont change the page we just change the component. browser will not refresh the page.
like in older days when we visit another page the whole page reloads/refreshes.
===================================
5 - Diffrence in client side and server side routing?
ans - #server side routing: when we click our anchor tag, it reloads the whole page, sends a network call for the page and then fetch the html from server and shows us the page.
      
#client side routing: All the components are loaded into our app so we don't have to make external network calls to fetch the networks/ servers. when the app is loaded for first time, all components are already there and when clicking link the component is loaded.
