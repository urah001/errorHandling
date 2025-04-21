# errorHandling

this is my personal error handling documentation i dont think its the standard way of error handling but at least it works 

- error { 
- npm ERR! code ERESOLVE
- npm ERR! ERESOLVE unable to resolve dependency tree
- npm ERR!
- } 
- temporary sol:  npm i kinde-angular --legacy-peer-deps                            

- error {
- npm run dev / start
- [project name][version] dev
- next dev
- bus error 
- }
- temporary sol : A Bus Error when running npm run dev with Next.js (using Turbopack) usually means there's a low-level issue with memory access. Here’s how to fix it:


---

🔥 Possible Causes & Fixes

1️⃣ Clear npm Cache & Reinstall Dependencies

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
