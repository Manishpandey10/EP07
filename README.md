HOOKS SHOULD ONLY INSIDE THE COMPONENT , NOT OUTSIDE THE COMPONENT FUNCTION.
# useEffect
- it takes 2 parameters first is a callback fucntion and other is a dependencies array.
useEffect is called everytime the component renders. if we dont put a dependency array in here then, it will render everytime the component renders, but if we have a dependecny array then , useEffect will be rendered only when there is a change in the state variables present in the array. and if we have a empty dependency array . useEffect will be called only in the initial render. the component loads the useEffect is called and that's all.
- the callback fn will be called, after the component renders. 


- why we need state variable?
ans - we need state variables to track the variable, if we simply use the variable and somehow update the value , the UI will not be updated automatically. 
const [value, setvalue] = useState(default value for the variable)
here value is the variable and setValue is a fucntion which will update the UI ,
when ever setValue is executed i.e the value of  state variable changes the React will re render the  whole component and show us the updated value.

- why varible is getting updated and changing value since it is a const value and what is updated the element containig state variable or the whole component!!

ans- initial "value" and "value" after invoking the set Function are two diffrent variable, when ever the function is called, the whole component is re rendered === whole component is invoked and a new instance of the variable is created with updated value. and react using diffing algo. finds the diffrence in the older version of component and newer one , and where ever element the variable is used will be updated . 

* when ever local state variable is changed/updated , the component is rerendered. react triggers a reconciliation cycle.

* #server side routing: when we click our anchor tag, it reloads the whole page, sends a network call for the page and then fetch the html from server and shows us the page.
      
* client side routing: All the components are loaded into our app so we don't have to make external network calls to fetch the networks/ servers. when the app is loaded for first time, all components are already there and when clicking link the component is loaded.