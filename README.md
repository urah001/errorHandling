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

rm -rf node_modules package-lock.json
npm cache clean --force
npm install
npm run dev

If you’re using Yarn:

rm -rf node_modules yarn.lock
yarn cache clean
yarn install
yarn dev

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
