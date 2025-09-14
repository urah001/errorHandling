# errorHandling

this is my personal error handling documentation i dont think its the standard way of error handling but at least it works 

<details> 
 <summary> npm ERR! code ERESOLVE </summary>
 error   :

 - npm ERR! code ERESOLVE
- npm ERR! ERESOLVE unable to resolve dependency tree
- npm ERR!
  
- ```temporary sol:  npm i kinde-angular --legacy-peer-deps ```                           

</details>

---
<details>
 
<summary> bus error </summary>

- error
- $ npm run dev / start
- $ [project name][version] dev
- $ next dev
- $ bus error 
 

 - temporary sol : A Bus Error when running npm run dev with Next.js (using Turbopack) usually means there's a low-level issue with memory access.
 - Here’s how to fix it:

Clear npm Cache & Reinstall Dependencies

Corrupted dependencies can cause bus errors.

```
rm -rf node_modules package-lock.json
npm cache clean --force
npm install
npm run dev
```
If you’re using Yarn:
```
rm -rf node_modules yarn.lock
yarn cache clean
yarn install
yarn dev
```
 Delete & reinstall dependencies (rm -rf node_modules && npm install).

5. Run in Safe Mode (NODE_OPTIONS="--napi-modules").
   

</details>

---

<details>
 
 <summary> package.json : unable to load  </summary>

 
- Error:  Unable to load schema from 'https://json.schemastore.org/package': getaddrinfo EAI_AGAIN .

- solution : reload/restart vs code  
  
</details>

---
<details>
 
 <summary> angular : command not available </summary>

- $ ng serve
 
- Error: This command is not available when running the Angular CLI outside a workspace.

- solution : right click on the folder and click the `open intergrated terminal here` or cd to the project main folder and rerun 
  
</details>

---

<details>
 <summary>
 npm run dev  ✓ Starting... then stops
 </summary>

-solution : restart your pc / system 
-solution2 : reinstall node modules and pack.lock.json
 
</details>

---


<details>

<summary>
 Your custom PostCSS configuration must export a `plugins` key.
</summary>

solution : edit or add if you dont have a `postcss.config.js`/`postcss.config.mjs` file with this : 

```

// postcss.config.mjs
import tailwindcss from 'tailwindcss'
import autoprefixer from 'autoprefixer'

/** @type {import('postcss-load-config').Config} */
const config = {
  plugins: [tailwindcss, autoprefixer],
};

export default config;
```
 
</details>

---

<details>

<summary>
 hydration warning
</summary>

 solution : put 
 ```
 suppressHydrationWarning
```  
 
 in 
 
 <html lang="en" suppressHydrationWarning> 
 
 located in the app/layout.tsx
</details>

---

<details>

 <summary>
  files not uploading in git
 </summary>
 
> git push -u origin main
error: RPC failed; HTTP 408 curl 22 The requested URL returned error: 408
send-pack: unexpected disconnect while reading sideband packet
fatal: the remote end hung up unexpectedly
Everything up-to-date

```soln``` : check for a network issues or big files , github deosnt allow big file 
</details>

---

<details>

 <summary>
  Import "[module]" could not be resolvedPylancereportMissingImports
 </summary>

```soln``` : add ``` # type: ignore ``` to the end of the import statement to ignore this warning if you know you already installed this 

</details>

---


