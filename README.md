```
Demo to show a bug with svelte5 transitions in versions

svelte@5.0.0-next.97 and onwards. (96 is fine).

If an Element if wrapped into a component, transitions break. The minimal demonstrator shows two divs which are exactly the same with one difference:
- the red div: inlined
- the green div: wrapped into component

Instructions:
- npm install
- npm run dev
- navigate to http://localhost:5173/test/
- click the button. You will see the green div not being transitioned in over time but simply appearing.

```
