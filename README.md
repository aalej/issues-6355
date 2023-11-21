# Repro for Firebase Tools issue 6355

### Versions

firebase-tools: v12.9.1<br>
node: v18.16.1<br>

### Steps for setup

1. Run `npx create-next-app web-app`
   - ✔ Would you like to use TypeScript? Yes
   - ✔ Would you like to use ESLint? Yes
   - ✔ Would you like to use Tailwind CSS? Yes
   - ✔ Would you like to use `src/` directory? Yes
   - ✔ Would you like to use App Router? (recommended) Yes
   - ✔ Would you like to customize the default import alias? No
1. Run `cd web-app`
1. Run `firebase experiments:enable webframeworks`
1. Run `firebase init`
   - Select "Realtime Database", "Functions", and "Hosting"
   - Select "Don't set up a default project"
   - Hit "Enter" for the rest. Choose default options
1. Run `firebase emulators:start --project demo-project --only hosting`
1. Open "127.0.0.1:5000" on a web browser
   - Default Next.js web page is displayed
