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
