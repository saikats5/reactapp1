# reactapp1

A javascript library for building user interfaces

//default export
export default person //person.js
import person from './person.js';
import psn from './person.js';


//named export
export const clean = () => {}; //test.js
export const test = 33; //test.js
import {clean, test} from './test.js';
import {ts as test} from './test.js';
import * as bundled from './test.js'; //bundled.test

SPREAD - used to split array elements or object properties
const newArray = [...arr, 1,2]
const newObj = {...obj, newprops: 5}

REST - used to merge a list of function arguments into an array
function sortArgs[...args]{
    return args.sort();
}

DESTRUCTURING
[a,b] = ['Hello', 'World']
{name} = {name: 'Max', age: 20}
age //undefined

//create-react-app react-app // create the app

registerServiceWorker();//below ReactDOM
The service worker is a web API that helps you cache your assets and other files so that when the user is offline or on slow network, he/she can still see results on the screen, as such, it helps you build a better user experience, that's what you should know about service worker's for now. It's all about adding offline capabilities to your site.

Compiled react
return React.createElement('div', {className: 'App'}, React.createElement('h1', null, 'header element'));

onclick --> javascript but in jsx --> onClick={}
follow standard Handler with functionname, don't add () on click handler, this will execute immediately
setState is provided by React.Component

react hooks in React 16

class App extends Component {
    state = {
        test1: [],
        test2: 'sometext'
    }
}

import React, { useState } from 'react';
const app = props => {
    const arr = //const [ nameState, setName ] = useState({  //returns 2 elements array //1st object, 2nd function to change the                                 object
        persons: [
            { name: 'max', age: 22 },
            { name: 'mat', age: 23 }
        ],
        otherState: 'sometext'
    })

    //useState({otherState: 'some other text'});
    //const [otherState, setOtherState] = useState('some other other text');

    const clickHandler = () => {
        setName({
            persons: [
                { name: 'maxy', age: 22 },
                { name: 'maty', age: 23 }
            ],
            otherState: nameState.otherState
        })
    }
}

//setName will completely replace the state, otherstate will be removed