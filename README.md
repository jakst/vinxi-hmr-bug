This is a reproduction of an issue in Vinxi. The vinxi dev server should only watch for changes in `index.html` with the current setup, but changes in `index2.html` also triggers page reloads.

To reproduce:

1. `pnpm install`
2. `pnpm dev`
3. Open the app in your browser and make a change to [index2.html](./index2.html)
4. Observe that the console prints a message about reloading the page because of
   changes in `index2.html`, and the page makes a full reload.
