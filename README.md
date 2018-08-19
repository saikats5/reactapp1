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
